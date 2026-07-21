---
marp: true
paginate: true
size: 16:9
backgroundImage: url('./assets/default.png')
style: |
  @import url('./assets/diamond.css');
  img[alt~='masked'] {
    mask-image: url('./assets/dls-mask.png');
    mask-repeat: no-repeat;
    mask-size: contain;
    mask-position: 100%, 0%;
    position: absolute;
    width: 1200px;

    /* Place to right-bottom */
    right: 0px;
    top: 0px;
    }

---
<!-- _class: lower-heading -->
![bg](./assets/h1.png)

# Beamline Update
Dean Keeble
I15-1 User Meeting, July 2026

---

**Introduction**
**Science Advisory Committee Review**
**Upgrades**
**Detectors**
**Software**
**Critical Upgrades**
**User Access & Diamond-II**

---

![bg](./assets/dls.png)
# Introduction

---

### What is I15-1?

![bg right:25% w:500](./assets/beamline_layout.jpeg)

The **X-ray Pair Distribution Function (XPDF)** beamline

- High-energy beam: **40, 65, 76 keV**<br>(λ = 0.31, 0.19, 0.16 Å)
- Total scattering: captures Bragg and diffuse scattering

---

### Sample environments

![bg right:32%](./assets/sample_puck.jpg)

- Capillaries (spinning or static), flat plate geometry
- Robotic sample changer — 22-sample pucks, up to 440 positions
- Cryostream (80–500 K) · hot-air blower (RT-900°C)

---

### Sample environments - complex
- Electrochemical cells (battery cycling)
- Gas flow and reaction cells (catalysis, reaction following)
- One-offs and user supplied equipment

---

<style scoped>
.team-grid { display: flex; gap: 20px; margin-top: 16px; justify-content: center; }
.team-item { flex: 1; max-width: 170px; text-align: center; }
.team-item img { width: 95px; height: 124px; object-fit: cover; border-radius: 6px; display: block; margin: 0 auto; }
.team-item .nophoto { width: 95px; height: 124px; background: #ccc; border-radius: 6px; margin: 0 auto; }
.team-name { font-size: 0.75em; font-weight: bold; margin-top: 7px; }
.team-role { font-size: 0.6em; color: #555; margin-top: 2px; line-height: 1.3; }
.tech { margin-top: 22px; font-size: 0.65em; color: #444; text-align: center; }
</style>

### The beamline team
Currently five full-time staff support operations on I15-1
<div class="team-grid">
  <div class="team-item">
    <img src="./assets/team_dean.png" alt="Dean Keeble">
    <div class="team-name">Dean Keeble</div>
    <div class="team-role">Principal Beamline Scientist</div>
  </div>
  <div class="team-item">
    <img src="./assets/team_dan.png" alt="Daniel Irving">
    <div class="team-name">Daniel Irving</div>
    <div class="team-role">Beamline Scientist</div>
  </div>
  <div class="team-item">
    <img src="./assets/team_anna.png" alt="Anna Herlihy">
    <div class="team-name">Anna Herlihy</div>
    <div class="team-role">Beamline Scientist</div>
  </div>
  <div class="team-item">
    <img src="./assets/team_tobie.png" alt="Tobias Bird"> 
    <div class="team-name">Tobias Bird</div>
    <div class="team-role">Post Doctoral Research Associate</div>
  </div>
  <div class="team-item">
    <img src="./assets/team_finley.jpeg" alt="Tobias Bird"> 
    <div class="team-name">Finley Belcher</div>
    <div class="team-role">Senior Beamline Technician</div>
  </div>
</div>

<div class="tech">
<strong>Technical & engineering:</strong> Stuart Gurney · Andrew Fairley · Peter Smith · Niamh Dougan · Dom Oram
</div>
<div class="tech">
<strong>PhD students:</strong> Niels Schreiner · Sophie Ray · Gayathri Manoj</div>

---

<style scoped>
.bl-grid { display: flex; gap: 20px; margin-top: 20px; }
.bl-item { flex: 1; text-align: center; }
.bl-item img { width: 100%; height: 170px; object-fit: cover; border-radius: 6px; }
.bl-id { font-size: 1.05em; font-weight: bold; margin-top: 10px; }
.bl-name { font-size: 0.68em; margin-top: 3px; color: #444; }
</style>

### The crystallography science group

**Group leader:** Philip Chater

<div class="bl-grid">
  <div class="bl-item">
    <img src="./assets/i11.jpg" alt="I11 hutch">
    <div class="bl-id">I11</div>
    <div class="bl-name">High Resolution Powder Diffraction</div>
  </div>
  <div class="bl-item">
    <img src="./assets/i15.jpg" alt="I15 extreme conditions">
    <div class="bl-id">I15</div>
    <div class="bl-name">Extreme Conditions</div>
  </div>
  <div class="bl-item current">
    <img src="./assets/i15-1_hutch.jpg" alt="I15-1 hutch">
    <div class="bl-id">I15-1</div>
    <div class="bl-name">XPDF</div>
  </div>
  <div class="bl-item">
    <img src="./assets/i19.jpeg" alt="I19">
    <div class="bl-id">I19</div>
    <div class="bl-name">Small Molecule Single Crystal</div>
  </div>
</div>

---
<style scoped>
  a{
  font-size: 1.0rem;
  }
</style>
## Diamond-II
![bg right:40% w:350](./assets/diamond-ii-tdr.png)
- Machine
- Beamlines
- Controls, Data & Computation
- Buildings & infrastructure 

https://www.diamond.ac.uk/Diamond-II.html

---
![](./assets/diamond-ii-timeline.png)

---

![masked](./assets/i15-1.png)
# SAC Review
10th-11th September 2025

---
<style scoped>
h2 { margin-bottom: 8px; }
.sac-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 14px 20px;
  margin-top: 10px;
}
.sac-person { text-align: center; }
.sac-person img, .sac-person .nophoto {
  width: 88px; height: 88px;
  border-radius: 50%;
  object-fit: cover;
  display: block;
  margin: 0 auto;
  border: 2px solid #e0e0e0;
}
.sac-person.chair img, .sac-person.chair .nophoto {
  border: 3px solid #0078A3;
  box-shadow: 0 0 0 3px rgba(0,120,163,0.15);
}
.nophoto { background: linear-gradient(135deg, #d0d0d0, #b8b8b8); }
.sac-name { font-size: 0.70em; font-weight: bold; margin-top: 7px; line-height: 1.2; }
.sac-affil { font-size: 0.56em; color: #666; margin-top: 3px; line-height: 1.3; }
.chair-label { font-size: 0.52em; color: #0078A3; font-style: italic; display: block; }
.sacmember-label { font-size: 0.52em; color: #0078A3; font-style: italic; display: block; }
</style>

### The review panel

<div class="sac-grid">
  <div class="sac-person chair">
    <img src="./assets/sac_pulham.jpeg" alt="Colin Pulham">
    <div class="sac-name">Colin Pulham<span class="chair-label">Chair</span></div>
    <div class="sac-affil">University of Edinburgh</div>
  </div>
  <div class="sac-person">
    <img src="./assets/sac_brewster.jpg" alt="Aaron Brewster">
    <div class="sac-name">Aaron Brewster</div>
    <div class="sac-affil">Lawrence Berkeley National Laboratory</div>
  </div>
  <div class="sac-person">
    <img src="./assets/sac_chapman.png" alt="Karena Chapman">
    <div class="sac-name">Karena Chapman</div>
    <div class="sac-affil">Stony Brook University</div>
  </div>
  <div class="sac-person">
    <img src="./assets/sac_dinnebier.jpeg" alt="Robert Dinnebier">
    <div class="sac-name">Robert Dinnebier</div>
    <div class="sac-affil">Max Planck Institute for Solid State Research</div>
  </div>
  <div class="sac-person">
    <img src="./assets/sac_hatcher.jpeg" alt="Lauren Hatcher">
    <div class="sac-name">Lauren Hatcher</div>
    <div class="sac-affil">Cardiff University</div>
  </div>
  <div class="sac-person">
    <img src="./assets/sac_levin.jpg" alt="Igor Levin">
    <div class="sac-name">Igor Levin</div>
    <div class="sac-affil">NIST</div>
  </div>
  <div class="sac-person">
    <img src="./assets/sac_rivers.jpg" alt="Mark Rivers">
    <div class="sac-name">Mark Rivers</div>
    <div class="sac-affil">Univ. of Chicago / Argonne</div>
  </div>
  <div class="sac-person">
    <img src="./assets/sac_robertson.jpeg" alt="Karen Robertson">
    <div class="sac-name">Karen Robertson</div>
    <div class="sac-affil">University of Nottingham</div>
  </div>
  <div class="sac-person">
    <img src="./assets/sac_rosseinsky.jpg" alt="Matt Rosseinsky">
    <div class="sac-name">Matt Rosseinsky<span class="sacmember-label">SAC rep.</span></div>
    <div class="sac-affil">University of Liverpool</div>
  </div>
</div>

---

### Overall assessment
- Leading international PDF facility
- Producing world-class science
- Strong publication output and citation impact
- Healthy user demand (~1.4× oversubscribed)
- Strong alignment with UK priorities in energy and materials research

---
### Strengths highlighted
- High-throughput operation and mail-in access
- Robotic sample handling capability
- Wide range of in situ / operando environments
- Unique complementarity with ISIS neutron PDF measurements
- Innovative methods and instrumentation development

---

### Future opportunities
- ARC detector programme identified as a key priority
- Hazardous gas capability would enable new science areas
- Increased automation of data reduction and analysis
- Continued growth of mail-in and remote access
- Further enhancement of user workflows and throughput

---

### Key take-home message

> _I15-1 has established itself as a leading facility for total scattering and PDF studies._

- World-leading science
- Strong user community
- Exciting developments underway
- Well positioned for future growth

---

![masked w:520](./assets/rio.jpeg)
# Upgrades

---
![bg right:30%](./assets/motion-rack.jpeg)
### Motion/RIO controllers

- Successfully completed a major modernisation of the I15/I15-1 controls infrastructure
- Increased reliability and operational independence of both beamlines

---

### New chemistry lab
- Recently extended and refurbished lab 83b
- Now have access to ducted fume hoods much closer to the beamline
![bg left:45% w:550](./assets/lab83.jpeg)

---

![bg right:40% w:400](./assets/trolley.jpg)
### New gas trolley
- We've built our own gas trolley
- Six MFCs and various mixing capabilities

---

### Wiggler(s) - new

![bg left:40%](./assets/wiggler_new.png)

- in late 2025 DLS took delivery of a spare wiggler
- It's has higher potential output so commissioning includes health physics etc.

---

### Wiggler(s) - current

- During the May shutdown a cooling water fault caused a pressure increase
- An incorrectly calibrated PRV caused a burst disk to rupture
- Identification of issue was stymied by mandatory 5-year electrical testing

![bg right:30% w:370](./assets/wiggler_failure.jpg)

---

### Wiggler(s) - current
>_As far as we can test before filling with LHe the wiggler looks fine._
![bg left:56%](./assets/wiggler_current.jpeg)

---

# Detectors
![masked w:550](./assets/arc_inside.jpeg)

---

<style scoped>
  h2, p, li { color: white !important;  }
</style>

![bg](./assets/varex.png)

## Varex (_née_ Perkin Elmer) Detectors
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :white_check_mark: big
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :white_check_mark: heavy
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :white_check_mark: cheap

---

![](./assets/detectors.jpeg)
 <!-- _footer: https://doi.org/10.1148/radiol.2018172656--> 

---
On the 10th July 2018 the CEO signed a PPF for an ambitious angularly-resolved CdTe (ARC) hybrid photon counting detector

![bg left](./assets/i15-1.png)

---

### ARC detector issues
![](./assets/arc_flat.png)

---

### A Two-pronged attack
1. Slightly reduce the ambition of the ARC in the short to medium term
2. Perfect the data acquisition and processing required using a commerical alternative

---

![bg vspace:1000](./assets/new_detexctors.jpg)

---

 &nbsp;| model | sensor <br>thickness | pixel<br>size | frame<br>rate |  coverage | width
:-----:|:------|:-----|:------|:------|:---|---
![h:150](./assets/eiger.webp) | Eiger2 X CdTe | 750&nbsp;um | 75&nbsp;um | 4.5&nbsp;kHz | 17° | 38.4&nbsp;mm
![h:150](./assets/arc.jpg)| ARC CdTe| 1000&nbsp;um | 55&nbsp;um | 25&nbsp;Hz | 109° or 18° | 42.2&nbsp;mm

---
<style scoped>
h3 {
    position: absolute;
    top: 60px;
    left: 75px;
    right: 75px;
  }
</style>
### Eiger simulations of scattering from LaB<sub>6</sub>

![bg h:500](./assets/lab6.png)

![bg h:450](./assets/eiger_coverage_76keV.png)

---

![bg left:60% w:900](./assets/silicon_single_shot.png)
_A Perkin Elmer Collection from 1mm silicon projected onto the Eiger_

---

<style scoped>
.eiger-photo {
  position: absolute;
  top: 48px; right: 60px;
  width: 255px; height: 255px;
  border-radius: 50%;
  overflow: hidden;
  border: 3px solid #e0e0e0;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}
.eiger-photo img { width: 100%; height: 100%; object-fit: cover; }
</style>

<div class="eiger-photo"><img src="./assets/eiger.jpeg" alt="Eiger detector"></div>

### Current status: Eiger
- is in the hutch
- acquisition software is deployed
- installation on the endstation scheduled for August

---

<style scoped>
.eiger-photo {
  position: absolute;
  top: 48px; right: 60px;
  width: 255px; height: 255px;
  border-radius: 50%;
  overflow: hidden;
  border: 3px solid #e0e0e0;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}
.eiger-photo img { width: 100%; height: 100%; object-fit: cover; }
</style>

<div class="eiger-photo"><img src="./assets/MiniARCbox.png" alt="ARC detector"></div>

### Current status: ARClet
- new chassis is being designed, and we'll build multiple
- acquisition software is deployed
- installation on the endstation scheduled for September

---

![masked w:600](./assets/code.png)
# Software

---

## Project Waffle
**Deploying the Diamond-II Software Stack on I15-1**
- Internal project to run the Diamond-II software stack on I15-1 in production
- **Two goals**: prove the stack works on real experiments; improve the beamline for users now

---

## Current Status

<style scoped>
.status-cards { display: flex; gap: 28px; margin-top: 28px; }
.card {
  flex: 1; text-align: center; padding: 28px 16px;
  background: rgba(0,120,163,0.07);
  border-radius: 14px; border: 1.5px solid rgba(0,120,163,0.25);
}
.card svg { width: 56px; height: 56px; display: block; margin: 0 auto 14px; }
.card-title { font-size: 0.88em; font-weight: bold; margin-bottom: 8px; }
.card-desc { font-size: 0.65em; color: #555; line-height: 1.5; }
</style>

<div class="status-cards">

  <div class="card">
    <svg viewBox="0 0 48 48" xmlns="http://www.w3.org/2000/svg">
      <circle cx="24" cy="24" r="6" fill="#0078A3"/>
      <circle cx="24" cy="24" r="13" fill="none" stroke="#0078A3" stroke-width="3" stroke-dasharray="5.5 3"/>
      <circle cx="24" cy="7"  r="3.5" fill="#0078A3"/>
      <circle cx="24" cy="41" r="3.5" fill="#0078A3"/>
      <circle cx="7"  cy="24" r="3.5" fill="#0078A3"/>
      <circle cx="41" cy="24" r="3.5" fill="#0078A3"/>
    </svg>
    <div class="card-title">Integrated Workflow</div>
    <div class="card-desc">Robot loads, sample alignment, and Eiger collections running entirely within the new framework</div>
  </div>

  <div class="card">
    <svg viewBox="0 0 48 48" xmlns="http://www.w3.org/2000/svg">
      <rect x="8"  y="10" width="32" height="5" rx="2.5" fill="#0078A3"/>
      <rect x="8"  y="21" width="32" height="5" rx="2.5" fill="#0078A3"/>
      <rect x="8"  y="32" width="20" height="5" rx="2.5" fill="#0078A3"/>
      <circle cx="38" cy="34.5" r="6" fill="none" stroke="#0078A3" stroke-width="3"/>
      <line x1="43" y1="40" x2="47" y2="44" stroke="#0078A3" stroke-width="3" stroke-linecap="round"/>
    </svg>
    <div class="card-title">Collection Queuing</div>
    <div class="card-desc">Swathes of planned collections can be queued and run autonomously</div>
  </div>

  <div class="card">
    <svg viewBox="0 0 48 48" xmlns="http://www.w3.org/2000/svg">
      <rect x="5" y="11" width="38" height="27" rx="3" fill="none" stroke="#0078A3" stroke-width="3"/>
      <polyline points="5,14 24,29 43,14" fill="none" stroke="#0078A3" stroke-width="3" stroke-linejoin="round" stroke-linecap="round"/>
    </svg>
    <div class="card-title">Mail-in Experiments</div>
    <div class="card-desc">First deployment target: fully automated mail-in experiment support</div>
  </div>

</div>

---

### What you will notice - web forms
![h:450](./assets/sample-service.png) ![h:450](./assets/experiment-planning.png)

---

### What you will notice - differently shaped data
- Eiger and/or ARClet data will look different to Perkin Elmer data
- We won't unilaterally choose to use the new detetcors until we're happy with the performance
---

![bg left:40% w:400](./assets/puck-box.jpg)
### What you will notice - sending pucks
We'll be starting to send pucks out for you to load the samples into in your home lab
_(we'll be starting with non-hazardous, local samples!)_

---

# Critical<br>Upgrades
![masked w:850](./assets/optics_hutch.jpeg)

---

## Crystal cage
![bg right:40% h:400](./assets/cage-overview.png)
- We're upgrading the core part of the monochromator
- Should yield better energy switching and reliability

---
## High heatload components
- Primary slits
- Side beam absorber
- Primary attenuator

---

# User Access<br>& Diamond-II
![bg](./assets/dls.png)

---


## Allocation Period 41

- **AP41** — final standard proposal call, deadline **30 September 2026**
- AP41 is planned to be longer than usual, but is already loaded with AP39 cancellations


---

## The Dark Period

- Facility shutdown for Diamond-II construction begins **December 2027**
- Expected duration: **~18 months**
- I15-1 during shutdown: data analysis, paper writing, replying to emails, secondments...

---
## I15-1 Timeline
<style scoped>
h2 { margin-bottom: 40px; }
.tl { margin: 0 10px; }
.tl-above { position: relative; height: 52px; }
.tl-pt { position: absolute; bottom: 0; transform: translateX(-50%); text-align: center; }
.tl-pt .pt-name { display: block; font-size: 0.62em; font-weight: bold; white-space: nowrap; line-height: 1.3; }
.tl-pt .pt-arr { display: block; font-size: 11px; }
.tl-axis { position: relative; height: 4px; background: #555; }
.tl-axis::after { content: ''; position: absolute; right: -12px; top: -5px; border-top: 7px solid transparent; border-bottom: 7px solid transparent; border-left: 12px solid #555; }
.tl-tick { position: absolute; top: -3px; width: 2px; height: 10px; background: #555; transform: translateX(-50%); }
.tl-rows { margin-top: 8px; }
.tl-row { position: relative; height: 27px; margin-bottom: 5px; }
.tl-bar { position: absolute; height: 27px; border-radius: 5px; }
.tl-bar-label-in { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); color: white; font-size: 0.7em; font-weight: bold; white-space: nowrap; pointer-events: none; }
.tl-bar-label-out { position: absolute; top: 50%; transform: translateY(-50%); font-size: 0.63em; font-weight: bold; white-space: nowrap; }
.tl-months { position: relative; height: 20px; margin-top: 6px; }
.tl-mo { position: absolute; transform: translateX(-50%); font-size: 0.54em; color: #999; white-space: nowrap; }
</style>

<div class="tl">
  <div class="tl-above">
    <div class="tl-pt" style="left:5%">
      <span class="pt-name" style="color:var(--diamond-primary)">User Meeting</span>
      <span class="pt-arr" style="color:var(--diamond-primary)">▼</span>
    </div>
    <div class="tl-pt" style="left:20%">
      <span class="pt-name" style="color:var(--diamond-alt-green)"><b>AP41 deadline</b><br><span style="font-weight:normal;font-size:0.9em">30 Sep 2026</span></span>
      <span class="pt-arr" style="color:var(--diamond-alt-green)">▼</span>
    </div>
  </div>
  <div class="tl-axis">
    <div class="tl-tick" style="left:5%"></div>
    <div class="tl-tick" style="left:15%"></div>
    <div class="tl-tick" style="left:25%"></div>
    <div class="tl-tick" style="left:35%"></div>
    <div class="tl-tick" style="left:45%"></div>
    <div class="tl-tick" style="left:55%"></div>
    <div class="tl-tick" style="left:65%"></div>
    <div class="tl-tick" style="left:75%"></div>
    <div class="tl-tick" style="left:85%"></div>
  </div>
  <div class="tl-rows">
    <div class="tl-row">
      <div class="tl-bar" style="left:10%;width:5%;background:var(--diamond-alt-orange)"></div>
      <span class="tl-bar-label-out" style="left:15.5%;color:var(--diamond-alt-orange)">Wiggler reinstallation</span>
    </div>
    <div class="tl-row">
      <div class="tl-bar" style="left:15%;width:5%;background:var(--diamond-alt-red)"></div>
      <span class="tl-bar-label-out" style="left:20.5%;color:var(--diamond-alt-red)">Eiger commissioning</span>
    </div>
    <div class="tl-row">
      <div class="tl-bar" style="left:20%;width:25%;background:var(--diamond-alt-cyan)"></div>
      <span class="tl-bar-label-in" style="left:32.5%">AP40</span>
    </div>
    <div class="tl-row">
      <div class="tl-bar" style="left:50%;width:40%;background:var(--diamond-alt-green)"></div>
      <span class="tl-bar-label-in" style="left:70%">AP41</span>
    </div>
    <div class="tl-row">
      <div class="tl-bar" style="left:28%;width:55%;background:var(--diamond-alt-violet)"></div>
      <span class="tl-bar-label-in" style="left:55.5%">Rapid Access</span>
    </div>
  </div>
  <div class="tl-months">
    <div class="tl-mo" style="left:5%">Jul '26</div>
    <div class="tl-mo" style="left:15%">Sep '26</div>
    <div class="tl-mo" style="left:25%">Nov '26</div>
    <div class="tl-mo" style="left:35%">Jan '27</div>
    <div class="tl-mo" style="left:45%">Mar '27</div>
    <div class="tl-mo" style="left:55%">May '27</div>
    <div class="tl-mo" style="left:65%">Jul '27</div>
    <div class="tl-mo" style="left:75%">Sep '27</div>
    <div class="tl-mo" style="left:85%">Nov '27</div>
  </div>
</div>






---
![bg](./assets/stfc.png)

---
> Overall, the multidisciplinary facilities budget will reduce by 15% over four years through making efficiency savings in how STFC operates the three major facilities on behalf of UKRI and deliberate choices to prioritise critical capability.

---

User Webinar on Wednesday 14 October 2026 at 13:00 (UTC)
![bg left ](./assets/diamond-user-webinar.png)

---

<style scoped>
.team-grid { display: flex; gap: 70px; margin-top: 16px; justify-content: center; }
.team-item { flex: 1; max-width: 270px; text-align: center; }
.team-item img { width: 125px; height: 164px; object-fit: cover; border-radius: 6px; display: block; margin: 0 auto; }
.team-item .nophoto { width: 95px; height: 124px; background: #ccc; border-radius: 6px; margin: 0 auto; }
.team-name { font-size: 0.75em; font-weight: bold; margin-top: 7px; }
.team-role { font-size: 0.6em; color: #555; margin-top: 2px; line-height: 1.3; }
</style>

- In the meantime, please reach out to the Diamond User Committee to find out how you can support and advocate for Diamond.
&nbsp;
<div class="team-grid">
  <div class="team-item">
    <img src="./assets/duc-luke-daniels.webp" alt="Luke Daniels">
    <div class="team-name">Luke Daniels</div>
    <div class="team-role">University of Liverpool</div>
    <div class="team-role">L.M.Daniels@liverpool.ac.uk</div>
  </div>
  <div class="team-item">
    <img src="./assets/duc_gary_nichol.jpeg" alt="Gary Nichol">
    <div class="team-name">Gary Nichol</div>
    <div class="team-role">University of Edinburgh</div>
    <div class="team-role">g.s.nichol@ed.ac.uk</div>
  </div>
</div>

---

<!-- _class: lower-heading -->
![bg](./assets/h3.png)

# Beamline Update
Dean Keeble
I15-1 User Meeting, July 2026