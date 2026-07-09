<div align="center">

# 刘胜伟 | Shengwei Liu

**Cloud Security Architect · AI Safety Researcher · Zero-Trust Practitioner**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shengwei--liu-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/shengwei-liu)
[![Location](https://img.shields.io/badge/📍-Singapore-blue?style=flat-square)]()
[![Email](https://img.shields.io/badge/📧-lsw19920322@gmail.com-red?style=flat-square)](mailto:lsw19920322@gmail.com)

</div>

---

### 👤 About Me

I am a **Solutions Architect** with 10+ years of engineering experience, currently pursuing research at the intersection of **cloud-edge security**, **AI safety for embodied systems**, and **zero-trust infrastructure hardening**. I hold a Master's degree in Applied Computing (AI Specialization) from Taylor's University and am seeking a **PhD opportunity in Cybersecurity** in Singapore to advance my research on securing autonomous AI decision-making pipelines.

My core thesis — the **Kinematic-Token Theorem** — formally proves that cloud-only LLM inference latency creates a physical safety deadlock for real-time autonomous vehicle control, and proposes a multi-layered defense architecture combining network isolation, AI safety firewalls, and edge computing to resolve it.

> *"My moat is not the technologies I use, but the security judgments I make — where to short-circuit, where to isolate, where to degrade."*

---

### 🔬 Research Interest

**Securing AI-Driven Cyber-Physical Systems: Zero-Trust Architecture, Multi-Agent Safety Orchestration, and Edge-Cloud Hybrid Defense**

| Research Dimension | My Contribution |
|:-------------------|:----------------|
| **Zero-Trust Network Security** | Hub-Spoke VNet + 4 Private Endpoints + bidirectional NSG + Managed Identity. Backend invisible from public internet. Validated by automated Shadow E2E test verifying Private DNS A records |
| **AI Safety & Alignment** | 3-Agent pipeline (Router → Safety Firewall → Action Compiler) with cascading early circuit-breaking. Safety agent can **BLOCK** unsafe physical actions before they reach actuators |
| **Edge Computing Security** | WebGPU in-browser inference ($0.00 server cost) protects user privacy — sensitive data never leaves the client device, reducing the cloud attack surface to zero for high-frequency queries |
| **Formal Verification of AI Control Deadlocks** | Kinematic-Token Theorem: mathematical proof that $v \times T_{cloud} > d_{obstacle} - d_{brake}$ at operational speeds, necessitating hybrid edge-cloud cognitive pipelines |
| **IoT Protocol Security** | Hand-crafted HMAC-SHA256 SAS Token signing (not SDK wrapper) for IoT Hub C2D messaging, demonstrating deep understanding of authentication protocols |
| **Infrastructure Security Testing** | Self-healing Shadow E2E test suite: deploys full infrastructure replica → audits Private DNS resolution → auto-destroys with Ctrl+C signal safety |

---

### 🏅 Microsoft Certifications

<div align="center">

| Certification | Title | Domain |
|:---:|:---|:---|
| **AZ-305** | Azure Solutions Architect Expert | ☁️ Cloud Architecture |
| **AZ-104** | Azure Administrator Associate | ☁️ Cloud Operations |
| **AI-102** | Azure AI Engineer Associate | 🤖 AI Engineering |
| **SC-300** | Identity and Access Administrator | 🔐 **Security & Identity** |
| **AB-100** | Agentic AI Business Architect | 🤖 AI Strategy |

</div>

---

### 🛡️ Flagship Project

<table>
<tr>
<td width="140" align="center">
<img src="https://img.shields.io/badge/🛡️-OmniGuard-0078D4?style=for-the-badge" />
</td>
<td>

**[Project-OmniGuard](https://github.com/swliu920322/Project-OmniGuard)** — Cloud-Edge Collaborative Security Orchestrator & Zero-Trust Sandbox

An enterprise-grade security platform proving that cloud-only AI inference creates physical safety deadlocks for autonomous fleets, with a full Zero-Trust defense architecture deployed on Azure Singapore.

</td>
</tr>
</table>

**Security Architecture Highlights:**

```
Public Internet
    │
    ▼
┌────────────────────────────────┐
│ Next.js API Gateway (BFF)      │  ← Only public-facing surface
│ Catch-all route proxy          │     Hides all internal paths
└───────────┬────────────────────┘
            │ .internal DNS (private)
            ▼
┌────────────────────────────────┐
│ FastAPI Backend                │  ← external: false
│ (VNet-internal ONLY)           │     Invisible from internet
└───────────┬────────────────────┘
            │ Private Endpoints (zero public access)
            ▼
┌──────┬──────────┬──────────┬──────────────┐
│Cosmos│ Key Vault│   Blob   │ Azure OpenAI │
│  DB  │  (RBAC)  │  Store   │  (Private)   │
└──────┴──────────┴──────────┴──────────────┘
```

**Key Metrics:**

| Metric | Value |
|:-------|:------|
| Total Codebase | **6,300+ lines** across frontend, backend, IaC, and automation |
| Architecture Decision Records | **33 ADRs** (documented engineering reasoning) |
| IaC Templates | 3-layer modular Bicep (main → infra → compute) |
| E2E Security Test | 287-line self-healing Shadow test with Private DNS validation |
| Multi-Agent Pipeline | 3 agents with 2 circuit-breaker short-circuits |
| Edge AI Inference | WebGPU Qwen2.5 + MiniLM-L6-v2 at $0.00 server cost |

---

### 💼 Professional Experience

| Period | Company | Role | Security-Relevant Work |
|:-------|:--------|:-----|:-----------------------|
| 2025–Present | Independent | **Lead Architect** | Project-OmniGuard: Zero-Trust infra, Multi-Agent AI safety, IoT security |
| 2023–2024 | **Scania Group** | Software Engineer | Industrial MES/MOM systems under strict **compliance and security audit** standards |
| 2021–2023 | **Accenture** | Associate Manager / Tech Lead | FinTech platform architecture with **audit token life-cycle management** and modular isolation |
| 2020–2021 | Aosheng Info Tech | Lead Systems Architect | Corporate banking migration with **static code review and dry-run preflight checks** |

---

### 🎓 Education

| Degree | Institution | Period | Focus |
|:-------|:------------|:-------|:------|
| **MSc Applied Computing** (AI Specialization) | Taylor's University, Malaysia | 2025.9–2026.8 | Enterprise RAG, Multi-Agent Orchestration |
| B.Eng Mechanical Engineering | Taiyuan University of Technology | 2010.9–2014.9 | — |

---

### 🧰 Technical Stack

**Security & Infrastructure**
`Zero-Trust` `VNet/NSG` `Private Link` `Managed Identity` `Key Vault RBAC` `HMAC-SHA256 SAS` `Entra ID (SC-300)` `Shadow E2E Testing`

**Cloud & DevOps**
`Azure Container Apps` `Azure Functions` `Cosmos DB` `IoT Hub` `Bicep IaC` `Docker` `ACR` `Log Analytics`

**AI & Machine Learning**
`Azure OpenAI` `Multi-Agent Orchestration` `WebGPU Inference` `RAG` `Transformers` `Semantic Routing` `SSE Streaming`

**Application Development**
`Next.js 14` `FastAPI` `TypeScript` `Python` `React` `Canvas/Physics Simulation`

---

### 📊 GitHub Stats

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=swliu920322&show_icons=true&theme=tokyonight&hide_border=true&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=swliu920322&layout=compact&theme=tokyonight&hide_border=true)

</div>

---

### 🎯 What I'm Looking For

I am actively seeking a **PhD position in Cybersecurity / AI Safety** in Singapore. My research aims to extend the Kinematic-Token Theorem into a formal framework for securing AI-driven cyber-physical systems, with focus on:

- 🔐 **Zero-Trust architectures** for autonomous IoT fleets in adversarial network environments
- 🤖 **AI safety guarantees** through multi-agent compliance firewalls with formal verification
- ⚡ **Edge-cloud hybrid security** — proving that local compute reduces both latency and attack surface
- 🏗️ **Infrastructure security testing** — automated shadow environment validation of network isolation

> If your lab works on securing AI systems, cloud-edge security, or IoT/CPS safety, I would love to connect.

---

<div align="center">

📧 **lsw19920322@gmail.com** · 🔗 **[linkedin.com/in/shengwei-liu](https://linkedin.com/in/shengwei-liu)** · 📍 **Singapore**

</div>
