<div align="center">

# 刘胜伟

**云安全架构师 · 零信任工程实践者 · AI + IoT 全栈工程师**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shengwei--liu-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/shengwei-liu)
[![Location](https://img.shields.io/badge/📍-Singapore-blue?style=flat-square)]()
[![Email](https://img.shields.io/badge/📧-lsw19920322@gmail.com-red?style=flat-square)](mailto:lsw19920322@gmail.com)

**[🇬🇧 English Version](./PROFILE_README.md)**

</div>

---

### 👤 关于我

10+ 年全栈工程经验的 **云安全架构师**。从世界 500 强技术交付主管（Accenture）到欧洲工业制造产线系统（Scania），我的核心能力是**把安全架构从 PPT 落地成跑得动的真实系统**——不只是画 Hub-Spoke 拓扑图，而是写出 Bicep 模板、配好 Private Endpoint、跑通 Shadow E2E 测试证明网络确实是隔离的。

目前持有 5 项 Microsoft 认证（含 **AZ-305 架构专家** 和 **SC-300 身份安全**），正在通过个人旗舰项目 **Project-OmniGuard** 持续深耕云边安全、多智能体 AI 编排与 IoT 设备安全。

---

### 🏅 Microsoft 认证矩阵

<div align="center">

| 认证编号 | 名称 | 领域 |
|:---:|:---|:---|
| **AZ-305** | Azure 解决方案架构师专家 | ☁️ 云架构 |
| **AZ-104** | Azure 管理员 | ☁️ 云运维 |
| **AI-102** | Azure AI 工程师 | 🤖 AI 工程 |
| **SC-300** | 身份与访问管理员 | 🔐 **安全与身份** |
| **AB-100** | Agentic AI 商业架构师 | 🤖 AI 战略 |

</div>

---

### 🛡️ 旗舰项目：OmniGuard

<table>
<tr>
<td width="140" align="center">
<img src="https://img.shields.io/badge/🛡️-OmniGuard-0078D4?style=for-the-badge" />
</td>
<td>

**[Project-OmniGuard](https://github.com/swliu920322/Project-OmniGuard)** — 云边协同安全编排器 · 零信任沙盘 · 6,300+ 行工程代码

一个从零设计并实现的企业级安全平台，部署在 Azure 新加坡区域。不是 Demo，是全链路跑得通的系统。

</td>
</tr>
</table>

#### 我在这个项目里实际造了什么：

**🔐 安全层 — 不是画图，是真能验证的零信任**

- 手写了 **Hub-Spoke VNet 拓扑** + 4 个 Private Endpoint（Cosmos DB / Key Vault / Storage / OpenAI），后端对公网完全不可见（`external: false`）
- 手写了 **HMAC-SHA256 SAS Token 签发**（不是调 SDK 一行搞定，是用 `hmac` + `hashlib` 从协议层手签），用于 IoT Hub C2D 消息认证
- 写了 **287 行自愈式 Shadow E2E 测试**：拉起影子资源组 → 验证 Private DNS A 记录指向 `10.1.2.x` 子网 → 自动销毁。Ctrl+C 也不会泄露资源
- **NSG 双向微分段**：Deny Internet Inbound + Allow Backend Only to Storage Subnet

**🤖 AI 安全层 — 多智能体编排 + 物理级熔断**

- 3-Agent 流水线（Router → Safety Firewall → Action Compiler），带 **2 个早期短路点**：
  - `SENSOR_ERROR` → 立即 STOP，不浪费后续 Agent Token
  - Safety Agent 返回 `BLOCK` → 安全覆盖，动作不会到达物理执行器
- 运动学-Token 定理工程验证：前端物理仿真证明云端 2600ms 延迟下 AGV 无法在碰撞前刹停，必须 15ms 边缘端急刹

**⚡ 边缘计算层 — 浏览器里跑大模型**

- **WebGPU** 在浏览器就地拉起 Qwen2.5-0.5B + MiniLM-L6-v2，$0.00 服务端算力
- 余弦相似度语义路由器（阈值 ≥ 0.72），本地能答的绝不上云

**🏗️ 基础设施层 — 全链路 IaC + 自动化**

- 三层模块化 Bicep（main → nested-infra → compute-module），支持 `sandbox` / `secure-iot` 场景切换
- 可视化 IaC 配置器：在浏览器里配 VNet CIDR、SKU、托管身份，导出可部署的 `.zip` 包
- Bicep 预检编译 + Azure 云端 `az deployment sub validate` 预飞行校验
- **33 份 ADR** 架构决策记录（不只是写代码，还记录了为什么这样做）

**📊 项目数据**

| 指标 | 数值 |
|:-----|:-----|
| 总代码量 | **6,300+ 行**（前端 3,500 + 后端 800 + IaC 560 + 自动化 1,200） |
| ADR 文档 | **33 份**（Infra 8 / Backend 6 / Frontend 13 / Architecture 10） |
| E2E 测试 | 287 行（自愈式，验证私网 DNS + ACA 健康） |
| IoT 全链路 | Event Hub Trigger ↔ C2D 消息（HMAC-SHA256 SAS 手签） |

---

### 💼 工程履历

| 时间 | 公司 | 角色 | 做了什么 |
|:-----|:-----|:-----|:---------|
| 2025–至今 | 独立项目 | **Lead Architect** | OmniGuard：零信任基础设施 + 多智能体 AI 安全 + IoT 设备安全 |
| 2023–2024 | **Scania Group** | Software Engineer | 欧亚跨区域产线 MES/MOM 系统，严格工业合规与安全审计 |
| 2021–2023 | **Accenture** | 技术交付主管 | FinTech 平台 0→1 架构，微前端隔离，审计 Token 生命周期状态机 |
| 2020–2021 | 奥升信息 | Lead Systems Architect | 企业银行核心系统迁移，静态代码审查 + Dry-run 预检安全门 |

---

### 🎓 教育背景

| 学位 | 学校 | 时间 |
|:-----|:-----|:-----|
| **应用计算硕士** (AI 方向) | Taylor's University, Malaysia | 2025.9–2026.8 |
| 机械工程学士 | 太原理工大学 | 2010.9–2014.9 |

---

### 🧰 技术栈

**安全与基础设施**
`Zero-Trust` `VNet/NSG` `Private Link` `Managed Identity` `Key Vault RBAC` `HMAC-SHA256` `Entra ID` `Shadow E2E`

**云平台**
`Azure Container Apps` `Azure Functions` `Cosmos DB` `IoT Hub` `Bicep IaC` `Docker` `ACR` `Log Analytics`

**AI 工程**
`Azure OpenAI` `Multi-Agent Pipeline` `WebGPU` `RAG` `Transformers` `Semantic Routing` `SSE Streaming`

**应用开发**
`Next.js 14` `FastAPI` `TypeScript` `Python` `React` `Canvas 物理仿真`

---

<div align="center">

📧 **lsw19920322@gmail.com** · 🔗 **[linkedin.com/in/shengwei-liu](https://linkedin.com/in/shengwei-liu)** · 📍 **Singapore**

</div>

