# 🏗️ 刘圣伟 (Shengwei Liu) | 云&AI工程师 | AZ-305 专家级架构师

> **"连接先进 Agent 智能体编排与高合规零信任云端基础设施。"**
> 目前就读于马来西亚（攻读 AI 硕士学位） | 计划于 2026 年 8/9/10 月迁往新加坡

---

## 👤 个人简介

资深软件工程师与云架构师，拥有 **8 年以上一线生产环境开发交付经验** 与 **人工智能硕士学位**（主攻企业级 RAG 检索增强生成与多智能体编排）。我兼具深厚的前端状态机逻辑控制底蕴和严谨的云平台工程架构能力，擅长在微软 Azure 上为大模型（LLM）等 AI 业务负载设计并部署安全、高可用且高度合规的专有网络边界。

<p align="left">
  <img src="https://img.shields.io/badge/证书-AZ--104%20Azure%20Administrator-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/证书-AZ--305%20Solutions%20Architect%20Expert-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/证书-SC--300%20Azure%20Identity%20and%20Access%20Administrator%20Associate-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/证书-AI--102%20Azure%20AI%20Engineer%20Associate-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/证书-AB--100%20Agentic%20AI%20Business%20Solutions%20Architect-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
</p>

---

## 🛡️ 代表资产：Project-OmniGuard (硕士毕业设计)
*一款企业级云边协同网络安全决策沙盘系统，用于展示具身智能机队在恶劣边界下的安全状态机执行与遥测数据路由。*

* **零信任私有网络边界 (ACA + Private Link):**  
  在 **Azure Container Apps (ACA)** 上部署了虚拟网络隔离（VNet-isolated）的双容器架构。公网前端 Next.js 充当 **API 网关**，通过内网 DNS 协议将请求转发给私有后端 FastAPI 副本（`external: false`）。利用 **Private Endpoint（私网端点）** 彻底切断了 Cosmos DB、Storage Account 以及 Azure OpenAI 的所有公网入口。
* **云边混合双通道 AI 管线 (WebGPU + 云端大模型):**  
  设计了浏览器端原生 **WebGPU** 语义分流机制（Xenova MiniLM + Qwen2.5），在客户端以 **$0.00 服务端算力开销** 本地解算高频交互与 RAG 检索，只在超出本地知识边界时，通过前端 API 代理流式（SSE）回退到私网内部的 Azure OpenAI。
* **实时遥测与机队治理大盘:**  
  使用 Next.js 构建了可视化大盘，实时呈现机队物理指标（生命值、电量、温度、速度）并集成了网络抖动与延迟模拟器，动态渲染云端基础架构拓扑和 Agent 决策链路。
* **高可靠 DevOps 与击穿缓存的 CI/CD:**  
  编写了声明式 **Bicep** 模板实现基础设施的幂等一键部署。针对 Docker 编译和 Container Apps 镜像拉取中的缓存失效痛点，设计了 `--no-cache` 与 `TRIGGER_VERSION` 环境变量污染相结合的升级流水线，确保新代码与数据快照实时热更新上线。

---

### 🛠️ 技术清单
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

## 🛠️ 技术栈清单
* **云平台与基建:** Microsoft Azure, Azure Container Apps (ACA), Private Link (私网端点), VNet 虚拟网络隔离, ACR, Bicep IaC, Docker
* **人工智能 (AI):** Azure OpenAI Service, 浏览器端 WebGPU 本地推理, Embeddings (向量化), RAG, 语义分流路由
* **后端与 API:** Python, FastAPI, Azure Functions ASGI Host 容器底座, Uvicorn, RESTful API
* **前端与状态:** Next.js (App Router), TypeScript, React, Tailwind CSS, WebSockets, 服务器端发送事件 (SSE 流式传输)

---

## 📈 架构设计哲学
1. **零冗余与明确边界:** 倡导物理目录级的前后端隔离，划清跨团队协作边界，从根本上杜绝代码漂移与依赖臃肿。
2. **基础设施即代码 (IaC):** 所有的网络拓扑、访问权限控制和计算资源必须代码化、版本化，达到企业级安全审计标准。
3. **FinOps 驱动的智能体设计:** 充分释放边缘算力（如 WebGPU），降低云端推理开销，在维护极致数据隐私的同时最大化投资回报比。

---

## 📫 职业目标：新加坡 2026
我正在寻找新加坡的 **资深云架构师 (Senior Cloud Architect)**、**AI 平台工程师 (AI Platform Engineer)** 或 **全栈技术主管/架构师 (Lead Full-Stack Architect)** 职位，面试时间预计为 2026 年 7/8 月。

* **LinkedIn:** [Shengwei Liu](https://www.linkedin.com/in/shengwei-liu/)
* **Email:** [通过 LinkedIn 私信联系]
* **个人简历:** 可根据要求提供完整 PDF 版简历
