# Hola, soy Franco 👋

Estudiante de Ingeniería con enfoque en **telecomunicaciones y radiofrecuencia**, y desarrollador **full‑stack**. Me gusta unir las dos cosas: medir y caracterizar sistemas de radio, y construir el software que los opera y los visualiza.


---

## 🔭 Proyectos destacados

### 📡 [Narrowcast‑NB](https://github.com/franco0209/Narrowcast-NB) — Red celular privada NB‑IoT / LTE‑M
Red celular propia de extremo a extremo: **ESP32 + módulo NB‑IoT → eNB con USRP (OpenAirInterface) → núcleo 4G Open5GS → MQTT → panel web**. Todo en Docker Compose, con plan de RF validado y reglas de seguridad para emitir, radio virtual (srsRAN/ZMQ) para probar sin hardware y medición de consumo en PSM/eDRX.
`Open5GS` `OpenAirInterface` `srsRAN` `USRP` `Docker` `FastAPI` `MQTT` `ESP32`

### 🎛️ [Caracterizador de Canal Inalámbrico — USRP N210](https://github.com/franco0209/CaracterizadorDeCanal_USRPN210)
App de escritorio con dos SDR USRP N210 (uno transmite, otro captura I/Q) para medir **pérdida de propagación (log‑distancia), efecto de obstrucciones LOS/NLOS, desvanecimiento a pequeña escala y multitrayectoria**. Incluye canal simulado para usar la interfaz sin hardware.
`Python` `UHD` `SDR` `NumPy` `pywebview`

### 🛰️ [TwoMice‑DGPS](https://github.com/franco0209/TwoMice-DGPS) — Caracterización de antena GPS y DGPS
Medición con **VNA** (S11, VSWR, impedancia, resonancia y ancho de banda a −10 dB) de la antena activa del receptor Mighty Mouse 3GPS, y **posicionamiento diferencial con dos receptores** (CEP50/95, 2DRMS, línea base, IC95 por bootstrap de bloques). Backend de análisis + dashboard, con tests.
`FastAPI` `React` `Plotly` `NumPy/SciPy` `NMEA` `Touchstone (.s1p)`

### ⚡ Electro Total — sistema de gestión full‑stack *(repo privado, cliente real en producción)*
Plataforma de operación de una empresa de servicios técnicos: **API NestJS + Prisma + PostgreSQL** y **SPA React (PWA)**.
- **Facturación electrónica SUNAT** propia: facturas y notas de crédito UBL 2.1, firma XMLDSig, envío SOAP y parseo del CDR, PDF de factura.
- **Asistencia con reconocimiento facial y GPS reales** (embeddings + similitud coseno), registros diferidos con aprobación y cálculo de horas.
- **CRM y servicios** con workflow de estados (FSM), entregables y evidencias fotográficas; generación de cotizaciones/informes asistida por IA.
- **RBAC data‑driven** (10 roles, permisos por área/global), JWT con refresh tokens rotados y detección de reuso, auditoría inmutable, soft delete.
- **Agente local** en Node para enviar facturas a portales que bloquean IPs de servidor.
- 30 modelos Prisma, 11 migraciones, tests unitarios/e2e (Jest) y de frontend (Vitest + MSW), specs por feature.
`NestJS` `TypeScript` `Prisma` `PostgreSQL` `React 19` `Vite` `Mantine` `TanStack Query` `SUNAT/UBL 2.1`

---

## 🧰 Stack

| Área | Tecnologías |
|---|---|
| Radio / Telecom | USRP (UHD), OpenAirInterface, srsRAN, Open5GS, NB‑IoT/LTE‑M, VNA, GNSS/NMEA |
| Backend | NestJS, Node.js, Prisma, PostgreSQL, Python (FastAPI), MongoDB |
| Frontend | React, TypeScript, Vite, Mantine, Plotly |
| Embebido | ESP32 (Arduino/PlatformIO), MQTT |
| DevOps | Docker / Compose, Git, Linux |
| Análisis | NumPy, SciPy, pandas, Matplotlib, Plotly |

---

## 📫 Contacto
Abierto a colaborar en proyectos de **SDR, redes celulares privadas/IoT, caracterización RF y desarrollo full‑stack**. Escríbeme por GitHub.
