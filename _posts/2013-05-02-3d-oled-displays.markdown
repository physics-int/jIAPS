---
layout: post
title: 3D OLED Displays
date: 2013-05-02 07:56:39.000000000 +02:00
type: post
published: true
status: publish
categories:
- Article
tags:
- 3D
- displays
- flexible
- glasses
- OLED
- Samsung
- TV
meta:
  _edit_last: '1'
  _thumbnail_id: '173'
  _wpas_done_all: '1'
  _wpas_skip_2192546: '1'
  _jetpack_related_posts_cache: a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1442006271;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:7;}i:1;a:1:{s:2:"id";i:184;}i:2;a:1:{s:2:"id";i:798;}}}}
author:
  login: bertu
  email: norbert@bonnici.co
  display_name: Norbert Bonnici
  first_name: Norbert
  last_name: Bonnici
---
<h1>Introduction to 3D displays</h1>
<p>What must a 2D plane do to make a viewer think that they are actually looking into a 3D space? This has been a question to many scientists and engineers worldwide to create a non-volumetric display which is capable of giving viewers stereoscopic cues for a monocular system: [1]</p>
<ul>
<li>occlusion which is the effect of an object partially covering another and the effect of shadows,</li>
<li>linear perspective which is how same sized objects vary in size on the retina depending on the viewing distance,</li>
<li>depth of field, since the eye adapts its lens to accommodate for a focused object,</li>
<li>how objects look diffused (due to the atmosphere) when viewed from a large distance,</li>
<li>and relative scales according to known objects (example a dog).</li>
</ul>
<p>New 3D displays now add binocular support thus we are able to observe cues such as stereo and movement parallax which are effects of seeing different images with each eye and how we move our heads respectively. Stereo parallax is usually the main feature of all 3D displays, to give viewers depth perception. [2]</p>
<h1>Introduction to OLED displays</h1>
<p>In the 1960s electro-luminescence, which is the generation of light using an electrical excitation, was observed in organic semiconductors for an anthracene single crystal, through recombination (the capture of injected electrons and holes) and excitons (their exited states). A typical Organic Light Emitting Diode (OLED) display consists of a conjugated polymer Poly-Phenylene Vinylene (PPV) which acts as the main semiconductor layer between metallic electrodes, typically Indium-Tin Oxide (ITO) as a Hole Injection Layer (HIL) and a Magnesium alloy or Aluminium as the cathode (electron injection layer), as seen in Figure 1. [3, 4]</p>
<p>However more advanced materials such as Graphene are ready to take ITO's place since it allows for flexible displays while improving the transparency. In addition, Graphene does not have a band-gap which allows it to work across a larger part of the electromagnetic spectrum, from ultraviolet to infra red. Figure 2 prototypes. [5]</p>
<p>[caption id="attachment_171" align="aligncenter" width="314"]<img class=" wp-image-171 " alt="Figure 2: A prototype of a graphene flexible OLED display. [5]" src="{{ site.baseurl }}/assets/graphene.png" width="314" height="452" /> Figure 2: A prototype of a graphene flexible OLED display. [5][/caption]</p>
<h1>Glasses or no glasses?</h1>
<p>OLED displays are not volumetric displays thus to mimic the spatial cues of a 3D space, the display must hack our brain into thinking that we are actually viewing a 3D space rather than a flat plane.</p>
<h2>Stereoscopic Displays</h2>
<p>Stereoscopic displays require the user to wear special eye wear to be able to separate two channels of information (one for each eye) while making sure that the appropriate channel is going to the correct eye. Two main systems, which are currently being used are Active Shutter glasses and Polarised glasses.</p>
<p>The main disadvantage of such displays is that the glasses end up reducing the brightness of the image, which is currently the selling point of OLED displays. This is because OLEDs do not require a back-light since the display emits light on its own, while on the other side, a Liquid Crystal Display (LCD) requires a back-light.</p>
<h3>Active 3D</h3>
<p>Active 3D systems typically work by increasing the frame-rate (minimum of 100Hz for PAL and 120Hz for NTSC) at which the display operates to interleave two sets of images, one for the right eye and one for the left one. The glasses have active shutters which select which images should enter the eye at what time. They incorporate a synchronisation device which typically works via infra red or radio frequency. [1]</p>
<h3>Passive 3D</h3>
<p>Similar to a typical IMAX theatre, a passive system projects two sets of images at two different polarization angles (spatial multiplexing) which are then separated using polarized glasses to provide two distinct images for each eye. This is the cheapest and lightest system as it does not require the glasses to have electronics or shutters built into them. [1,2] Figure 3 depicts this.</p>
<p>[caption id="attachment_174" align="aligncenter" width="539"]<img class=" wp-image-174 " alt="Figure 3: Spatial multiplexing of polarised pixels to create two separate viewing channels. [2]" src="{{ site.baseurl }}/assets/polarised.png" width="539" height="247" /> Figure 3: Spatial multiplexing of polarised pixels to create two separate viewing channels. [2][/caption]</p>
<h3>Headset</h3>
<p>A simple method is to mount two OLED displays in a headset, one for each eye thus being able to view two sets of images, one on each side to give the impression of a 3D space. This version only works with one user but it is cost effective as only two small displays are required. [1]</p>
<h2>Auto-stereoscopic displays</h2>
<p>The great advantage for auto-stereoscopic displays is that they do not require glasses, which means anyone with two eyes can pop in front of the display and see a 3D effect. These displays are usually implemented using either a Parallax barrier or a Lenticular lens. Figure 4 shows the two types of auto-stereoscopic displays. The main disadvantage of auto-stereoscopic displays is that they have to sacrifice half of the horizontal resolution to accommodate for two separate viewing channels.</p>
<p>[caption id="attachment_175" align="aligncenter" width="346"]<img class=" wp-image-175 " alt="Figure 4: Auto-stereoscopic displays: a, shows a lenticular lens display. b, parallax barrier display. [1]" src="{{ site.baseurl }}/assets/auto.png" width="346" height="343" /> Figure 4: Auto-stereoscopic displays: a, shows a lenticular lens display. b, parallax barrier display. [1][/caption]</p>
<h3>Lenticular lens</h3>
<p>Lenticular lenses are cylindrical lenses aligned with columns of the OLED pixels, which are used to diffuse light so that it can only be seen from a specific angle from the display, which allows to direct the stereo images to the left and right eye individually.</p>
<p>We can obtain the distance between each lenticular lens using Equation 1, which gives the lenticular pitch, $latex l $, in terms of the pixel pitch, $latex i $, which is the distance between each pixel, the distance from the viewing windows, $latex z $, and the focal length, $latex f $. Figure 5 explains this visually. [2]</p>
<p>$latex l = 2i (z-f)/z $</p>
<p>[caption id="attachment_176" align="aligncenter" width="355"]<img class=" wp-image-176 " alt="Figure 5: A lenticular lens auto-stereoscopic display. [2]" src="{{ site.baseurl }}/assets/lenticular.png" width="355" height="266" /> Figure 5: A lenticular lens auto-stereoscopic display. [2][/caption]</p>
<h3>Parallax barrier</h3>
<p>The two-view parallax barrier display works by interlacing the left and right images in columns on the display and use optical apertures aligned with columns of the OLED pixels which block half of the image to separate the left image from the right in a viewing window as illustrated in Figure 6. This might be the simplest display to implement as only black strips are required to separate the image to provide two separate channels.</p>
<p>We can find the distance between each parallax barrier using Equation \ref{eq:barrier}, which gives the barrier pitch, $latex b $, in terms of the pixel pitch, $latex i $, the distance from the viewing windows, $latex z $, same as above, the gap between the barrier and the pixels, $latex g $. [2]</p>
<p>$latex b = 2i (z-g)/z $</p>
<p>[caption id="attachment_178" align="aligncenter" width="368"]<img class=" wp-image-178 " alt="Figure 6: A parallax barrier auto-stereoscopic display. [2]" src="{{ site.baseurl }}/assets/barrier.png" width="368" height="268" /> Figure 6: A parallax barrier auto-stereoscopic display. [2][/caption]</p>
<h1>Availability</h1>
<p>The largest 3D OLED display soon to be available on the market is the 55" 3D OLED Display by LG. [6] Samsung also have a similar display soon to be available. Many new smart phones are now using Active Matrix OLEDs as their displays, but 3D versions are not yet in the market. Yet some smart phones and game consoles such as the Nintendo 3DS are using auto-stereoscopic displays using a parallax barrier but with a different display technology, that of Super LCDs. [7]</p>
<p>[caption id="attachment_179" align="aligncenter" width="300"]<img class="size-medium wp-image-179" alt="Figure 7: The latest 55” OLED display from LG. [6]" src="{{ site.baseurl }}/assets/lg55-300x192.jpg" width="300" height="192" /> Figure 7: The latest 55” OLED display from LG. [6][/caption]</p>
<h1>Conclusion</h1>
<p>Various stereoscopic techniques such as active shutter glasses and parallax barrier, were covered in this article, which enable the display to produce high fidelity 3D images. 3D OLED displays are still in the pipelines but in a couple of years we will be able to purchase such advanced displays.</p>
<div title="Page 4">
<h1>References</h1>
<ol>
<li>Dodgson, N. Autostereoscopic 3D Displays. <em>IEEE Computer</em> <strong>38</strong>, 31–36 (2005).</li>
<li>Holliman, N. 3D display systems. <em>Science</em> <strong>38</strong>, 45 (2010).</li>
<li>Friend, R., Gymer, R. &amp; Holmes, A. Electroluminescence in conjugated polymers. <em>Nature</em> <strong>397</strong>, 121–128 (1999).</li>
<li>Fyfe, D. LED Technology: Organic displays come of age. <em>Nature Photonics</em> <strong>3</strong>, 453–455. issn: 1749-4885 (Aug. 2009).</li>
<li>Savage, N. Come into the light. <em>Nature</em> <strong>483</strong>, S38–9. issn: 1476-4687 (Mar. 2012).</li>
<li>LG. <em>LG</em> 55EM960V Television 2012. "http://www.lg.com/uk/tvs/lg-55EM960V-oled-tv".</li>
<li>Nintendo. <em>Nintendo</em> 3DS 2010.</li>
</ol>
</div>
