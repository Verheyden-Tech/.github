# 🚀 Welcome to Verheyden Tech

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

`DCS.Billing` | `DCS.Contact` | `DCS.Diary` | `DCS.Document` | `DCS.ERP` | `DCS.Flow` | `DCS.Health` | `DCS.HR` | `DCS.Mailing` | `DCS.Scheduler` | `DCS.Shop` | `DCS.VisPre` (3D Visualization) | so far, to be continued..

---

## 🧠 Project "Gerar": AI-Driven Infrastructure

Verheyden Tech integrates advanced LLM capabilities directly into the development and support lifecycle. 

**Gerar** is our proprietary AI assistant powered by **Llama 3.1**, running entirely in-house on a dedicated, high-performance edge node:
* **Roadmap:** Gerar is actively being integrated into the DCS ecosystem as a Level 1 Support agent, with Phase 2 expanding its capabilities to autonomous Level 2 Support and a dedicated Verheyden Tech coding agent.

---

## 📜 Engineering Philosophy

At Verheyden Tech, quality code is predictable code. We adhere to rigid development conventions to ensure a pristine, scalable codebase:

1.  **Self-Documenting Logic:** Inline comments are strictly prohibited. The code's intent must be perfectly clear through its structure, documentation and naming.
2.  **Comprehensive XML Documentation:** Every public class, method, and property is meticulously documented using `/// <summary>` tags in professional English.
3.  **Strict Namespace Conventions:** Namespaces map structurally, not geographically. We strictly follow the `namespace DCS.[ModuleName].[Layer]` pattern (e.g., `DCS.Billing.Data` or `DCS.User.UI`). Directory structures do not pollute namespaces, with the sole exception of Enums. `using` directives are always placed outside the namespace block.

<br/>

*Driven by logic. Built for scale. Shaping simplicity.*
