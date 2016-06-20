---
layout: post
title: Laser Cooling by the Doppler effect
date: 2015-07-14 23:32:27
categories: Article
author: Kevin Psaila
---

The ability to cool and manipulate atoms using laser beams has allowed a relatively new, rapid expanding field to emerge. Current research focus primarily on how existing cooling techniques can be improved. The applications of cold atoms can vary from atomic clocks to studies of quantum degeneracy. This paper explains the basic mechanisms used in laser cooling and illustrates the development of the field by describing a selection of key experiments. 

## Introduction
By laser cooling, one can prepare a sample of atoms with an RMS velocity $$ < 1ms^{-1}$$ and with a temperature on the order of a few $$ 100\mu K$$. On absorbing and emitting light, an atom recoils since the photon imparts some momentum, albeit a tiny amount, to the atom. This causes the atom to be both accelerated and decelerated depending on whether it is moving towards or away from the light source. Doppler cooling involves light whose frequency is red-detuned to just below the resonance frequency of the atoms. Now, atoms moving towards the light are blue-shifted into resonance and are more likely to absorb the light whilst those moving away from the light are red-shifted further away from resonance and are less likely to absorb the light. The atoms absorb more photons if they move towards the light source due to the Doppler effect and hence this leads to preferential absorption towards the light source. As this is the direction of motion, the atoms are decelerated or slowed. Following absorption, atoms re-emit spontaneously and the recoil is in a random direction, however, on repeating this process many times, the mean velocity and thus the kinetic energy of the atom will be reduced. As a result atoms are slowed down and since temperature is the measure of random internal kinetic energy, the atoms are cooled.

## Deceleration and cooling of atomic beams
The cooling process of atoms in free space can be done in various ways including the cavity Doppler cooling method. This method could be done either with a single transverse mode or by using degenerate transverse modes. We will see, in some detail, how does the former method works.

###Cooling with a single transverse mode
Consider an atom of mass *m* with momentum *p*=*m*/*v* and kinetic energy $$ W=\textbf{p}^{2}/2m $$ that is illuminated by a plane electromagnetic wave of wave vector $$ \textbf{k}_{i}$$. In order for the coherent scattering peak to dominate the spectrum of scattered light, we assume that the light is detuned by more than one linewidth from any atomic transition and that its intensity is insufficient to saturate the transitions at the given detuning. Incident light falling on a fixed (in space) atom would be monochromatic scattered at the incident frequency, while for a free particle the recoil may be taken into consideration. By the conservation of momentum, in scattering, the atom would have a momentum equivalent to $$ \textbf{p'}=\textbf{p}+\hbar\textbf{k}_{i}-\hbar\textbf{k}_{s} $$ and a kinetic energy of $$ W'=W-\hbar\nabla$$ (1) where $$ \textbf{k}_{s} $$ is the photon's wave vector.

$$ \nabla=-(\textbf{k}_{i} - \textbf{k}_{s}) . \textbf{v} - \frac{\hbar(\textbf{k}_{i} - \textbf{k}_{s})^2}{2m}$$ (2)

By conservation of energy the frequency of the scattered photon is $$ ck_{s} = ck_{i} + \nabla$$ which is determined by the two-photon Doppler effect along the transferred momentum $$ \hbar(\textbf{k}_{i} - \textbf{k}_{s})^2$$. During scattering recoil takes place and results as heat, as shown in Eq. (2). If the scattered photon is blue detuned relative to the incident photon, the atom's kinetic energy is reduced. Conventional Doppler cooling fails to work for atoms with multilevel internal structure.

![Fig. 1: Schematic diagram of 2D or 3D cavity Doppler cooling using multiple beams and a single cavity. For 2D cooling a pair of counter propagating beams along the x axis and polarized along y is used, while for 3D cooling and added pair of beams are introduced propagating along +/- y and polarized along the x.]({{ site.baseurl }}/assets/laser.png)

Fig. 1: Schematic diagram of 2D or 3D cavity Doppler cooling using multiple beams and a single cavity. For 2D cooling a pair of counter propagating beams along the x axis and polarized along y is used, while for 3D cooling and added pair of beams are introduced propagating along +/- y and polarized along the x.

In contrast, cavity Doppler cooling relies on a negative two-photon Doppler effect $$ <(\textbf{k}_{i} - \textbf{k}_{s}).\textbf{v}>$$. This method depends on the frequency of the incident and scattered light, so internal structures can be cooled at a rate which is proportional to the coherent scattering rate. Since,in this method, the force is dissipated in the same direction as the transferred momentum, it is possible to conduct two-dimensional or three-dimensional cooling by the use of multiple incident beams and a single optical cavity as shown in Fig. 1 above. The force *f* due to coherent scattering is

$$\textbf{f} = \Gamma_{w}[ \hbar (\textbf{k}_{x}- \textbf{k}_{z}) L(\delta_{++})+ \hbar (\textbf{k}_{x}+ \textbf{k}_{z}) L(\delta_{+-})+ \hbar (-\textbf{k}_{x}- \textbf{k}_{z}) L(\delta_{-+})+ \hbar (-\textbf{k}_{x}+ \textbf{k}_{z}) L(\delta_{--})]$$ (3)

$$ \Gamma_{w}$$ is the rate of scattering, from one beam, of the cavity mode without the cavity enhancement and $$ L (\delta_{\pm \pm})$$ is the frequency-dependent intensity-enhancement factor of the cavity at the detuning of the scattered light. $$ \Gamma_{w}$$ can be found by decomposing the directional dependence of the strength of the waves from the source into Gaussian transverse modes.

The force due to scattering in the cavity is found by:

$$ \textbf{t}= \hbar(\textbf{k}_{x}-\textbf{k}_{z})\Gamma_{sc} \eta_{0}\frac{4\delta_{i}^{'} \gamma_{c}^{2} (\textbf{k}_{x}-\textbf{k}_{z}).\textbf{v}}{(\gamma_{c}^{2}+\delta_{+ +}^{2})(\gamma_{c}^{2}+\delta_{- -}^{2})} + \hbar(\textbf{k}_{x}+\textbf{k}_{z})\Gamma_{sc} \eta_{0}\frac{4\delta_{i}^{'}\gamma_{c}^{2}(\textbf{k}_{x}+\textbf{k}_{z}).\textbf{v}}{(\gamma_{c}^{2}+\delta_{+ -}^{2})(\gamma_{c}^{2}+\delta_{- +}^{2})}$$ (4)

Where $$ \Gamma_{sc}$$ is the free space scattering rate for a single incident beam and $$ \eta_{0}$$ is the ratio of power scattering into a single direction of the cavity to the power scattered into free space. The maximum scattering rate is achieved when the Doppler effect $$ (\pm\textbf{k}_{x}\mp\textbf{k}_{z}).\textbf{v}$$ is equal to $$ \delta_{i}^{'}$$, such that the denominator of equation (4) is reduced. The maximum force is achieved on the resonating scattering rate into the cavity which is represented by $$ \Gamma_{sc}\eta_{0}$$ at which the two-photon recoil momentum $$ \hbar (\textbf{k}_{x} \mp \textbf{k}_{z})$$ is transferred onto the atom. (Refer to Fig. 2)

![]({{site.baseurl }}/assets/graph.png)

Fig. 2: Cavity Doppler force along a diagonal direction as a function of Doppler effect. The detuning of the incident light relative to the cavity resonance is $$ \delta_{i}=-\gamma_{c}-2E_{rec}/\hbar$$ (solid line) and $$ \delta_{i}=-2\gamma_{c}-2E_{rec}/\hbar $$

## Doppler cooling limit
In laser cooling, when a photon is absorbed by the respective atom, with two red-detuned beams, it is expected to spontaneously emit a photon (in a random direction). Since these emissions are non-directional, over time the combined momentum averages out. The time taken for an atom to emit a photon depends on the natural line width, $$ \gamma$$, of the excited state of the atom and this factor sets the lower limit to the temperature of the atoms after cooling, which is:

$$ T_{Doppler}=\frac{h\gamma}{2k_{B}} $$

where $$ k_{B} $$ is the Boltzmann's constant and h is the Planck's constant.

Apart from the Doppler cooling limit there is also the recoil limit which is a fundamental limit of the atom. The recoil velocity an atom gains when it emits a single photon corresponds to a temperature termed the recoil limit.

To calculate the 3D cooling limit due to recoil heating in the setup with four incident beams along $$ \pm x$$ and $$ \pm y$$ we separate the heat due to scattering into free space and into the cavity mode. The scattering into free space is unaffected only if the cavity mode occupies a very small solid angle.

For a dipole pattern the average free space heating parallel to the dipole is $$ \frac{1}{5} E_{rec}$$ and that along the direction of the beam is $$ \frac{7}{5} E_{rec}$$. If the cavity line width $$ 2\gamma_{c} > \frac{E_{rec}}{\hbar}$$, the detuning that minimizes the temperature will be given by $$ \delta^{'}_{i}=-\gamma_{c}$$. Thus if the cooling rate is equal to the heating rate, the resulting kinetic temperature $$ T_{\alpha,min}$$ along direction $$ \alpha$$ is:

$$ k_{B}T_{\alpha,min}=\frac{\hbar \gamma_{c}}{2}(1+ \frac{C_{\alpha}}{\eta_{0}D_{\alpha}})$$
When the scattering rate into the resonator mode is bigger than the scattering rate into free space, the latter stops limiting the final temperature. Also, a large cavity linewidth leads to a large velocity capture range, while a narrow linewidth allows one to achieve a low final temperature.

The power coupling strength between atom and cavity is given by the intensity profile of the cavity mode. Therefore Eq. 4 remains valid for the position-dependent force if the cavity-to-free-space ratio $$ \eta_{0}$$ is replaced by its position dependent value:

$$ \eta(\rho,z)=\eta_{0}\frac{w_{0}^{2}}{w^{2}(z)}exp[-\frac{2\rho^{2}}{w^{2}(z)}]$$

where $$ w^{2}(z)=w^{2}_{0}[1+(\frac{z}{z_{R}})^2]$$ and $$ z_{R}=\frac{\pi w_{0}^{2}}{\lambda}$$ is the Rayleigh range of the cavity mode.

## Conclusion
Laser cooling has become a routine tool in many laboratories and especially in atomic and molecular physics. It is widely used for the investigation of cold quantum gases and trapping of atoms with optical fields. Laser cooling techniques also has applications for quantum information processing, for time and frequency standards and for highly accurate spectroscopy.

Apart from the laser cooling mechanism studied in this paper, there are more laser cooling mechanisms in which you can cool by laser polarisation gradients and work at low laser power. These are much more efficient than usual Doppler cooling, and they could be responsible for the low temperatures recently observed in 3D molasses, where polarisation gradients are certainly always present.


## Bibliography
1. A. E. Siegman, Lasers (University Science Books, Mill Valley, 1986).<br />
2. W.D. Phillips, Laser Cooling and Trapping of Neutral Atoms, Atomic physics Division,National Institute of Standards and Technology, 1992<br />
3. Vladan Vuletic, Hilton W. Chan, and Adam T. Black, Three-dimensional cavity Doppler cooling and cavity sideband cooling by coherent scattering, Department of Physics, Stanford University, Stanford, California, 2001<br />
4. Vladan Vuletic and Steven Chu, Laser Cooling of Atoms, Ions, or Molecules by Coherent Scattering, Department of Physics, Stanford University, Stanford, California, 1999<br />
5. J. Dalibard and C. Cohen-Tannoudji, Laser cooling below the Doppler limit by polarization gradients: simple theoretical models, Coll ́ege de France et Labo- ratoire de Spectroscopie Hertzienne de I’Ecole Normale Superieure, 1989<br />
6. Mendonca, J.T. : Tercas, H., Physics of Ultra-Cold Matter, Atomic Clouds, Bose-Einstein Condensates and Rydberg Plasmas, 2013<br />
7. E. S. Shuman1, J. F. Barry1 D. DeMille, Laser cooling of a diatomic molecule, 2010<br />
8. C.S. Adams and E. Riis, Laser coolond and trapping of neutral atoms, Department of Physics, Durham University, 1997<br />
9. <a href="http://www.artofproblemsolving.com/Wiki/index.php/LaTeX:Symbols" target="_blank">http://www.artofproblemsolving.com/Wiki/index.php/LaTeX:Symbols</a><br />
10. <a href="http://www.m2lasers.com/media/58086/laser-cooling.pdf" target="_blank">http://www.m2lasers.com/media/58086/laser-cooling.pdf</a><br />
11. <a href="http://www.quora.com/What-is-the-difference-between-the-Doppler-limit-and-the-Recoil-limit" target="_blank">http://www.quora.com/What-is-the-difference-between-the-Doppler-limit-and-the-Recoil-limit</a><br />
12. <a href="http://www.nobelprize.org/nobelprizes/physics/laureates/1997/press.html" target="_blank">http://www.nobelprize.org/nobelprizes/physics/laureates/1997/press.html</a>
