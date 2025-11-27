# Synaptics.Systems — Cybersecurity Core Bundle

> **Modules included**
>
> - **Compliance Audit Core v2** (`ComplianceAuditCore.html`)
> - **Compliance Core Module** (`ComplianceCore.html`)
> - **AML / CTF Core Engine** (`AML_Core_Engine.html`)
> - **NDSP Genesis Core v3 ULTRA** (`NDSP_Genesis_Core.html`)
> - **Server Framework & Architecture** (`ServerFramework.html`)
> - **Quantum Anchor Image** (`Michael_Rybaltowicz_<[Quantum_anchor]>.jpg`)

This bundle is a **static, drop-in cybersecurity package** for businesses that want a **defensive-only** monitoring and compliance layer without complex backend setup.

Everything runs on the client in local mode by default. You can host this on **GitHub Pages, GoDaddy, Netlify, Vercel, or any static host**.

The new `index.html` file acts as the **Quantum Cybersecurity Stack Hub**, wiring every module together with shared navigation, a quantum anchor visual, and a live readiness probe so you can confirm each HTML surface is available before launching it.

---

## 1. Features Overview

### 1.1 Compliance Audit Core v2

Interactive console for running **local compliance / entropy audits** on logs, prompts, configs, or policies:

- Creates conceptual scores for:
  - **Overall Compliance Risk**
  - **Entropy Drift**
  - **String-Coherence**
  - **Continuity Score**
- Lets you tune:
  - Entropy sensitivity, continuity weight, jurisdiction, strictness, and depth of metadata anchoring.
- Enforces **defensive hard rules** such as “Disallow Organized Crime” and unsafe AI patterns. :contentReference[oaicite:0]{index=0}  
- Exports a **JSON audit file** locally for offline review. :contentReference[oaicite:1]{index=1}  

File: `ComplianceAuditCore.html`

---

### 1.2 Compliance Core Module

A small, **embeddable compliance lock status** component for any page:

- Shows **Regulation Lock**, **Data Boundary Lock**, **OpenAI Policy Lock**, and **Non-Intrusion Lock** as engaged. :contentReference[oaicite:2]{index=2}  
- Enforces:
  - Local-only mode (no backend unless you add one).
  - “No identity / biometrics inference.”
  - Non-medical / non-diagnostic outputs.
  - “Organized-Crime Use: Disallowed.” :contentReference[oaicite:3]{index=3}  
- Provides a local **audit log** you can export as JSON. :contentReference[oaicite:4]{index=4}  

File: `ComplianceCore.html`

---

### 1.3 AML / CTF Core Engine

A **front-end AML/CTF console** for user and transaction risk evaluation:

- User Risk Check:
  - KYC verified vs. not verified
  - PEP / sanctions matches
  - Geo risk + intent (login, deposit, withdrawal, transfer) :contentReference[oaicite:5]{index=5}  
- Transaction Risk Check:
  - Amount
  - Asset type (normal, unhosted wallet, privacy coin)
  - Velocity, structuring pattern, mixer exposure :contentReference[oaicite:6]{index=6}  
- Computes risk scores and dispositions (`PASS`, `REVIEW`, `BLOCK`) using a **RiskScorer** and **rules engine**, and stores results in hash-chained audit logs. :contentReference[oaicite:7]{index=7}  
- Includes:
  - **Authority Anchors** for multi-authority approval flows.
  - **Vessel Monitor** for ledger / API drift detection. :contentReference[oaicite:8]{index=8}  

File: `AML_Core_Engine.html`

---

### 1.4 NDSP Genesis Core v3 ULTRA

A **read-only entropy / telemetry console** anchored to your quantum anchor image:

- Visual “entropy index,” coherence, trend slope, anomalies, and rolling stats. :contentReference[oaicite:9]{index=9}  
- Telemetry channels (conceptual proxies): cognitive load, signal variance, circadian drift, system noise, environment flux. :contentReference[oaicite:10]{index=10}  
- Optional backend authority via `NDSP_BACKEND` constant; defaults to **LOCAL-AUTHORITY** with session-only persistence. :contentReference[oaicite:11]{index=11}  
- Uses `Michael_Rybaltowicz_<[Quantum_anchor]>.jpg` as the anchor visual. :contentReference[oaicite:12]{index=12}  

File: `NDSP_Genesis_Core.html`  
Image: `assets/Michael_Rybaltowicz_<[Quantum_anchor]>.jpg`

---

## 2. Repository Structure

Recommended layout for this bundle:

```text
synaptics-cybersecurity-core/
├─ README.md
├─ public/
│  ├─ index.html
│  ├─ ComplianceAuditCore.html
│  ├─ ComplianceCore.html
│  ├─ AML_Core_Engine.html
│  ├─ NDSP_Genesis_Core.html
│  └─ assets/
│     └─ Michael_Rybaltowicz_<[Quantum_anchor]>.jpg
└─ (optional) package.json
