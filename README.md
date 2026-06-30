# 🏗️ Shengwei Liu | Cloud & AI Engineer | AZ-305 Solutions Architect Expert
*"The Cloud is just a landing zone. Engineering logic always comes first."*

With 8 years of production software engineering experience and an M.Sc. in AI, I bridge robust frontend state management with highly governed Azure cloud architectures. My focus is on **Enterprise AI Orchestration**—enforcing zero-trust compliance, strict physical network isolation, and deterministic deployment pipelines for LLM workloads.

<p align="left">
  <img src="https://img.shields.io/badge/Cert-AZ--104%20Azure%20Administrator-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/Cert-AZ--305%20Solutions%20Architect%20Expert-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/Cert-SC--300%20Azure%20Identity%20and%20Access%20Administrator%20Associate-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/Cert-AI--102%20Azure%20AI%20Engineer%20Associate-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/Cert-AB--100%20Agentic%20AI%20Business%20Solutions%20Architect-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
</p>

---

### 🛡️ Signature Asset: Project-OmniGuard (Master's Capstone)
A modern, zero-trust cloud-edge collaborative security orchestrator sandbox. Tailored for highly regulated enterprise environments to manage edge-device fleet telemetry and AI reasoning workloads.

* **Zero-Trust Private VNet Architecture (ACA & Private Link):** 
  Orchestrated a secure dual-container topology on **Azure Container Apps (ACA)**. The public-facing Next.js frontend acts as an **API Gateway**, proxying requests to the private backend FastAPI container (`external: false`) via private DNS. Completely eliminated public internet access to Cosmos DB, Storage Account, and Azure OpenAI using **Private Endpoints (Private Link)**.
* **Hybrid Edge-Cloud AI Pipeline (WebGPU & Azure OpenAI):** 
  Engineered an in-browser local RAG pipeline using **WebGPU** (running Xenova/all-MiniLM-L6-v2 and Qwen2.5 local inference) to handle high-frequency interactions on the client side at **$0.00 server cost**. Seamlessly falls back to private Azure OpenAI streaming (SSE) via the Next.js App Router dynamic proxy when local knowledge bounds are exceeded.
* **Real-time Embodied Telemetry Dashboard:** 
  Built a Next.js/React console demonstrating edge fleet metrics (HP, Battery, Velocity, Temp) with network jitter/latency simulators. Integrates live IoT/Event Hub data paths with an visual flowchart of the cloud topology and agent orchestration.
* **Deterministic DevOps & Cache-Busting Pipelines:** 
  Developed a Bicep IaC setup for rapid, idempotent environment recreation. Integrated a custom Docker build-and-deploy pipeline using `--no-cache` builds and automated environment variable pollution (`TRIGGER_VERSION`) to force revision updates and resolve registry cache invalidation bugs.

---

### 🛠️ The Sovereignty Stack
<p align="left">
  <!-- Cloud & Infra -->
  <img src="https://img.shields.io/badge/Azure-0089D6?style=flat-square&logo=microsoft-azure&logoColor=white" />
  <img src="https://img.shields.io/badge/Bicep-0078D4?style=flat-square&logo=microsoft&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <!-- Logic & AI -->
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/WebGPU-black?style=flat-square&logo=webgpu&logoColor=white" />
  <!-- UI / State -->
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
</p>

---

### 📈 Architectural Philosophy
* **Single Foundation:** Code duplication kills agility. I enforce directory-level physical isolation to govern cross-team boundaries and eliminate code drift.
* **Modular Progression:** As a practitioner of progressive calisthenics, I approach distributed systems with the exact same mechanics: refine foundational alignment (network isolation & secure identity) before scaling complex movements (AI applications).

---

### 📫 Target: Singapore 2026
Currently based in Malaysia completing my M.Sc. in AI. Actively seeking **Senior Cloud / AI Architect** roles in Singapore for July/August 2026.

* **LinkedIn:** [Shengwei Liu](https://www.linkedin.com/in/shengwei-liu/)
