---
layout: post
title: Building “Winnie-the-Pooh” computer cluster
date: 2013-07-04 17:13:53.000000000 +02:00
type: post
published: true
status: publish
categories:
- Article
tags:
- clusters
- Computing
- High
- HPC
- Performance
- Winnie-the-Pooh
meta:
  _edit_last: '1'
  _thumbnail_id: '240'
  _wpas_done_all: '1'
  _wpas_skip_2192546: '1'
  _jetpack_related_posts_cache: a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1442331908;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:417;}i:1;a:1:{s:2:"id";i:198;}i:2;a:1:{s:2:"id";i:699;}}}}
author:
  login: maciej.lewicki
  email: lewickimaciejj@gmail.com
  display_name: Maciej Lewicki
  first_name: Maciej
  last_name: Lewicki
---
<div title="Page 1">
<p style="text-align: justify;"><em style="font-size: 13px;">Institute of Theoretical Physics</em><span style="font-size: 13px;">, University of Wrocław</span></p>
<div title="Page 1">
<p style="text-align: justify;">One of the main difficulties faced by modern physics is a barrier associated with finding analytic solutions to, sometimes seemingly easy, problems. Some of these problems can be analysed numerically with a good accuracy - using computers. Recent rapid development of technology, which allows us to explore more and with better precision, is described best by the Moore’s law. The law describes exponential increase in time of number of transistors used in integrated circuits [1]. Unfortunately, benefits of using computers in physics interfere with high cost of building and maintaining supercomputers. Cheaper, but less professional solution is building Beowulf clusters [2].</p>
<p style="text-align: justify;"><!--more--></p>
<h1 style="text-align: justify;">Computer clusters</h1>
<p style="text-align: justify;">Beowulf cluster is a multi computer architecture, which is capable of performing parallel computations [3]. Usually, this type of cluster consists of one computer, which is a server node and a number of computers, which are client nodes. All computers are connected into a Local Area Network (LAN) using a switch. Such a system can also be connected to the Internet, which allows users to have remote access to the cluster. The main node is a server for a group of programs controlling the work of the client nodes, while client nodes have the minimum number of software needed to connect to main node and to solve problems. This type of solution is beneficial, because all the nodes used in the architecture can be ordinary PCs. Nowadays PCs are so popular, that building a Beowulf cluster is relatively inexpensive. The cost of maintenance is also low and if one of the nodes is damaged it can be easily replaced with another PC. Expensive supercomputer components are not required. Beowulf uses Linux as an Operating System. All necessary software are free, which makes such a solution more affordable. Of course, Beowulf cluster has also a few negative aspects. Because we are operating a number of fully valuable computers, they consume a lot of energy. Moreover, Beowulf built with many nodes will also need plenty of space. Nevertheless, it is a perfect solution to satisfy needs and financial limitations of a group of students.</p>
<h1 style="text-align: justify;">"Winnie-the-Pooh" cluster</h1>
<p>[caption id="attachment_229" align="aligncenter" width="225"]<a href="http://jiaps.org/wp-content/uploads/2013/07/klaster.jpg"><img class="size-medium wp-image-229" alt="Winnie-the-Pooh cluster" src="{{ site.baseurl }}/assets/klaster-225x300.jpg" width="225" height="300" /></a> Figure 1: Winnie-the-Pooh cluster[/caption]</p>
<p style="text-align: justify;">To build our cluster we used secondhand computers donated by a local company. We were given 5 PCs, which unfortunately had different hardware configuration.</p>
<p style="text-align: justify;"><a href="http://jiaps.org/wp-content/uploads/2013/07/Screen-Shot-2013-07-04-at-17.00.33.png"><img class="aligncenter size-medium wp-image-232" alt="Screen Shot 2013-07-04 at 17.00.33" src="{{ site.baseurl }}/assets/Screen-Shot-2013-07-04-at-17.00.33-300x232.png" width="300" height="232" /></a></p>
<p style="text-align: justify;">We were also given a 24-port switch from the resources of our university. On each node we installed Ubuntu Server 2.6.32 and following software</p>
<p style="text-align: justify;"><a href="http://jiaps.org/wp-content/uploads/2013/07/Screen-Shot-2013-07-04-at-17.00.49.png"><img class="aligncenter size-medium wp-image-233" alt="Screen Shot 2013-07-04 at 17.00.49" src="{{ site.baseurl }}/assets/Screen-Shot-2013-07-04-at-17.00.49-300x118.png" width="300" height="118" /></a></p>
<h1 style="text-align: justify;">Performance tests</h1>
<p style="text-align: justify;">In order to test "Winnie-the-Pooh" cluster efficiency we run a program that uses capabilities of parallel programming. We used the Message Passing Interface (MPI) communication protocol. The program is an implementation of the Ising model. All measurements were taken using unix <em>time<strong> </strong></em>program(<em>user</em> value), 10 times per each number of nodes and taking the average value.</p>
<p>[caption id="attachment_238" align="aligncenter" width="300"]<a href="http://jiaps.org/wp-content/uploads/2013/07/article.png"><img class="size-medium wp-image-238" alt="&quot;Winnie-the-Pooh&quot; cluster efficiency" src="{{ site.baseurl }}/assets/article-300x210.png" width="300" height="210" /></a> Figure 2: "Winnie-the-Pooh" cluster efficiency[/caption]</p>
<p style="text-align: justify;">The second test we performed on the cluster was designed to verify its node-to-node communication abilities. To serve such purpose we used program generating Mandelbrot fractals [4]. Given desired coordinates, zoom and definition the output gives us a bitmap with a fractal. The default definition of 1280x720 pixels. Graphical effect is presented below.</p>
<p>[caption id="attachment_235" align="aligncenter" width="300"]<a href="http://jiaps.org/wp-content/uploads/2013/07/mandelbrot.jpg"><img class="size-medium wp-image-235" alt="Mandelbrot fractal" src="{{ site.baseurl }}/assets/mandelbrot-300x168.jpg" width="300" height="168" /></a> Figure 3: Mandelbrot fractal[/caption]</p>
<p style="text-align: justify;">The algorithm computes iterations of complex sequence, given by the equation: $latex z_{i+1} = z_i + c$, where c is a complex constant. The program generates proper colour by analysing the radius of convergence for given point and number of iterations. Each node computes these values for separate parts of the image and saves it to a file. Then, once again using MPI protocol, each node sends the data to master node, where proper colours in RGB scale are fitted.</p>
<p style="text-align: justify;">Transferred files weight only about 2 MBs and using the <em>time</em> utility we are hardly able to observe any decrease in efficiency, comparing to the earlier graph:</p>
<p>[caption id="attachment_234" align="aligncenter" width="300"]<a href="http://jiaps.org/wp-content/uploads/2013/07/gr.jpg"><img class="size-medium wp-image-234" alt="&quot;Winnie-the-Pooh&quot; cluster efficiency" src="{{ site.baseurl }}/assets/gr-300x210.jpg" width="300" height="210" /></a> Figure 4: "Winnie-the-Pooh" cluster efficiency[/caption]</p>
<p style="text-align: justify;">However the further analysis with <em>gprof</em> program let us observe, that communication functions take from 4% of time (2 nodes active) up to 11% (all nodes active). It is certainly satisfying efficiency for this simple type of computing cluster.</p>
<h1 style="text-align: justify;">Application</h1>
<p style="text-align: justify;">The purpose of constructing such a device was purely educational. Everyone involved in the process had a good chance of gaining a lot of knowledge from general linux environment usage, through hardware know-how and finally to real parallel programming. As the project got completed our interest in Beowulf clusters grew. It is a cheap and efficient way of obtaining your own mini-supercomputer. Even though the "Winnie-the-Pooh" does not provide with extraordinary computational power it has inspired us to undertake more innovative plan and build another Beowulf cluster. This time using much cheaper and more efficient single-board computers.</p>
<div title="Page 6">
<div>
<div>
<h1 style="text-align: justify;">References</h1>
<p style="text-align: justify;">[1] G.Moore. Cramming more components onto integrated circuit. <em>Electronics magazine</em>, 38:3, 1965.</p>
<p style="text-align: justify;">[2] J.Hall. Foreword,[in:] T. Sterling: <em>Beowulf Cluster Computing with Linux</em>, pages 5–6. MIT Press, Cambridge, second edition, 2003.</p>
<p style="text-align: justify;">[3] D.Eadline J.Radajewski. Beowulf howto. http://ibiblio.org/pub/ Linux/docs/HOWTO/archive/Beowulf-HOWTO.html.</p>
<p style="text-align: justify;">[4] J.W.Milnor. Dynamics in One Complex Variable (Third Edition), <em>Annals of Mathematics Studies</em> <em>160</em>. Princeton University Press.</p>
</div>
</div>
</div>
</div>
</div>
