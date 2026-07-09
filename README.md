<div align="center">

# Shengwei Liu

**Cloud Security Architect · Zero-Trust Builder · AI + IoT Full-Stack Engineer**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shengwei--liu-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/shengwei-liu)
[![Location](https://img.shields.io/badge/📍-Singapore-blue?style=flat-square)]()
[![Email](https://img.shields.io/badge/📧-lsw19920322@gmail.com-red?style=flat-square)](mailto:lsw19920322@gmail.com)

**[🇨🇳 中文版](./PROFILE_README_zh.md)**

</div>

---

### 👤 About Me

A **Cloud Security Architect** with 10+ years of full-stack engineering experience. From Fortune 500 delivery leadership at Accenture to industrial MES systems at Scania, my core strength is **turning security architectures from slides into working systems** — not just drawing Hub-Spoke topology diagrams, but writing the Bicep templates, configuring Private Endpoints, and running Shadow E2E tests to prove the network is actually isolated.

Currently holding 5 Microsoft Certifications (including **AZ-305 Solutions Architect Expert** and **SC-300 Identity & Access Security**), building **Project-OmniGuard** — an enterprise-grade cloud-edge security platform deployed on Azure Singapore.

---

### 🏅 Microsoft Certifications

<div align="center">

| Cert | Title | Domain |
|:---:|:---|:---|
| **AZ-305** | Azure Solutions Architect Expert | ☁️ Cloud Architecture |
| **AZ-104** | Azure Administrator Associate | ☁️ Cloud Operations |
| **AI-102** | Azure AI Engineer Associate | 🤖 AI Engineering |
| **SC-300** | Identity and Access Administrator | 🔐 **Security & Identity** |
| **AB-100** | Agentic AI Business Architect | 🤖 AI Strategy |

</div>

---

### 🛡️ Flagship Project: OmniGuard

<table>
<tr>
<td width="140" align="center">
<img src="https://img.shields.io/badge/🛡️-OmniGuard-0078D4?style=for-the-badge" />
</td>
<td>

**[Project-OmniGuard](https://github.com/swliu920322/Project-OmniGuard)** — Cloud-Edge Collaborative Security Orchestrator · Zero-Trust Sandbox · 6,300+ Lines of Production Code

An enterprise-grade security platform I designed and built from scratch, deployed on Azure Singapore. Not a demo — a fully functional end-to-end system.

</td>
</tr>
</table>

#### What I Actually Built:

**🔐 Security Layer — Not Diagrams, Verified Zero-Trust**

- Hand-built **Hub-Spoke VNet topology** with 4 Private Endpoints (Cosmos DB / Key Vault / Storage / OpenAI). Backend completely invisible from public internet (`external: false`)
- Hand-crafted **HMAC-SHA256 SAS Token signing** (not a one-line SDK call — built with `hmac` + `hashlib` from protocol level) for IoT Hub C2D message authentication
- Wrote a **287-line self-healing Shadow E2E test**: provisions a shadow resource group → verifies Private DNS A records point to `10.1.2.x` subnet → auto-destroys. Even Ctrl+C won't leak resources
- **Bidirectional NSG micro-segmentation**: Deny Internet Inbound + Allow Backend Only to Storage Subnet

**🤖 AI Safety Layer — Multi-Agent Orchestration with Physical Circuit-Breaking**

- 3-Agent pipeline (Router → Safety Firewall → Action Compiler) with **2 early short-circuit points**:
  - `SENSOR_ERROR` → immediate STOP, no downstream Agent token waste
  - Safety Agent returns `BLOCK` → override, action never reaches physical actuators
- Engineering validation of the Kinematic-Token Theorem: frontend physics simulation proves AGVs cannot brake before collision at 2600ms cloud latency — 15ms edge braking is required

**⚡ Edge Computing Layer — LLMs Running Inside the Browser**

- **WebGPU** boots Qwen2.5-0.5B + MiniLM-L6-v2 directly in the browser at $0.00 server compute cost
- Cosine similarity semantic router (threshold ≥ 0.72) — if it can be answered locally, it never hits the cloud

**🏗️ Infrastructure Layer — Full IaC + Automation Pipeline**

- 3-layer modular Bicep (main → nested-infra → compute-module), supporting `sandbox` / `secure-iot` scenario switching
- Visual IaC Configurator: configure VNet CIDR, SKUs, Managed Identity in the browser, export deployable `.zip` packages
- Bicep preflight compilation + Azure `az deployment sub validate` pre-flight validation
- **33 Architecture Decision Records** — documenting not just what was built, but why

**📊 Project Metrics**

| Metric | Value |
|:-----|:-----|
| Total Codebase | **6,300+ lines** (Frontend 3,500 + Backend 800 + IaC 560 + Automation 1,200) |
| ADR Documents | **33** (Infra 8 / Backend 6 / Frontend 13 / Architecture 10) |
| E2E Test Suite | 287 lines (self-healing, validates Private DNS + ACA health) |
| IoT Full-Duplex | Event Hub Trigger ↔ C2D Messages (HMAC-SHA256 SAS hand-signed) |

---

### 💼 Engineering Track Record

| Period | Company | Role | What I Did |
|:-------|:--------|:-----|:-----------|
| 2025–Present | Independent | **Lead Architect** | OmniGuard: Zero-Trust infra + Multi-Agent AI safety + IoT device security |
| 2023–2024 | **Scania Group** | Software Engineer | Cross-regional EU/Asia MES/MOM systems under strict industrial compliance & security audits |
| 2021–2023 | **Accenture** | Associate Manager / Tech Lead | FinTech platform 0→1 architecture, micro-frontend isolation, audit token lifecycle state machine |
| 2020–2021 | Aosheng Info Tech | Lead Systems Architect | Corporate banking core system migration, static code review + dry-run preflight security gates |

---

### 🎓 Education

| Degree | Institution | Period |
|:-------|:------------|:-------|
| **MSc Applied Computing** (AI Specialization) | Taylor's University, Malaysia | 2025.9–2026.8 |
| B.Eng Mechanical Engineering | Taiyuan University of Technology | 2010.9–2014.9 |

---

### 🧰 Tech Stack

**Security & Infrastructure**
`Zero-Trust` `VNet/NSG` `Private Link` `Managed Identity` `Key Vault RBAC` `HMAC-SHA256` `Entra ID` `Shadow E2E`

**Cloud Platform**
`Azure Container Apps` `Azure Functions` `Cosmos DB` `IoT Hub` `Bicep IaC` `Docker` `ACR` `Log Analytics`

**AI Engineering**
`Azure OpenAI` `Multi-Agent Pipeline` `WebGPU` `RAG` `Transformers` `Semantic Routing` `SSE Streaming`

**Application Development**
`Next.js 14` `FastAPI` `TypeScript` `Python` `React` `Canvas Physics Simulation`

---

<div align="center">

📧 **lsw19920322@gmail.com** · 🔗 **[linkedin.com/in/shengwei-liu](https://linkedin.com/in/shengwei-liu)** · 📍 **Singapore**

</div>

