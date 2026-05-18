# Clinical Decision Support System (CDSS) & Deterministic Triage Engine

A lightweight, zero-latency, client-side medical triage and automated prescription formatting system engineered for optimized clinical workflows.

**Production Live Link:** https://ananthaaju-dev.github.io/ai-prescription-maker/

---

## Technical Architecture & Design Decisions

* **Client-Side Edge Execution:** Built entirely as a Single Page Architecture (SPA) to ensure zero network latency during critical patient evaluations. Keeping computation local guarantees 100% data privacy—clinical parameters never leave the provider's machine.
* **Deterministic Triage Framework:** Replaced slow probabilistic processing with structured object mapping and custom JSON dictionaries to instantly flag and cross-reference localized symptoms and critical keywords.
* **Dynamic Patient State Caching:** Engineered a volatile local state management machine that dynamically tracks symptom inputs, diagnostic summaries, and pharmaceutical dosages before generating output states.

---

 Core Engineering Highlights

 1. Algorithmic Risk Stratification
The core JavaScript engine handles clinical prioritization automatically:
* **Acute/Urgent Classifications:** Instantly triggers visual warnings if key red-flag conditions match the input matrix.
* **Routine Management:** Formats non-critical cases automatically to minimize administrative overload.

2. Print-Optimized Layout Integration
Designed custom CSS `@media print` rules directly into the interface. This allows physicians to seamlessly export cleanly formatted, standard-compliant physical prescriptions with a single keystroke, bypassing bulky browser UI elements.

---

##  Scalability Roadmap

* **Phase 1 (Current):** Standalone lightweight client prototype with integrated clinical lexicons.
* **Phase 2 (Planned):** Migration to a robust full-stack ecosystem utilizing a decoupled frontend framework (React.js) and a secure server layer (Node.js/Express).
* **Phase 3 (Enterprise):** Implement end-to-end encryption (E2EE) data pipelines for healthcare standard compliance and integrate vector-based large language model endpoints for deep diagnostic cross-checking.

---
*Developed as an independent research prototype in high-performance digital healthcare automation.*
