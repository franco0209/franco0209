# Hi, I'm Franco 

**Telecommunications Engineering & Software Engineering student.** I work across both worlds: I build **business software (CRM / ERP / back-office systems)** that real companies use, and I design, measure and prototype **wireless systems (SDR, private cellular networks, antennas, GNSS)**.

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

### [Narrowcast-NB](https://github.com/franco0209/Narrowcast-NB) — Private NB-IoT / LTE-M cellular network
End-to-end private network: **ESP32 + NB-IoT module → USRP eNB (OpenAirInterface) → Open5GS 4G core → MQTT → web control panel**, all in Docker Compose. Includes a validated RF plan with transmission safety rules, a virtual radio (srsRAN/ZMQ) to test without hardware, and PSM/eDRX power measurements.
`Open5GS` `OpenAirInterface` `srsRAN` `USRP` `Docker` `FastAPI` `MQTT` `ESP32`

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
| **Telecom & RF** | SDR (USRP/UHD), OpenAirInterface, srsRAN, Open5GS, NB-IoT / LTE-M, channel characterization, VNA/antenna measurement, GNSS/DGPS |
| **Embedded / IoT** | ESP32 (Arduino/PlatformIO), MQTT, AT-command modems |
| **Signal analysis** | NumPy, SciPy, pandas, Matplotlib |

---

## 📫 Let's talk
Open to internships and collaborations in **software engineering (CRM/ERP, full-stack)** and **telecom / RF / IoT**.
