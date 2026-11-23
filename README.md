# Hi, I'm Franco 

**Telecommunications Engineering & Software Engineering student.** I work across both worlds: I build **business software (CRM / ERP / back-office systems)** that real companies use, and I design, measure and prototype **wireless and transmission systems (SDR, private cellular networks, PDH, antennas, GNSS)**.

---

## 💼 Featured: ElectroTotal — CRM / ERP platform *(private repo, in production)*

Full-stack operations platform I built for a real technical-services company. The source is private because it contains client and tax data, so here is what it does:

- **CRM & service management** – clients, accounts, branches, inspectors and technicians; services driven by a state-machine workflow, deliverables and photo evidence; AI-assisted quotes and reports.
- **Electronic invoicing (SUNAT, Peru)** – in-house engine for invoices and credit notes in UBL 2.1: XML-DSig signing, SOAP submission, CDR parsing and PDF generation.
- **ERP-style back office** – RBAC with 10 roles and area/global permissions, immutable audit log, soft delete, document management, payroll-oriented hour calculation.
- **Attendance with face recognition + GPS** – real camera and geolocation, embedding-based matching, deferred records with approval flow.
- **Local agent** (Node.js) that submits invoices to client portals that block server IPs.
- **Engineering practice** – 30 Prisma models, 11 migrations, Jest e2e/unit tests, Vitest + MSW frontend tests, spec-driven development.

`NestJS` `TypeScript` `Prisma` `PostgreSQL` `React 19` `Vite` `Mantine` `TanStack Query` `JWT` `Swagger` `UBL 2.1`

---

## 📡 Telecommunications & RF projects

### [Narrowcast-NB](https://github.com/franco0209/Narrowcast-NB) — Private NB-IoT cellular network, with an interactive lab
A private cellular network built from open-source software and low-cost hardware, with no operator involved: **ESP32 + NB-IoT module → USRP eNB (OpenAirInterface) → Open5GS 4G core → MQTT → web control panel**, all in Docker Compose. Real SIM authentication (Milenage), NAS security and IP assignment, plus a validated RF plan with transmission safety rules (off by default, authorised, gain- and time-limited, every session logged).
It also ships a **didactic laboratory that needs no radio**: a virtual irrigation node registers through the *real* OAI eNB into the *real* Open5GS core and sends MQTT through the actual GTP-U tunnel. You can open the UE, the RAN and the core, change the NB-IoT radio (band, PRB, NPRACH, paging) and see the modelled consequences: coverage level, repetitions, latency, energy.
`Open5GS` `OpenAirInterface` `srsRAN` `NB-IoT` `USRP` `Docker` `FastAPI` `React` `MQTT` `ESP32`

### [Radio Link Planner](https://github.com/franco0209/radio-link-planner) — Point-to-point radio link feasibility in the browser
Drop two sites on a map and get a plain-language verdict: **real terrain profile (Copernicus 90 m DEM), earth curvature, Fresnel zone, link budget and yearly availability**. If the link is blocked it computes how much taller the masts must be, or **proposes up to two repeater sites** and verifies each hop on the terrain. Everything runs client-side, the scenario lives in the URL, and the UI is in English, Spanish and Portuguese.
📡 **[Live demo](https://franco0209.github.io/radio-link-planner/)**
`TypeScript` `Leaflet` `Propagation modelling` `Vigants-Barnett` `GitHub Pages`

### [PDH Studio](https://github.com/franco0209/pdh-studio) — Bit-accurate PDH emulator in the browser *(latest)*
Emulates the **Plesiochronous Digital Hierarchy (E1 to E4)** bit by bit: G.711 PCM, the G.704 frame with CRC-4, AMI/HDB3 line codes, three levels of justification multiplexers with independent clocks, slips, alarms (LOS, LOF, AIS, RAI) and **G.826 error performance**. Every picture is drawn from the real bit streams, and any bit of an E4 can be traced back to its E1, time slot and sample. It bridges a radio hop to E1 quality and prices add/drop in PDH versus SDH on a network map of southern Peru. 78 automated tests; companion to Radio Link Planner.
📡 **[Live demo](https://franco0209.github.io/pdh-studio/)**
`TypeScript` `React` `Leaflet` `G.704` `G.742/G.751` `G.826` `Vitest`

### [Wireless Channel Characterizer — USRP N210](https://github.com/franco0209/CaracterizadorDeCanal_USRPN210)
Desktop app using two SDRs (one transmits, one captures I/Q) to measure **path loss (log-distance), LOS/NLOS obstruction effects, small-scale fading and multipath**. Includes a simulated channel so it runs without hardware.
`Python` `UHD` `SDR` `NumPy`

### [TwoMice-DGPS](https://github.com/franco0209/TwoMice-DGPS) — Antenna characterization & differential GPS
**VNA measurements** (S11, VSWR, impedance, resonance, −10 dB bandwidth) of the Mighty Mouse 3GPS active antenna, plus **differential positioning with two receivers** (CEP50/95, 2DRMS, baseline, block-bootstrap CIs). Analysis backend + dashboard, with tests.
`FastAPI` `React` `Plotly` `NumPy/SciPy` `NMEA` `Touchstone`

---

## 🧰 Skills

| Area | Technologies |
|---|---|
| **Software engineering** | TypeScript, NestJS, Node.js, Python (FastAPI), Java, C++, REST APIs, RBAC/JWT auth, testing (Jest, Vitest, pytest), spec-driven development |
| **Frontend** | React, Vite, Mantine, TanStack Query, Plotly, Leaflet |
| **Data & infra** | PostgreSQL, Prisma, MySQL, MongoDB, Docker / Compose, Git, Linux |
| **Business systems** | CRM, ERP, workflow/state machines, electronic invoicing (UBL 2.1), audit & permissions |
| **Telecom & RF** | SDR (USRP/UHD), OpenAirInterface, srsRAN, Open5GS, NB-IoT / LTE-M, PDH/E1 transmission (G.704, G.826), channel characterization, VNA/antenna measurement, GNSS/DGPS |
| **Embedded / IoT** | ESP32 (Arduino/PlatformIO), MQTT, AT-command modems |
| **Signal analysis** | NumPy, SciPy, pandas, Matplotlib |

---

## 📫 Let's talk
Open to internships and collaborations in **software engineering (CRM/ERP, full-stack)** and **telecom / RF / IoT**.

fcahua@unsa.edu.pe
