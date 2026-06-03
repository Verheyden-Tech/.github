<div align="center">

# 🏛️ Verheyden Tech

> **Independent software engineering — enterprise architecture, AI integration, and absolute data sovereignty.**

[![License: VT Proprietary](https://img.shields.io/badge/License-VT_Proprietary-800020.svg)](https://github.com/Verheyden-Tech/.github/blob/main/VT_LICENSE.md)
![Architecture: Micro-Modular](https://img.shields.io/badge/Architecture-Micro--Modular-1A1A1A.svg)
![AI: Gerar VT-Proprietary](https://img.shields.io/badge/AI-Gerar_VT--Proprietary-B8860B.svg)
![Infrastructure: Secure & Local](https://img.shields.io/badge/Infrastructure-Secure_%26_Local-800020.svg)

</div>

---

## 🎯 Who We Are

Verheyden Tech is an independent software development company specialising in robust enterprise solutions, strictly layered architectures, and intelligent system integrations. Every component we ship is predictable, auditable, and built for long-term operational scale.

---

## ⚙️ The Data Control System (DCS)

Our flagship product is **DCS** — a multi-platform enterprise suite delivering desktop (`DCS.Framework`) and mobile (`DCS.Mobile`) experiences from a single, rigorously layered codebase.

### 🏗️ Architecture

Dependencies flow strictly downward. No module may reference a peer or upstream layer.

```text
Layer 0/1  DCS.Data.Shared ──► DCS.Data  ◄── DCS.Core
Layer 2    DCS.CoreLib
Layer 3    DCS.Authorisation
Layer 4    DCS.User
Layer 5    Feature Modules (Tier 1–4)
Layer 6    DCS.Framework (WPF)  ·  DCS.Mobile (MAUI)
```

### 🧩 Feature Modules

Every module is a self-contained solution following the canonical four-assembly split (Core / Data / Service / UI):

`DCS.Billing` · `DCS.Contact` · `DCS.Diary` · `DCS.Document` · `DCS.ERP` · `DCS.Fleet` · `DCS.Flow` · `DCS.Gastro` · `DCS.Health` · `DCS.HR` · `DCS.Mailing` · `DCS.Scheduler` · `DCS.Shop` · `DCS.VisPre`

---

## 🧠 Gerar AI

**Gerar** is the proprietary AI core of Verheyden Tech — a fully local, production-grade AI assistant running on a self-hosted Ollama inference stack.

### Architecture

```text
VT.Gerar.UX  (WPF chat client)
     │
Gerar Bridge  (FastAPI · localhost:8765)
     │
Ollama  (Qwen3:14B Q6_K · localhost:11434)
     │
Hardware: Ryzen 7 5700X · RX 6800 XT · 32 GB RAM
```

### Capabilities

**Coding Agent** — Gerar operates as an autonomous development partner with full access to the DCS codebase. It enforces VT architectural conventions, generates XML-documented C# across all layers, executes `.NET` builds, manages Git, and iterates on compile errors without human intervention.

**First & Second Level Support** — Gerar is the context-aware support agent for all DCS modules. It queries live production data (`dcs_main` PostgreSQL), resolves issues, and escalates with full technical context.

**Threat Intelligence Unit (TIU)** — Gerar serves as the forensic investigator of the Verheyden Tech TIU. It conducts geolocation and ASN analysis, DNS/WHOIS/TLS reconnaissance, log analysis for attack patterns, and produces court-ready forensic reports with a verifiable hash-linked chain of custody.

**Self-Improvement** — Gerar can propose, review, and apply changes to its own codebase through a gated `propose → approve → apply` workflow. No silent self-modification.

### Data Sovereignty

- Runs exclusively on local hardware — no cloud, no telemetry
- Ollama bound to `127.0.0.1` — no LAN exposure by default
- All chat history, file access, and model outputs remain on the host machine
- Web search is an explicit opt-in tool, not a background process
- Vector memory (`nomic-embed-text`) is stored locally with a hard 2 000-entry limit and automatic consolidation

### Ecosystem

| Repository | Description |
|---|---|
| [`Gerar-AI`](https://github.com/Verheyden-Tech/Gerar-AI) | Bridge, tools, memory, system prompt, voice listener |
| [`VT.Gerar.UX`](https://github.com/Verheyden-Tech/VT.Gerar.UX) | WPF chat client with session management, output modes, TTS |
| [`VT.Gerar.Installer`](https://github.com/Verheyden-Tech/VT.Gerar.Installer) | Visual setup wizard — hardware detection, model selection, three installation modes |

---

## 📜 Engineering Philosophy

Quality code is predictable code. Verheyden Tech adheres to rigid development conventions across every repository.

**Self-documenting logic** — inline comments are prohibited. Intent is expressed through structure, naming, and architectural placement.

**Comprehensive XML documentation** — every public class, method, and property carries a `/// <summary>` in professional English.

**Strict namespace conventions** — namespaces follow `DCS.[ModuleName].[Layer]` (e.g., `DCS.Billing.Data`, `DCS.User.UI`). Directory structures do not pollute namespaces, with the sole exception of Enums. `using` directives are always placed outside the namespace block.

**Proprietary primitives** — DI resolution, base classes, commands, and result types are all VT-owned. No third-party DI frameworks, no community MVVM toolkits.

**Zero-warning builds** — every assembly ships clean. Warnings are treated as build defects.

---

## ⚖️ License & Intellectual Property

All software, codebases, AI configurations, system prompts, and architectural designs under the Verheyden Tech organisation are proprietary and strictly protected.

Use, modification, or distribution without explicit written consent and a valid license agreement is prohibited. See [`VT_LICENSE.md`](https://github.com/Verheyden-Tech/.github/blob/main/VT_LICENSE.md) for the complete EULA, including restrictions on AI exploitation and model scraping.

---

<div align="center">

*Driven by logic. Built for scale. Owned end to end.*

© 2026 Verheyden Tech

</div>
