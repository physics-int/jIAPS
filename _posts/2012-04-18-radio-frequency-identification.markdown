---
layout: post
title: Radio Frequency Identification
date: 2012-04-18 16:40:10.000000000 +02:00
type: post
published: true
status: publish
categories:
- Article
tags:
- Frequency
- Identification
- Radio
- RFID
meta:
  _edit_last: '1'
  _thumbnail_id: '71'
  _wpas_skip_2192546: '1'
  _yoast_wpseo_focuskw: rfid
  _yoast_wpseo_title: Radio Frequency Identification - jIAPS
  _yoast_wpseo_metadesc: RFIDs have existed for over 50 years and devices that roughly
    resemble the operating principles of RFIDs can be traced back to the Second World
    War.
  _yoast_wpseo_linkdex: '84'
  _jetpack_related_posts_cache: a:1:{s:32:"8f6677c9d6b0f903e98ad32ec61f8deb";a:2:{s:7:"expires";i:1442280764;s:7:"payload";a:3:{i:0;a:1:{s:2:"id";i:699;}i:1;a:1:{s:2:"id";i:898;}i:2;a:1:{s:2:"id";i:426;}}}}
author:
  login: ericpace
  email: ericpace@gmail.com
  display_name: Eric Pace
  first_name: Eric
  last_name: Pace
---
<div>
<h2><span style="font-size: 16px; line-height: 1.5;"><span style="font-family: Georgia, 'Times New Roman', serif; font-size: 34px; line-height: 44px;">History</span></span></h2>
<p>RFIDs have existed for over 50 years and devices that roughly resemble the operating principles of RFIDs can be traced back to the Second World War[1]. German scientists at the time discovered that by rolling their planes whenever they were returning to base, pilots changed the reflected radio signal and thus the radar crew on the ground could identify the aircraft[1, 2].</p>
<p>This system turned out to be a rudimentary form of a passive RFID. The British were also working on similar technology, and under Watson-Watt, the so-called Identify Friend or Foe system was developed.</p>
<p>The first work exploring these systems was published by Harry Stockman in the paper, “Communi- cation by means of reflected power”[3]. The first patent for an RFID system employing active tags and re-writable storage was received in the 1970’s[1].</p>
<p>In the 1990’s RFID technology was being deployed commercially, mainly finding applications such as electronic toll collection. Having been successful, other business areas were investing in RFID technology, most notably by Walmart.</p>
<p>Today, a single tag could be used for electronic toll collection, parking lot access as well as access to gated communities[1].</p>
<p>[caption id="attachment_73" align="aligncenter" width="640"]<a href="http://jiaps.org/wp-content/uploads/2012/04/rfid-circuits.png"><img class="size-single-thumbnail wp-image-73" title="Figure 1" alt="" src="{{ site.baseurl }}/assets/rfid-circuits-640x360.png" width="640" height="360" /></a> Figure 1: The images above illustrate the circuit and semiconductor chip that form a typical RFID tag.[4, 5[/caption][caption id="attachment_77" align="aligncenter" width="220"]<a href="http://jiaps.org/wp-content/uploads/2012/04/rfid_setup.jpg"><img class="size-archive-thumbnail wp-image-77" title="Figure 2" alt="" src="{{ site.baseurl }}/assets/rfid_setup-220x113.jpg" width="220" height="113" /></a> Figure 2: RFID system.[6[/caption]</div>
<div>
<h1>Advantages</h1>
<p>Currently, the more traditional barcode system is more widely used than RFID for tagging products and it it still the technology of choice for many applications. This is mainly due to the fact that RFIDs are more expensive. Thus we will not be seeing barcodes disappear any time soon.</p>
<p>However, there are many areas where RFID technology has prevailed. These are mainly industrial areas involving the shipment of goods.</p>
<p>The major advantage of RFID is that it does not require LoS to operate and thus products may be scanned from a distance, even if they are packaged in boxes or containers. While barcode systems are able to scan one item at a time, RFID systems can scan collections of items instantaneously, reducing labor requirements.[7]. Further advantages are that they can interrogate multiple items at the same time; they do not incur maintenance costs; they can store large amounts amounts of data (when compared to barcodes).</p>
<div>
<div>
<h1>RFID Types</h1>
<p>RFIDs may be categorized according to detection limits that different technologies impose on them.</p>
<h2>Close Coupled</h2>
</div>
</div>
<div title="Page 3">
<p>RFIDs operating the shortest range are called close-coupled systems. Typical interaction distance ranges from 0cm (contact) up to 1cm. At these ranges these systems generally operate in the near-field (discussed in section ). Thus the tag and the reader are coupled using both electric and magnetic fields and operate up to a range of 30MHz.</p>
<p>Close-coupling allows for the transfer of sufficient power to operate microprocessors in the tag. Such systems find application mostly in security strict environments[8].</p>
<h2>Remote Coupled</h2>
<p>These middle range systems operate mainly in the far-field region and have ranges up to 1m. They are based on magnetic induction caused reader within the tag and are thus known as inductive radio systems[8].</p>
<p>There are also a few systems employing capacitive coupling, however these form only 10% of the remote coupled category[8].</p>
<h2>Long Range</h2>
<p>Having the greatest range of operation, these systems operate via ultra high frequency electromag- netic waves. As a result, these systems use a different operating principle known as backscatter[8], and are thus known as backscatter systems. With passive backscatter, distances up to 3 metres may be achieved, while with active backscatter systems, ranges up to 15 metres have been achieved. Apart from backscatter systems, there are systems which use surface acoustic waves (discussed in section ) in the microwave range[8].</p>
<h2>Power</h2>
<p>Another way of classifying RFID systems is according to the way they receive power. The main distinction is between passive and active tags, however some sources mention semi-passive tags as well. However for most purposes, the terms active and semi-passive are analogous.</p>
<h2>Passive Tags</h2>
<p>Passive RFID tags consist of an antenna, a semi-conductor chip attached to the antenna and a protective covering to withstand environmental wear and to allow for easy attachment to goods. They are called passive RFID tags for the simple reason that they have no dedicated power source, but are powered completely through the field generated by the RFID reader itself[10]. The tag antenna captures the energy and powers the semiconductor chip just enough to transmit its ID. The covering is usually made out of glass or a laminar plastic substrate[11].</p>
<p>Passive tags can be very small, as they do not require a battery. Passive tags may be as small as a coin, however the smaller the tag, the shorter the read range[12]. Current passive RFID tags contain about 16 to 64 KB of memory[7].</p>
<p>&nbsp;</p>
<p>[caption id="attachment_80" align="aligncenter" width="640"]<a href="http://jiaps.org/wp-content/uploads/2012/04/passive_RFID_Park2011.jpg"><img class="size-single-thumbnail wp-image-80 " title="Figure 3" alt="" src="{{ site.baseurl }}/assets/passive_RFID_Park2011-640x360.jpg" width="640" height="360" /></a> Figure 3: This is an example of a Passive RFID tag[9[/caption]</div>
<div title="Page 4">
<p>The reader device may be set up to either broadcast its electromagnetic (EM) signal continuously or otherwise broadcast only when necessary. When the read is brought near an RFID tag, the EM signal is received by the tag through its antenna. Using diodes to rectify the radio frequency voltage, a charge within the tag’s capacitor is built up. A return signal is sent once the capacitor has built a sufficient amount of charge. This return signal is modulated according the data that is being sent to the reader.</p>
<h2>Active Tags</h2>
<p>Active tags, unlike their passive counterparts, have their own power source, allowing them to transmit stronger signals which increases their broadcast range significantly. The on-board power source makes these class of tags much more expensive. It also requires the tag to have larger physical dimensions. The typical sizes of active tags vary between the size of car key-fobs to the size of a mobile phone, depending on the ranges required.</p>
<p>Due to these limitations, these tags are used to track large items over large distances, such as container shipments from one country to another. Active tags are also useful when memory re- quirements and read ranges require the RFID system to operate at higher frequencies of up to 2.45GHz or 5.8GHz[12].. This is not possible with passive tags since they cannot provide sufficient power.</p>
<h1>Physical Principles</h1>
<h2>Near-Field</h2>
<p>“Faraday’s principle of magnetic induction is the basis of near-field coupling between a reader and a tag”[11]. A reader will establish an alternating magnetic field such that when a tag is placed within it, an alternating voltage is generated across its coils. The voltage may be rectified and accumulated in a capacitor to then be used to power the semiconductor. Tags that use near-fieldcoupling use load-modulation.</p>
<p>[caption id="attachment_83" align="aligncenter" width="640"]<a href="http://jiaps.org/wp-content/uploads/2012/04/active_RFID_Park2011.jpg"><img class="size-single-thumbnail wp-image-83" title="Figure 4" alt="actice rfid" src="{{ site.baseurl }}/assets/active_RFID_Park2011-640x360.jpg" width="640" height="360" /></a> Figure 4: This is an example of an Active RFID tag[9[/caption]Since the tag is powered by the magnetic field, this power consumption may be measured as a voltage drop in the reader antenna. The tag is supplied with a load resistance which may be switched on and off according to what data needs to be transmitted. The toggling of the load resistance will result voltage fluctuations which may be decoded by the reader to identify the data being sent – this technique is known as load-modulation, described below.</div>
<div>
<p>The issue with near-field communication is that as we increase the frequency, the distance over which the near-field coupling can operate decreases, according to the equation:</p>
<p>$latex r = \frac{c}{2\pi f}$</p>
<p>where f is the frequency of operation, c the speed of light and r is the usable range. Also the range over which we may transfer energy via the magnetic field drops at a rate of $latex 1/r^3$. Such limitations have led to techniques that make use of far-field coupling.</p>
<h2>Far-Field</h2>
<p>The tag receives EM waves propagating from the dipole antenna through a smaller dipole antenna attached to the tag. In these systems, the alternating voltage may be accumulated by rectifying it using a diode and charging up a capacitor. However unlike the near-field, the information held in the tag cannot be transmitted back to the reader using load-modulation.</p>
<p>The technique designers use for commercial far-field tags is called back scattering (see section ). In this technique the antenna will reflect back some of the energy, depending on its impedance. By varying this impedance with time, the tag’s ID pattern may be reflected back. Impedance tuning can be achieved by connecting a transistor across the dipole antenna.</p>
<p>Systems using far-field principles normally operate in the Ultra High Frequency (UHF) band (around 2.45GHz) and these systems’ range is limited by the energy that reaches the tag and by how sensitive the reader is to the reflected signal “The actual return signal is very small, be- cause it is the result of two attenuations, each based on an inverse square law. Thus the returning energy is $latex 1/r^4$”[11].</p>
<p>[caption id="attachment_86" align="aligncenter" width="220"]<a href="http://jiaps.org/wp-content/uploads/2012/04/RFID_backscatter.png"><img class="size-archive-thumbnail wp-image-86" title="Figure 5" alt="" src="{{ site.baseurl }}/assets/RFID_backscatter-220x150.png" width="220" height="150" /></a> Figure 5: Figure showing how Backscatter works[8[/caption]</div>
<div>
<p>Today, semiconductors require much less power to operate and with receivers of greater sensitivity, readers employing this system can interrogate tags up to 3 metres away[11].</p>
<h2>Backscatter</h2>
<p>RFID systems operating at ranges greater than 1 metre operate using the far-field principle and operate in the UHF bands. Such short wavelengths makes it possible to build very small antennae.</p>
<p>“Electromagnetic waves are reflected by objects with dimensions greater than around half the wavelength of the wave. The efficiency with which an object reflects electromagnetic waves is described by its reflection cross-section”[8]. When objects are resonating with the incident wave, such as what occurs when transmitting a signal at the resonating frequency of an antenna, a large reflection cross-section is observed. The reflection characteristics are further changed by varying the antenna’s resistance[8].</p>
<p>Figure 5 illustrates the backscatter operation. Power $P1$ is emitted from the reader. Following attenuation, power $latex P1^\prime$ arrives at the antennae of the tag as RF voltage. This voltage is rectified using <em>Schottky</em> diodes $latex D1$ and $latex D2$ as they have a low threshold voltage. Power $latex P2$ is reflected from the tag back to the reader. The amplitude of this power is modulated according to the data being transmitted. Power $latex P2^\prime$ arrives at the reader after attenuation.</p>
<p>Powers $latex P1$ and $latex P2^\prime$ are travelling in opposite direction. Since power $latex P1$ is stronger by a few orders of magnitude, it can be suppressed by a directional coupler. The ratio $latex \frac{P1}{P2}$ can be estimated using the radar equation.</p>
</div>
<div title="Page 7">
<div>
<div>
<h2>Surface Acoustic Waves</h2>
<p>Surface Acoustic Wave (SAW) devices are based on the piezoelectric effect. A mechanical stress on certain materials results in voltage across them[13]. This effect is also reversible. Usually these devices are operated in the 2.45GHz region.</p>
<p>The reader generates a pulse that is received by a transducer which converts the EM wave into an acoustic wave. The frequency of the surface wave corresponds to the transmission frequency. There are reflective strips affixed to the substrate positioned at varying distances which reflect the acoustic wave back to the transducer.</p>
<p>The number of pulses received by the transducer corresponds to the number of reflective strips. The delay between pulses corresponds to the distance between the strips. These pulses are converted back to high frequency EM waves and propagated back to the reader[8].</p>
<p>The storage capacity of a SAW based tag depends on the length of the substrate and on the minimum realizable distance between reflective strips. Ranges up to 1 to 2 metres may be achieved.</p>
<h1>Applications</h1>
<p>There are many areas where RFID technology has been found useful, as is mentioned in many articles.</p>
<p>David Dorman discusses library security systems[14]. Designs for communication between covert RFID tags are described in the paper by Pan and Narayanan[15].RFID systems have also found uses in blood banking for automatic inventory check-in[16]. A paper by Ziai and Batchelor discusses how people may be monitored via a new concept of placing ultra thin tags directly on the skin in the form of a tattoo.</p>
<h2>Security</h2>
<p>Today, most organizations require an efficient access control system.</p>
<p>This is mainly because the organization needs to control access to restricted areas and monitor employee activity within the premises. RFID is a great solution as the tags may be read from great distances away and multiple tags may be read at the same time.</p>
<h2>Weapons Tracking</h2>
<p>An example of Weapons tracking is the Australian Customs and Border Protection Service. Officers monitor the use of all weapons, vehicles and other gear and thus a system to provide real-time visibility into these assets is required. The initial solution to this problem was to use a flat file system and exchange it between central offices. However such reports were often inaccurate.</p>
<p>HF (13.56MHz) RFID system was adopted to replace the flat file system. With the RFIDs in place, the central office can track exactly where the items are located and immediately address any misplacements or losses.</p>
<h2>Animal Tracking</h2>
</div>
</div>
</div>
<div title="Page 8">
<p>For stock keeping, and in an effort to control epidemics, RFIDs are being used on livestock. There are different types of RFIDs such as collars or injectable tags or ear tags. RFID allows the identi- fication and tracking of individual animals and this allows the owners to manage feeding patterns and generate statistics for each animal in the livestock. Such information helps in the determination of when the animal should be bred or sent to the market.</p>
<p>Animal health is also an area which receives aid from RFIDs. “The ability to trace back through the food chain provides national and international health agencies a valuable tool in controlling the spread of diseases.”[17]. RFID systems are also being used in zoos for Real Time Tracking (RTL) of elephants via ankle bracelets[18]. The readers are positioned in towers and track the movement of the elephants.</p>
<h2>Clothes Tracking</h2>
<p>The best example of clothes tracking is WalMart. The company has been amongst the first to adopt RFID technology in order to be able to track shipments of products through the supply chain[19]. Recently in 2010, WalMart has also decided to adopt a more a rigorous approach as it now tracks individual items, insisting that “the devices are crucial to improving the logistics of inventory management”[20].</p>
<h1>Hazards</h1>
<h2>Radiation</h2>
<p>Electric fields may be divided into ionizing and non-ionizing radiation. “If EM energy is considered as a photon, then the energy of the photon depends on the frequency. The higher the frequency, the higher the energy”[21].</p>
<p>“The ionization energy or ionization potential is the energy necessary to remove an electron from the neutral atom”[22]. Photon energy must be higher than 300GHz[21] in order to be considered as ionizing. Thus RFID frequencies (operating between a few hertz up to 2.4GHz) are non-ionizing[23].</p>
<p>In studies of effects of radio waves on humans, two perspectives are considered: 1) the whole body averaged “specific absorption rate (SAR). SAR is the mass-normalized rate at which the energy of an electromagnetic field is coupled into an absorbing body; it has units of Watts per Kg”[23]. 2) the RF-energy-induced core-temperature increase, known as thermal effects.</p>
<p>Studies on non-ionizing fields have shown that there are short term thermal effects, however no long term effects such as sterility or cancer have been observed[21].</p>
<p>The concerns regarding thermal effects is mostly localized to parts of the body which have a relative lack of blood flow, such as the eyes. The lack of blood flow means that there is lower heat dissipation. It has been shown that short term exposure (up to an hour) to very high levels of radiation can cause cataracts in rabbits[23].</p>
<p>There is no convincing evidence that exposure to RF radiation shortens the lifespan of human beings or that it is a carcinogen. However, there is evidence that chronic exposure to RF radiation with SAR of about 2 to 3 W/kg resulted in cancer promotion in mice[23].</p>
</div>
<div title="Page 9">
<h2>Tags in Patients</h2>
<p>The U.S. Food and Drug Administration (FDA) raised issues that patients implanted with an RFID tag will make them incompatible to MRI[24]. In a study by James Lambert, it was found that the “device is safe inside a patient during MRI testing as far as device movement, heating, and image distortion [are concerned]. However, the device may fail due to the MRI exam.”</p>
<p>Also researchers have found[25, 26] that “high-frequency (HF) 13.56 MHz RFID tags do not sig- nificantly interfere with the functionality of imaging devices, nor do those devices affect the tags’ functionality.”</p>
<h1>References</h1>
<ol>
<li>Jerry L, Barbara C. Shrouds of Time: The history of RFID. AIM Publication;p. 11. Available from: https://www.aimglobal.org/estore/ProductDetails.aspx?ProductID=529.</li>
<li>net R. RFID Basics; 2011. Available from: http://rfid.net/basics.</li>
<li>Stockman H. Communication by Means of Reflected Power. Measurement. 1948;.</li>
<li>Uleotech. Electronic RFID tag and Peripherals;. Available from: http://www.uleotech.com/ partners/electronic-tag-maker/.</li>
<li>Tagsys. Tagsys RFID;. Available from: http://www.tagsysrfid.com/Products-Services/ RFID-Tags/Folio-370-LI-370SY-LI.</li>
<li>AIM. What is RFID?;. Available from: http://www.aimglobal.org/technologies/rfid/ what_is_rfid.asp.</li>
<li>Ahuja S, Potti P. An Introduction to RFID Technology. Communications and Network. 2010;02(03):183–186. Available from: http://www.scirp.org/journal/PaperDownload. aspx?DOI=10.4236/cn.2010.23026.</li>
<li>Finkenzeller K. RFID Handbook: Fundamentals and Applications in Contactless Smart Cards, Radio Frequency Identification and Near-Field Communication. 2010;Available from: http: //books.google.com/books?hl=en&amp;amp;lr=&amp;amp;id=gtAQm4DCbP0C&amp;amp;oi=fnd&amp;amp;pg= PR5&amp;amp;dq=RFID+Handbook:+Fundamentals+and+Applications+in+Contactless+Smart+ Cards&amp;amp;ots=1M-nhwCYZj&amp;amp;sig=HNRXwoFZADOoBnZ4S7B_utgfbNY.</li>
<li>Park CR, Lee SJ, Eom KH. The Design of RFID Conveyor Belt Gate Systems Using an Antenna Control Unit. Sensors. 2011 Sep;11(9):9033–9044. Available from: http://www. mdpi.com//1424-8220/11/9/9033/.</li>
<li>Sorrells P. Passive RFID Basics. Technology. 1998;.</li>
<li>Want R. An Introduction to RFID Technology. 2006;p. 25–33.</li>
<li>Weinstein R. RFID : A Technical Overview and Its Application to TECHNOLOGY. IT Professional. 2005;(June).</li>
<li>Piezoelectric. Piezoelectric materials; 2006. Available from: http://www.piezomaterials. com/index.htm.</li>
<li>David D. RFID on the Move; 2003.</li>
<li>Pan Q, Narayanan RM. Design of a Covert RFID Tag Network for Target Discovery and Target Information Routing. Sensors. 2011 Sep;11(10):9242–9259. Available from: http: //www.mdpi.com//1424-8220/11/10/9242/.</li>
<li>Wray BR. Automation in blood banking: RFID. MLO: medical laboratory observer. 2011 Oct;43(10):34. Available from: http://www.ncbi.nlm.nih.gov/pubmed/22029155.</li>
<li>TI. Animal ID Advances Livestock Health and Industry Economics;. Available from: http: //www.ti.com/rfid/shtml/apps-anim-tracking-id.shtml.</li>
<li>net R. Dallas Zoo Tracks Elephants Using CSL Real Time Lo- cation System; 2012. Available from: http://rfid.net/news/ 399-dallas-zoo-track-elephants-real-time-location-system.</li>
<li>Bustillo M. Wal-Mart Radio Tags to Track Clothing; 2010. Available from: http://online. wsj.com/article/SB10001424052748704421304575383213061198090.html.</li>
<li>Wolverton J. Wal-Mart to Embed RFID Tags in Clothing Beginning August 1;2010. Available from: http://thenewamerican.com/tech-mainmenu-30/computers/ 4157-wal-mart-to-embed-rfid-tags-in-clothing-beginning-august-1.</li>
<li>RFID4SME. Is RFID Safe at the workplace? 2006;p. 9. Available from: http: //www.rfid-in-action.eu/public/rfid-knowledge-platform/all-rfid-documents/ communication-strategies-to-inform-consumers-stakeholders/rfid4sme_ is-rfid-safe-at-the-workplace.</li>
<li>Nave C. Ionization Energies;. Available from: http://hyperphysics.phy-astr.gsu.edu/ hbase/chemical/ionize.html.</li>
<li>Hueter FG. Biological Effects of Radiofrequency Radiation. Health Effects Research Labora- tory; 1986.</li>
<li>Spychips.FDALETTERRAISESQUESTIONSABOUTVERICHIPSAFETY,DATASECU- RITY; 2004. Available from: http://www.spychips.com/press-releases/verichip-fda. html.</li>
<li>Swedberg C. Swiss Study Finds RFID Tags Safe for MRI, CT Scans; 2010. Available from: http://www.rfidjournal.com/article/view/7442.</li>
<li>Steffen T, Luechinger R, Wildermuth S, Kern C, Fretz C, Lange J, et al. Safety and relia- bility of radio frequency identification devices in magnetic resonance imaging and computed tomography. 2010;Available from: http://www.pssjournal.com/content/4/1/2.</li>
</ol>
</div>
</div>
