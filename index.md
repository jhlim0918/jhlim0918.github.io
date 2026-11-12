---
layout: default
---

# About

<p class="lead">I am a Nevada Center for Astrophysics Postdoctoral Fellow at the University of Nevada, Las Vegas. I am a theorist who runs large 3D simulations to find out how planetesimals, planets and brown dwarfs form in the disks of gas and dust around young stars.</p>

I completed my Ph.D. in astrophysics at Iowa State University in 2026, advised by [Prof. Jacob B. Simon](https://www.jbsimon.com/home), with support from a NASA FINESST fellowship. Before that, I earned my B.S. and M.S. in astronomy at Chungnam National University in Daejeon, South Korea, where I grew up and where my M.S. work with Prof. Jungyeon Cho was on compressible and magnetized turbulence.

<ul class="chips">
  <li>Planet formation</li>
  <li>Protoplanetary disks</li>
  <li>Streaming instability</li>
  <li>Gravitational instability</li>
  <li>(Magneto)hydrodynamic turbulence</li>
  <li>GPU and high-performance computing</li>
</ul>


# The big picture

Every planetary system, including our own, began as a disk of gas and dust around a young star. Building a planet from that dust means growing by more than ten orders of magnitude in size, from micron-sized grains to bodies thousands of kilometers across. Two steps along the way remain poorly understood.

The first is the **planetesimal barrier**. Dust sticks into millimeter- to centimeter-sized pebbles, but beyond that size collisions tend to bounce or shatter grains, and gas drag makes pebbles drift into the star faster than they can grow. Something must gather pebbles into dense clouds that collapse under their own gravity into the 1–100 km planetesimals that seed planets. The leading candidate is the **streaming instability**, in which the drag between dust and gas makes dust pile up spontaneously into dense filaments.

The second is what happens in the **youngest, most massive disks**. When a disk is massive enough, its own gravity can make it break up into bound clumps. This **gravitational instability** may form giant planets and brown dwarfs on wide orbits directly, and its spiral arms may also trap dust and let it grow early.

My work connects these processes to what we can measure: images of young disks from ALMA, the planetesimals preserved in our own Kuiper Belt, and the spins of planetary and brown-dwarf companions.

<div class="questions">
  <div class="question">
    <div class="q-num">Question 1</div>
    <div class="q-text">Where and when can the streaming instability form planetesimals?</div>
    <p>How the answer depends on grain size, dust abundance and turbulence.</p>
  </div>
  <div class="question obs">
    <div class="q-num">Question 2</div>
    <div class="q-text">What observable signatures does dust–gas dynamics leave?</div>
    <p>Polarization, optical depth and disk dust masses, planetesimal properties.</p>
  </div>
  <div class="question gi">
    <div class="q-num">Question 3</div>
    <div class="q-text">What forms when young, massive disks fragment?</div>
    <p>The masses and spins of the fragments, and how dust grows in their spiral arms.</p>
  </div>
</div>

<figure>
  <div class="figure-scroll">{% include big_picture.svg %}</div>
  <figcaption>Two routes to planetary bodies and the observations that test them. My published work (teal) asks when the streaming instability can overcome the growth barrier; my current work at UNLV (amber) follows gravitationally unstable young disks.</figcaption>
</figure>


# Research

## Conditions for planetesimal formation by the streaming instability <span class="status published">Published</span>

<div class="research-item">
<div markdown="1">

The streaming instability can only form planetesimals if it concentrates dust strongly enough for self-gravity to take over ("strong clumping"). Whether it does depends on the size of the grains, how much dust there is relative to gas, and how turbulent the disk is. In a series of 3D simulations I mapped these conditions across a wide range of disk environments: in [turbulent disks](https://doi.org/10.3847/1538-4357/ad47a2) (Lim et al. 2024), for [small grains and low dust abundance](https://doi.org/10.3847/1538-4357/adb311) (Lim et al. 2025), and in [laminar disks](https://doi.org/10.3847/1538-4357/ae47e9) (Lim et al. 2026).

The figure summarizes the resulting criteria. In laminar disks, filled points mark simulations that formed planetesimals; in turbulent disks, planetesimals form above the line for each turbulence strength α. The dust abundance needed rises steeply for the smallest grains and as turbulence gets stronger.

</div>
<figure>
  <img src="{{ '/assets/images/all_Zcrit_web.png' | relative_url }}" alt="Critical dust-to-gas ratio for strong clumping versus grain Stokes number, for laminar and turbulent disks" loading="lazy">
  <figcaption>Dust abundance needed for planetesimal formation (dust-to-gas column density ratio Z) versus grain size (dimensionless stopping time τ<sub>s</sub>), for laminar (points) and turbulent (lines) disks.</figcaption>
</figure>
</div>


## Streaming-instability dynamics in unstratified and stratified disks <span class="status published">Published</span>

<div class="research-item narrow-fig">
<div markdown="1">

Besides forming planetesimals, the streaming instability drives the coupled motion of dust and gas near the disk midplane. Much of what we know comes from "unstratified" simulations that leave out the star's vertical gravity, which are cheaper and can be run at higher resolution. In [Lim et al. (2025)](https://doi.org/10.3847/1538-4357/ae01a6) I compared unstratified and vertically stratified simulations systematically across a range of radial pressure gradients.

Within the parameters explored, the instability behaves in the same way in unstratified disks and in the midplane of stratified disks: both form comparable dust filaments, with the stratified runs more confined vertically. This justifies using high-resolution local models of the midplane to predict observables.

</div>
<figure>
  <img src="{{ '/assets/images/unstrat_strat_rhop_web.png' | relative_url }}" alt="Dust density in unstratified (top) and stratified (bottom) streaming-instability simulations" loading="lazy">
  <figcaption>Dust density in unstratified (top) and stratified (bottom) simulations.</figcaption>
</figure>
</div>


## Gravitational instability: fragment masses and spins <span class="status ongoing">In progress</span>

At UNLV I am studying how massive young disks fragment, using local 3D simulations with self-gravity, magnetic fields (including ambipolar diffusion) and adaptive mesh refinement that follow the clumps as they collapse. The goal is to measure the masses and spins of the fragments and how magnetic fields and cooling change them.

## Dust growth in self-gravitating disks <span class="status ongoing">In progress</span>

The spiral arms of a gravitationally unstable disk are pressure maxima that can trap dust. I am adding dust particles, their growth and their self-gravity to these simulations to ask how large grains can grow in the arms, and whether the dust can collapse into planetary embryos while the disk is still young and massive.


# Publications

Full and up-to-date lists are on [SciX]({{ site.scix }}) and [Google Scholar]({{ site.google_scholar }}).

### First-author papers

<ol class="pubs">
  <li><span class="ptitle">The Streaming Instability in 3D: Conditions for Strong Clumping</span><br>
    <strong>J. Lim</strong>, J. B. Simon, R. Li, O. Brouillette, D. G. Rea, W. Lyra &middot; <span class="venue">ApJ 1000, 156 (2026)</span><br>
    <span class="plinks"><a href="https://doi.org/10.3847/1538-4357/ae47e9">Journal</a><a href="https://arxiv.org/abs/2509.18270">arXiv</a></span></li>
  <li><span class="ptitle">Bridging Unstratified and Stratified Simulations of the Streaming Instability for τ<sub>s</sub> = 0.1 Grains</span><br>
    <strong>J. Lim</strong>, S. A. Baronett, J. B. Simon, C.-C. Yang, D. Sengupta, O. M. Umurhan, W. Lyra &middot; <span class="venue">ApJ 993, 12 (2025)</span><br>
    <span class="plinks"><a href="https://doi.org/10.3847/1538-4357/ae01a6">Journal</a></span></li>
  <li><span class="ptitle">Probing Conditions for Strong Clumping by the Streaming Instability: Small Dust Grains and Low Dust-to-gas Density Ratio</span><br>
    <strong>J. Lim</strong>, J. B. Simon, R. Li, D. Carrera, S. A. Baronett, A. N. Youdin, W. Lyra, C.-C. Yang &middot; <span class="venue">ApJ 981, 160 (2025)</span><br>
    <span class="plinks"><a href="https://doi.org/10.3847/1538-4357/adb311">Journal</a></span></li>
  <li><span class="ptitle">Streaming Instability and Turbulence: Conditions for Planetesimal Formation</span><br>
    <strong>J. Lim</strong>, J. B. Simon, R. Li, P. J. Armitage, D. Carrera, W. Lyra, D. G. Rea, C.-C. Yang, A. N. Youdin &middot; <span class="venue">ApJ 969, 130 (2024)</span><br>
    <span class="plinks"><a href="https://doi.org/10.3847/1538-4357/ad47a2">Journal</a></span></li>
  <li><span class="ptitle">Decay of Turbulence in Fluids with Polytropic Equations of State</span><br>
    <strong>J. Lim</strong>, J. Cho &middot; <span class="venue">JKAS 53, 49 (2020)</span><br>
    <span class="plinks"><a href="https://doi.org/10.5303/JKAS.2020.53.2.49">Journal</a></span></li>
  <li><span class="ptitle">Generation of Solenoidal Modes and Magnetic Fields in Turbulence Driven by Compressive Driving</span><br>
    <strong>J. Lim</strong>, J. Cho, H. Yoon &middot; <span class="venue">ApJ 893, 75 (2020)</span><br>
    <span class="plinks"><a href="https://doi.org/10.3847/1538-4357/ab8066">Journal</a></span></li>
</ol>

### Co-authored papers

<ol class="pubs">
  <li><span class="ptitle">Closing the Gap: A Test of the Streaming Instability Using Simulations and Observations of the Cold-Classical Kuiper Belt Size Distribution</span><br>
    W. Hall, J. B. Simon, <strong>J. Lim</strong>, D. Carrera, M. Small &middot; <span class="venue">arXiv:2610.04114 (2026)</span><br>
    <span class="plinks"><a href="https://arxiv.org/abs/2610.04114">arXiv</a></span></li>
  <li><span class="ptitle">A Comparison between Particle and Fluid Approaches for Streaming Instability in Global Patch Simulations</span><br>
    D. Hetzel Ostertag, M. Flock, P. Rosendahl, A. Mignone, <strong>J. Lim</strong>, J. B. Simon &middot; <span class="venue">arXiv:2610.09575 (2026)</span><br>
    <span class="plinks"><a href="https://arxiv.org/abs/2610.09575">arXiv</a></span></li>
  <li><span class="ptitle">Revisiting Planetesimal Formation from mm-sized Grains in Pressure Bumps</span><br>
    T. S. Tanvir, J. B. Simon, D. Carrera, <strong>J. Lim</strong> &middot; <span class="venue">arXiv:2609.27025 (2026)</span><br>
    <span class="plinks"><a href="https://arxiv.org/abs/2609.27025">arXiv</a></span></li>
  <li><span class="ptitle">Azimuthal Dust Polarization from Aerodynamically Aligned Grains as Evidence for the Streaming Instability in Protoplanetary Disks</span><br>
    Z.-Y. D. Lin, <strong>J. Lim</strong>, J. B. Simon, Z.-Y. Li, et al. &middot; <span class="venue">ApJ 1006, 95 (2026)</span><br>
    <span class="plinks"><a href="https://doi.org/10.3847/1538-4357/ae8445">Journal</a></span></li>
  <li><span class="ptitle">A Comparative Study of the Streaming Instability: Unstratified Models with Marginally Coupled Grains</span><br>
    S. A. Baronett, W. Lyra, et al. (incl. <strong>J. Lim</strong>) &middot; <span class="venue">arXiv:2603.04558 (2026)</span><br>
    <span class="plinks"><a href="https://arxiv.org/abs/2603.04558">arXiv</a></span></li>
  <li><span class="ptitle">On the Mass Budget Problem of Protoplanetary Disks: Streaming Instability and Optically Thick Emission</span><br>
    D. Godines, W. Lyra, L. Ricci, C.-C. Yang, J. B. Simon, <strong>J. Lim</strong>, D. Carrera &middot; <span class="venue">ApJ 997, 192 (2026)</span><br>
    <span class="plinks"><a href="https://doi.org/10.3847/1538-4357/ae1f15">Journal</a></span></li>
  <li><span class="ptitle">Positive Feedback II: How Dust Coagulation inside Vortices Can Form Planetesimals at Low Metallicity</span><br>
    D. Carrera, L. E. J. Eriksson, <strong>J. Lim</strong>, W. Lyra, J. B. Simon &middot; <span class="venue">A&amp;A 701, L1 (2025)</span><br>
    <span class="plinks"><a href="https://doi.org/10.1051/0004-6361/202555045">Journal</a></span></li>
  <li><span class="ptitle">Positive Feedback: How a Synergy between the Streaming Instability and Dust Coagulation Forms Planetesimals</span><br>
    D. Carrera, <strong>J. Lim</strong>, L. E. J. Eriksson, W. Lyra, J. B. Simon &middot; <span class="venue">A&amp;A 696, L23 (2025)</span><br>
    <span class="plinks"><a href="https://doi.org/10.1051/0004-6361/202554100">Journal</a></span></li>
</ol>


# Talks

<ul class="tl">
  <li><span class="when">Jun 2026</span><span>3rd PFITS+ Meeting on Hydrodynamics of Circumstellar Disks and Planet Formation, SETI Institute, CA</span></li>
  <li><span class="when">Jan 2026</span><span>Dissertation talk, 247th Meeting of the American Astronomical Society, Phoenix, AZ</span></li>
  <li><span class="when">Sep 2025</span><span>Star and Planet Formation Group, University of Nevada, Las Vegas</span></li>
  <li><span class="when">Nov 2023</span><span>TCAN Disk Hydro &amp; Planet Formation, University of Arizona, Tucson, AZ</span></li>
  <li><span class="when">Feb 2020</span><span>Magnetic Fields in the Universe 7, Quy Nhon, Vietnam</span></li>
  <li><span class="when">Oct 2019</span><span>Korean Astronomical Society Meeting, Seoul, South Korea</span></li>
</ul>


# Teaching, mentoring and service

<ul class="tl">
  <li><span class="when">2027</span><span><strong>Organizing:</strong> one of the main organizers, <a href="https://jasonhsteffen.github.io/exsocal2027/">ExSoCal 2027</a></span></li>
  <li><span class="when">Fall 2026</span><span><strong>Teaching (UNLV):</strong> guest lecturer, AST 713: Astrophysics I (graduate level); two lectures on exoplanet detection (radial velocity, transits, direct imaging and gravitational microlensing)</span></li>
  <li><span class="when">2026–present</span><span><strong>Mentoring:</strong> Karol Nowohoński (master's student at ETH Zurich): self-gravitating dust in disks with the magnetorotational instability</span></li>
  <li><span class="when">2026–present</span><span><strong>Mentoring:</strong> Aydean Bejtovic (undergraduate at Iowa State): extending 3D streaming-instability simulations to different radial pressure gradients</span></li>
  <li><span class="when">2026–present</span><span><strong>Organizing:</strong> weekly meetings of the <a href="https://unlv-spfg.github.io/">UNLV Star and Planet Formation Group</a></span></li>
  <li><span class="when">2025</span><span><strong>Review:</strong> external reviewer for NASA's Solar System Workings program</span></li>
  <li><span class="when">2022–2024</span><span><strong>Mentoring:</strong> Olivia Brouillette (undergraduate researcher at Iowa State, now a graduate student at New Mexico State University; co-author of Lim et al. 2026)</span></li>
  <li><span class="when">2020–2024</span><span><strong>Teaching (Iowa State):</strong> General Physics II; Stars, Galaxies, and Cosmology; Physics for the Life Sciences; General Physics lab</span></li>
  <li><span class="when">2022–2023</span><span><strong>Preparing Future Faculty Associate</strong>, Iowa State University</span></li>
  <li><span class="when">2019</span><span><strong>Teaching (Chungnam National University):</strong> Galactic Astronomy</span></li>
  <li><span class="when">2018</span><span><strong>Organizing:</strong> LOC member, 8th East-Asia School and Workshop on Laboratory, Space, and Astrophysical Plasmas</span></li>
</ul>
