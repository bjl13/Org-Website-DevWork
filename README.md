# BJL13 Enterprise Solutions — Org Website (`dev/com-buildout`)

[![Branch](https://img.shields.io/badge/branch-dev--com--buildout-blueviolet)](https://github.com/BJL13-Enterprise-Solutions/Org-Website/tree/dev/com-buildout)
[![Status](https://img.shields.io/badge/status-in%20buildout-orange)](#status)
[![Astro](https://img.shields.io/badge/built%20with-astro-ff6f00)](https://astro.build/)
[![Accessibility](https://img.shields.io/badge/accessibility-WCAG%202.2%20%2F%20ADA-success)](https://www.w3.org/WAI/standards-guidelines/wcag/)
[![License: MIT](https://img.shields.io/github/license/BJL13-Enterprise-Solutions/Org-Website?color=green)](./LICENSE)

---

> **NOTE:**  
> You are viewing a personal staging of the site before it will go live.   
> Content here is **not yet live or canonical** unless mirrored in `/main`.  
> For the authoritative site and documentation, see the [`/main` branch](https://github.com/BJL13-Enterprise-Solutions/Org-Website/tree/main).

---

## 📜 [Mission Statement](./Mission-Statement.md)

## 🤝 [Partnership Information](./Partnership-Info.md)

---

## Overview

This branch powers the **.com buildout** for BJL13 Enterprise Solutions, a public-benefit LLC specializing in digital equity, automation, and accessible technology. We are currently in active development—expect rapid changes, breaking features, and experimental integrations.

[Full technical stack, folder structure, getting started, and contribution guidelines are below—see original README for details.]

---
# ✦ Core Product — AI Public Worker MVP  
**BJL13 Enterprise Solutions LLC**  
_A Digital Public Worker for Navigating Bureaucracy with Dignity_

---

## 🧭 Overview

This is the Core Product buildout for **BJL13 Enterprise Solutions (BES)** — a public-benefit LLC building tools that empower people marginalized by existing systems.

This MVP creates an **AI-augmented digital public worker**, designed to:
- Help users complete government forms
- Translate legal/bureaucratic language into plain English
- Auto-fill documents
- Advocate for users in navigating housing, health, legal, and economic systems

---

## 🔧 Features

- 📄 **Form Assistance**: Real-time help filling out forms (PDFs, applications, appeals)
- 🗣️ **Plain-Language Translation**: Converts jargon into understandable terms
- 🤝 **Resource Matching**: Finds and suggests mutual aid, legal aid, and government resources
- 🧠 **Explainable AI**: All steps include explanations of how/why answers were generated
- 🪄 **PDF Generation**: Outputs filled or templated PDFs, letters, or filings
- 🧱 **Modular**: Easily extended for local/state/federal support and multilingual use

---

## ⚙️ Tech Stack

| Component        | Tech Suggestion                         |
|------------------|------------------------------------------|
| Backend API      | `FastAPI` or `Express.js`                |
| AI Memory/RAG    | `FAISS`, `Weaviate`, or `Chroma`         |
| Agentic Logic    | `LangChain`, `CrewAI`, or `AutoGen`      |
| Form Automation  | `Playwright`, `Puppeteer` (optional)     |
| UI Framework     | `Tailwind CSS`, `Chakra UI`, `Next.js`   |
| Containerization | `Docker`, `docker-compose`               |

---

## 🧪 MVP Roadmap

### ✅ Phase 1: Local CLI + PDF Generator
- [ ] CLI accepts plain-language queries
- [ ] Agent identifies form type + needed info
- [ ] System responds with:
  - Guidance
  - Optional filled PDF
  - Resource links

### 🖥️ Phase 2: Web App Integration
- [ ] Minimal UI w/ text box and output card
- [ ] Upload PDF or select from common forms
- [ ] Edit & preview outputs
- [ ] One-click export

### 🔗 Phase 3: Memory + Agentic Routing
- [ ] Add embedded knowledge store (FAISS)
- [ ] Connect multiple specialist agents
- [ ] Log outputs to local secure storage

---

## 🧑‍💻 Getting Started

```bash
# Clone the repository
git clone https://github.com/bjl13/core-product.git
cd core-product

# Copy environment config
cp .env.example .env

# Launch with Docker
docker-compose up --build
