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

admin

---

schedule

---

contents probably

---

![bg](./assets/dls.png)
## Introduction

---

### What is I15-1?

![bg right:42%](./assets/beamline_layout.jpeg)

The **X-ray Pair Distribution Function (XPDF)** beamline

- High-energy beam: **40, 65, 76 keV** (λ = 0.31, 0.19, 0.16 Å)
- Wiggler source — high flux at hard X-ray energies
- Total X-ray scattering: captures Bragg **and** diffuse scattering
- PDF analysis reveals **local atomic structure** in crystalline, nanocrystalline, and amorphous materials
- Science areas: materials chemistry, battery research, pharmaceuticals, earth science, catalysis

---

### Supported Sample Environments

![bg right:32%](./assets/sample_puck.jpg)

**Standard:**
- Capillaries (spinning or static), flat plate geometry
- Robotic sample changer — 22-sample pucks, up to 96 positions

**Temperature:**
- Cryostream (80–500 K) · hot-air blower · resistance furnace (~1200°C)

**High pressure:**
- Diamond anvil cells (DAC) — multi-GPa range

**In-situ / reaction:**
- Electrochemical cells (battery cycling)
- Gas flow and reaction cells (catalysis, reaction following)

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
## SAC Review
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

![masked](./assets/i15-1.png)
## Upgrades, etc.

---

### Motion/RIO Controller Upgrade

- Successfully completed a major modernisation of the I15/I15-1 controls infrastructure.
- Replaced ageing hardware that had become increasingly difficult to maintain.
- Increased reliability and operational independence of both beamlines.
- Reduced technical risk and improved maintainability ahead of Diamond-II.
- Provided a flexible platform for future automation, instrumentation and scientific capability upgrades.


---

### New Chemistry Lab


---

## Wiggler Update

- [Status — e.g. scheduled maintenance, unplanned intervention, hardware upgrade]
- Changes to beam properties: [flux, energy range, stability]
- Impact on accessible science: [Q-range, sample size, throughput]
- Current status: [operational / in repair / upgraded and re-commissioned]

---

## ARC Detector
### Future Direction for XPDF Data Collection

- Custom CdTe photon-counting detector, purpose-built for I15-1
- **55 µm pixels** — 25 Hz continuous collection, 500 Hz burst mode
- Currently undergoing online commissioning
- What it enables: faster in-situ experiments, improved signal-to-noise, access to smaller samples
- Longer-term roadmap: [planned capability extensions, software integration milestones]

---

## Eiger Detector

- [Current Eiger model, any hardware or firmware updates]
- Continues to serve as the [primary / complementary] detector for [use cases]
- ARC and Eiger roles going forward: [complementary — Eiger for X, ARC for Y] or [transitional plan]
- [Anything users need to know about requesting one vs. the other]

---

## Waffle
### Deploying the Diamond-II Software Stack on I15-1

- Internal project to run the Diamond-II software stack on I15-1 in production
- **Two goals**: prove the stack works on real experiments; improve the beamline for users now
- Current status: [components deployed / in testing / rolled out to users]
- What users will notice: [improved automation, data acquisition, GDA interface — fill in specifics]
- I15-1 as pathfinder — your feedback will shape the Diamond-II user experience across the facility

---

## Critical Upgrades

| Upgrade | Status | User Impact |
|---------|--------|-------------|
| [Item 1] | Complete | [e.g. improved stability] |
| [Item 2] | In progress | [e.g. brief restricted access] |
| [Item 3] | Planned | [e.g. scheduled shutdown] |

- Priority work to ensure reliable operation through the end of Diamond-I
- [Note any scheduled shutdowns or periods of reduced capacity]

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
