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

```bash
grep "^# " slides.md
```

---

![bg](./assets/dls.png)
# Introduction

---

### What is I15-1?

![bg right:25% w:500](./assets/beamline_layout.jpeg)

The **X-ray Pair Distribution Function (XPDF)** beamline

- High-energy beam: **40, 65, 76 keV** (λ = 0.31, 0.19, 0.16 Å)
- Total X-ray scattering: captures Bragg and diffuse scattering

---

### Sample Environments

![bg right:32%](./assets/sample_puck.jpg)

- Capillaries (spinning or static), flat plate geometry
- Robotic sample changer — 22-sample pucks, up to 440 positions
- Cryostream (80–500 K) · hot-air blower (RT-900°C)

---

### Sample Environments - Complex
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

### The Beamline Team
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

### The Crystallography Science Group

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

### The Review Panel

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

### Overall Assessment
- Leading international PDF facility
- Producing world-class science
- Strong publication output and citation impact
- Healthy user demand (~1.4× oversubscribed)
- Strong alignment with UK priorities in energy and materials research

---
### Strengths Highlighted
- High-throughput operation and mail-in access
- Robotic sample handling capability
- Wide range of in situ / operando environments
- Unique complementarity with ISIS neutron PDF measurements
- Innovative methods and instrumentation development

---

### Future Opportunities
- ARC detector programme identified as a key priority
- Hazardous gas capability would enable new science areas
- Increased automation of data reduction and analysis
- Continued growth of mail-in and remote access
- Further enhancement of user workflows and throughput

---

### Key Take-Home Message

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
### Motion/RIO Controllers

- Successfully completed a major modernisation of the I15/I15-1 controls infrastructure
- Increased reliability and operational independence of both beamlines

---

### New Chemistry Lab
- Recently extended and refurbished lab 83b
- Now have access to ducted fume hoods much closer to the beamline
![bg left:45% w:550](./assets/lab83.jpeg)

---

![bg right:40% w:400](./assets/trolley.jpg)
### New Gas Trolley
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

### A Two-pronged Attack
1. Slightly reduce the ambition of the ARC
2. Perfect the data acquisition and processing required using a commerical alternative

---

![bg vspace:1000](./assets/new_detexctors.jpg)

---

 &nbsp;| model | sensor <br>thickness | pixel<br>size | frame<br>rate |  coverage | width
:-----:|:------|:-----|:------|:------|:---|---
![h:150](./assets/arc.jpg)| ARC CdTe| 1000&nbsp;um | 55&nbsp;um | 25&nbsp;Hz | 109° or 18° | 42.2&nbsp;mm
![h:150](./assets/eiger.webp) | Eiger2 X CdTe | 750&nbsp;um | 75&nbsp;um | 4.5&nbsp;kHz | 17° | 38.4&nbsp;mm

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

![bg w:900](./assets/silicon_single_shot.png)

---

### Current Status: Eiger
- is in the hutch
- acquisition software is deployed
- installation on the endstation scheduled for August

---

### Current Status: ARClet
- new chassis is being designed, and we'll build multiple
- acquisition software is deployed
- installation on the endstation scheduled for September

---

![masked](./assets/s)
# Software

---

## Waffle
### Deploying the Diamond-II Software Stack on I15-1

- Internal project to run the Diamond-II software stack on I15-1 in production
- **Two goals**: prove the stack works on real experiments; improve the beamline for users now
- Current status: [components deployed / in testing / rolled out to users]
- What users will notice: [improved automation, data acquisition, GDA interface — fill in specifics]
- I15-1 as pathfinder — your feedback will shape the Diamond-II user experience across the facility

---

# Critical<br>Upgrades
![masked w:850](./assets/optics_hutch.jpeg)

---

crystal cage

---

front end components, primary slits

---

# User Access
![bg](./assets/dls.png)
Access no

---


## Access Through End of Diamond-I

- **AP41** — final standard proposal call, deadline **30 September 2026**
- [Any rapid-access, BAG, or commissioning time mechanisms still available]
- Advice: prioritise experiments that need Diamond-I capabilities or that underpin Diamond-II publications
- Contact: xpdf@diamond.ac.uk for scheduling questions
- [Any notes on restricted modes or reduced capacity in the run-up to shutdown]

---

## The Dark Period

- Facility shutdown for Diamond-II construction begins **[date]**
- Expected duration: **[timeline]**
- I15-1 during shutdown: [preserved in place / decommissioned / folded into Diamond-II scope]
- **I15-1 in Diamond-II**: [upgraded capabilities, name change, new energy range — whatever is settled]
- In the meantime: [other facilities, data analysis backlog, publication push]
- Stay informed: [mailing list, website, contact]

---

funding?


---




























---
![bg](./assets/dls.png)

## List of things
Normal markdown rules apply:

It helps us keep track of: 
- things
- other things
- those things over there
- and more! :o: :smiley: :white_check_mark:

---
- some things need a reference†
- and sometimes you need maths inline $x=y^2$ or in a block:
$$\begin{aligned}\mathbf{Q} &= \mathbf{k}_f - \mathbf{k}_i \\
Q &= \vert\mathbf{Q}\vert\end{aligned} $$

 <!-- _footer: †Keeble et. al Appl. Phys. Lett. 102, 092903 (2013) --> 

---

### and some things need to be in a table

Fruit | Colour | Amount | Cost
-----|------|:-----:|------:
Banana &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  | Yellow | 4 | £1.00
Apple | Red | 2 | £0.60
Orange | Orange &nbsp; &nbsp; &nbsp; | 10 | £2.50
Coconut | Brown | 1 | &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; £1.50

---

<style scoped>
  p { text-align: center; }
</style>
...and sometimes
you want to temporarily
modify something

---

![masked](./assets/i15-1.png)
sometimes it's fun to abuse css

---
 fitting long lines to page width
#### <!--fit--> https://www.diamond.ac.uk/Instruments/Crystallography/I19/Manual/EH1.html
