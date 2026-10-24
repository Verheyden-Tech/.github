<div align="center">

# 🏛️ VERHEYDEN TECH

### Independent Software Engineering

**Local First · Secure by Design · Human Centered**

*Engineering software that puts people in control of their technology.*

[Website](https://verheyden-tech.de) · [GitHub](https://github.com/Verheyden-Tech)

</div>

---

## 🎯 Who We Are

**Verheyden Tech** is an independent German software engineering company developing modular business applications, intelligent assistance systems, and sovereign infrastructure solutions.

We believe that technology should serve people — not replace their judgment, compromise their privacy, or take control of their information.

Our engineering combines modern desktop applications, local artificial intelligence, modular software architecture, and independently operated server infrastructure into a cohesive ecosystem.

Our ambition is to create professional software that remains understandable, maintainable, secure, and firmly under the control of its operators.

**One ecosystem. Independent components. Human control.**

---

## ⚙️ Our Technology Ecosystem

Our products are designed to complement each other while maintaining clear architectural responsibilities.

| Product | Purpose |
|---|---|
| **Ásgarðr** | Modular desktop workspace and business management |
| **Gerar AI** | Intelligent, locally operated assistance |
| **Herold-OS** | Sovereign server infrastructure and central services |
| **VTOC** | Operations, licensing, monitoring, and customer support |

Together, these systems form the foundation of the Verheyden Tech technology ecosystem.

### 🏛️ Ásgarðr — Your Digital Workspace

**One workspace. Your information. Your control.**

Ásgarðr is our modular Windows desktop platform, designed to bring essential business processes into a consistent working environment.

Rather than forcing users to operate disconnected applications, Ásgarðr brings related workflows together through a unified interface and shared architectural foundations.

Its modular ecosystem includes:

- Contact and relationship management
- Document organization and processing
- Scheduling, appointments, and deadlines
- Email and correspondence
- Billing and business administration
- Human resources and operational workflows
- Case and file management for legal professionals
- Intelligent assistance through Gerar

Ásgarðr is developed primarily with **C#, .NET, and WPF**, supported by independently maintained VT components and libraries.

Local data storage, modular deployment, and controlled system integration are fundamental architectural principles.

**Current direction:** Ásgarðr is undergoing further integration, hardening, and end-to-end validation. Its future architecture is designed to support centrally managed office environments through Herold-OS while preserving practical offline workflows.

### 🧠 Gerar AI — Intelligence in Service of People

**Intelligence with purpose. Assistance with responsibility.**

Gerar AI is Verheyden Tech's intelligent assistant and digital representative.

Inspired by Norse mythology, Gerar embodies knowledge, reliability, discretion, and the responsible use of technological power.

Behind his distinctive identity is a developing assistance platform focused on local AI processing and meaningful integration into everyday workflows.

Gerar's architecture combines:

- Local language-model inference
- Natural-language interaction
- Speech recognition and voice interaction
- Context-aware assistance
- Document and information processing
- Integration with Ásgarðr workflows
- Extensible capabilities through modular tools and interfaces

Gerar is designed to assist users with information retrieval, workflow preparation, and supported application operations.

**Human oversight is a core requirement.** Sensitive or consequential changes must remain subject to appropriate authorization and confirmation.

The long-term objective is an assistant capable of supporting an entire organization through its authorized systems — without surrendering operational control to an external AI provider.

**Current direction:** Local inference, voice interaction, and application integration are under active development and validation. Advanced autonomous and cross-system capabilities remain subject to further engineering and security review.

### 🛡️ Herold-OS — Sovereign Infrastructure

**The foundation of a self-controlled digital environment.**

Herold-OS is Verheyden Tech's dedicated server operating environment for organizations that require greater control over their data, services, and infrastructure.

Based on a minimal Linux foundation, Herold-OS is designed to provide a secure, maintainable platform for centrally operated business services.

Its architecture includes:

- Debian-based minimal operating environment
- Containerized services using Podman and systemd
- Encrypted storage and hardware-backed key protection
- Central database and application services
- Internal service identities and encrypted communication
- Offline-verifiable licensing
- Controlled client synchronization
- Browser-based administration through the Herold Control Center
- Optional dedicated AI infrastructure

Herold-OS is designed around an important principle:

**An organization's core infrastructure should not require permanent dependence on an external cloud to remain operational.**

The platform aims to support offices and professional organizations operating their own infrastructure, with controlled access, defined trust boundaries, and reliable local services.

**Current direction:** Core installation, security, licensing, and service-stack functionality have reached laboratory validation milestones. Hardware validation, administration interfaces, recovery workflows, and production readiness remain ongoing development activities.

### 🖥️ VTOC — Verheyden Tech Operations Center

**One operational perspective across the VT ecosystem.**

VTOC is the internal management and support platform being developed for Verheyden Tech.

Its purpose is to consolidate the operational responsibilities involved in maintaining products, serving customers, and administering deployed infrastructure.

Planned and developing capabilities include:

- Infrastructure and system monitoring
- Centralized incident management
- Customer records and support tickets
- License issuance and administration
- Software package and release management
- Authorized remote diagnostics
- Customer communication and service history
- Auditable operational workflows

VTOC is designed to work alongside the Herold infrastructure without replacing local administrative authority.

Remote maintenance is intended to require explicit authorization, with restricted scopes and auditable operations.

**Current direction:** The application architecture, interface concepts, and foundational workflows are being developed and tested. VTOC is not presented as a generally available product.

---

## 🧭 Our Architecture Philosophy

Technology is trustworthy when its boundaries, responsibilities, and behavior can be understood.

Our engineering follows five principles.

### 🔐 01 — Data Sovereignty

Users and organizations should retain meaningful control over where their information is stored, how it is processed, and which systems can access it.

Local operation and independently controlled infrastructure are preferred wherever practical.

### 🛡️ 02 — Security by Design

Security is not a feature added after implementation.

Authentication, authorization, encryption, service isolation, and controlled access are architectural concerns from the beginning.

### 🧩 03 — Modular Independence

Systems should consist of clearly defined components with explicit responsibilities and controlled dependencies.

Shared functionality belongs in reusable foundations rather than duplicated implementations.

### 🤝 04 — Human Authority

Automation and artificial intelligence should improve human capabilities without silently taking over consequential decisions.

Authorization, transparency, and accountability remain essential.

### 🔧 05 — Long-Term Maintainability

Readable code, predictable behavior, explicit contracts, and repeatable validation are more valuable than unnecessary complexity.

Software should remain maintainable as its ecosystem evolves.

---

## 🛠️ Engineering & Technology

Our technology choices are driven by architectural suitability rather than trends.

| Domain | Core Technologies |
|---|---|
| Desktop applications | C#, .NET, WPF |
| Application architecture | Modular services and VT-owned libraries |
| Local persistence | SQLite-based encrypted storage |
| Server persistence | PostgreSQL |
| Server operating environment | Debian Linux |
| Service orchestration | Podman, systemd |
| API development | .NET, HTTP APIs |
| Administration interfaces | React, TypeScript |
| Local AI | Ollama and local inference components |
| Speech interaction | Local speech-processing components |
| Infrastructure security | TLS, LUKS2, TPM2, hardware-backed trust mechanisms |
| Development workflows | Git, GitHub, automated builds and tests |

Specific implementations may differ between products and deployment environments.

### 📐 Code Quality Standards

Our internal engineering conventions emphasize:

- Self-explanatory names and readable program structure
- Concise English XML documentation for public APIs
- No unnecessary inline comments or explanatory XAML comments
- Clearly separated architectural responsibilities
- Consistent namespaces and dependency boundaries
- Reusable internal packages where technically appropriate
- Warning-free builds as a quality objective
- Automated tests and explicit end-to-end validation
- Human approval for production releases and consequential changes

**A successful build is not equivalent to a validated release.**

---

## 🗺️ Our Development Roadmap

The Verheyden Tech ecosystem is being developed incrementally.

### 🚀 Current Priorities

**Ásgarðr**
- Stabilize application integration and voice-assisted workflows
- Complete critical end-to-end validation
- Prepare controlled pilot operation
- Advance the transition toward Herold-supported environments

**Gerar**
- Improve speech interaction reliability
- Expand authorized application operations
- Strengthen contextual assistance
- Develop modular extension mechanisms

**Herold-OS**
- Complete hardware-level validation
- Implement the Herold Control Center
- Validate backup and recovery procedures
- Establish controlled update and maintenance workflows
- Prepare the platform for managed organizational deployments

**VTOC**
- Consolidate internal support and administration workflows
- Develop infrastructure monitoring and incident handling
- Integrate licensing and software package administration
- Establish auditable remote diagnostics and maintenance

### 🌐 Long-Term Vision

Our objective is a connected but independently controlled software environment in which:

1. **Ásgarðr** provides the professional workspace.
2. **Herold-OS** operates the organization's central infrastructure.
3. **Gerar** provides intelligent assistance across authorized workflows.
4. **VTOC** supports the operational management of the wider ecosystem.

The goal is not to eliminate every external dependency, but to ensure that critical business functions remain as independent, transparent, and resilient as reasonably possible.

*Roadmap descriptions represent development objectives, not commitments to particular release dates or guaranteed feature availability.*

---

## 📦 Development & Availability

Verheyden Tech maintains both active development projects and experimental technology initiatives.

Individual components may be in research, implementation, laboratory validation, pilot preparation, or production operation.

**A documented capability or successful laboratory test does not automatically indicate public availability or production certification.**

Product availability and official announcements are communicated through our website.

Most internal repositories are private because they contain proprietary software and ongoing development work.

---

## ⚖️ Licensing & Intellectual Property

Unless explicitly stated otherwise in an individual repository or accompanying license, Verheyden Tech software is proprietary.

Access to a repository does not by itself grant permission to use, modify, redistribute, or commercially exploit its contents.

Applicable permissions and restrictions are determined by the relevant repository license and contractual agreements.

Third-party software and dependencies remain subject to their respective licenses.

---

## 📬 Connect With Us

**Verheyden Tech — Independent Software Engineering**

Based in Germany. Developing technology for organizations that value independence, security, and responsible innovation.

**Website:** https://verheyden-tech.de

**GitHub:** https://github.com/Verheyden-Tech

For product information, collaboration, or business inquiries, please use the contact options on our official website.

---

<div align="center">

### Technology should serve people.

**Built with purpose. Engineered for independence.**

© 2026 Verheyden Tech

</div>
