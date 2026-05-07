# 🚀 Welcome to Verheyden Tech

![License: Proprietary](https://img.shields.io/badge/License-Proprietary-red.svg)
![Architecture: Micro-Modular](https://img.shields.io/badge/Architecture-Micro--Modular-blue.svg)
![VT AI: Gerar](https://img.shields.io/badge/VT_AI-Gerar-purple.svg)
![Infrastructure: Secure & Scalable](https://img.shields.io/badge/Infrastructure-Secure_%26_Scalable-success.svg)

We build scalable, highly modular, and AI-assisted software ecosystems. Verheyden Tech is an independent software development company specializing in robust enterprise solutions, strictly layered architectures, and intelligent system integrations.

## ⚙️ The Data Control System (DCS)

Our flagship project is **DCS**, a massive, multi-platform enterprise suite. It relies on a strictly hierarchical dependency structure to ensure absolute maintainability, clear domain separation, and high performance across both Desktop (`DCS.Framework`) and Mobile (`DCS.Mobile`) environments.

### 🏗️ Core Architecture
The foundation of the DCS ecosystem is built on atomic, independent modules that cascade into higher-level services. Dependency flows strictly upwards:

* **`DCS.Core`**: The root of the system (Logging, Translations, Resources, IconService). No external dependencies.
* **`DCS.Data`**: The centralized data access layer handling all SQL operations and Server API communications. No external dependencies.
* **`DCS.CoreLib`**: Foundational base classes *(depends on `DCS.Core` & `DCS.Data`)*.
* **`DCS.Authorisation`**: Domain and authorization logic *(depends on `DCS.CoreLib`)*.
* **`DCS.User`**: User management systems *(depends on `DCS.Authorisation`)*.

### 🧩 Feature Modules
Built securely on top of the user and authorization layers, DCS features a wide array of specialized business modules. Every module is a self-contained powerhouse:

`DCS.Billing` | `DCS.Contact` | `DCS.Diary` | `DCS.Document` | `DCS.ERP` | `DCS.Flow` | `DCS.Health` | `DCS.HR` | `DCS.Mailing` | `DCS.Scheduler` | `DCS.Shop` | `DCS.VisPre` (3D Visualization) | *...and expanding.*

---

## 🧠 Project "Gerar" & Intelligent Ecosystem

Verheyden Tech integrates advanced LLM capabilities directly into the development, support, and operational lifecycle. 

**Gerar** is our proprietary AI assistant powered by a locally hosted **Llama 3.1** model, ensuring absolute data sovereignty and security. Rather than functioning as a disconnected tool, Gerar is deeply embedded into the Verheyden Tech infrastructure.

### 🚀 Capabilities & Synergies
The true power of our ecosystem lies in the combination of DCS's rigid, scalable architecture and Gerar's intelligent reasoning:

* **Automated Support Operations:** Gerar is actively being integrated as a context-aware 1st-Level Support agent for the entire DCS ecosystem. The roadmap for Phase 2 includes autonomous 2nd-Level Support, enabling Gerar to actively analyze, debug, and resolve domain-specific issues across all DCS modules.
* **Proprietary Coding Agent:** Gerar is specifically aligned with Verheyden Tech's strict engineering philosophy. It acts as an autonomous development partner that understands our architectural boundaries, enforces our zero-inline-comment policy, and generates perfectly structured XML documentation.
* **Intelligent Data Orchestration:** As the DCS feature set expands, Gerar is designed to intelligently comprehend and query data flows between these highly isolated modules, providing deep insights without compromising the strict architectural layers.
* **Secure & Resilient Infrastructure:** The backbone of our ecosystem relies on a highly optimized, scalable server architecture. We utilize headless Linux environments, fully containerized data layers (Dockerized PostgreSQL), and a zero-trust network architecture (Tailscale VPN) to guarantee maximum security, minimal overhead, and seamless remote orchestration.

---

## 📜 Engineering Philosophy

At Verheyden Tech, quality code is predictable code. We adhere to rigid development conventions to ensure a pristine, scalable codebase:

1. **Self-Documenting Logic:** Inline comments are strictly prohibited. The code's intent must be perfectly clear through its structure, naming, and architectural placement.
2. **Comprehensive XML Documentation:** Every public class, method, and property is meticulously documented using `/// <summary>` tags in professional English.
3. **Strict Namespace Conventions:** Namespaces map structurally, not geographically. We strictly follow the `namespace DCS.[ModuleName].[Layer]` pattern (e.g., `DCS.Billing.Data` or `DCS.User.UI`). Directory structures do not pollute namespaces, with the sole exception of Enums. `using` directives are always placed outside the namespace block.

---

## ⚖️ License & Intellectual Property

All software, codebases, AI system prompts, and architectural designs under the Verheyden Tech organization are proprietary and strictly protected. 

Use, modification, or distribution of this ecosystem is strictly prohibited without explicit, written consent and a valid license agreement. Please refer to the [VT_LICENSE](VT_LICENSE) file in the `.github` repository for the complete legal EULA, including specific restrictions regarding AI exploitation and model scraping.

<br/>

*Driven by logic. Built for scale. Shaping simplicity.*
