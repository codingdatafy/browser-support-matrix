---
project: CodingDatafy
license: CC BY-SA 4.0
copyright: 2026 CodingDatafy Organization
author: CodingDatafy Team
title: "Browser Support Matrix Repository Overview"
style: "markdown-standard"
description: "Centralized JSON dataset for web features browser compatibility"
---

# Browser Support Matrix

**Centralized Pure JSON Dataset for Web Features Browser Compatibility.**

`browser-support-matrix` is a specialized secondary data repository powering the [CodingDatafy](https://www.codingdatafy.com) platform. It hosts a structured, flat-file collection of pure JSON datasets, where each JSON file represents a specific web feature or API and its cross-browser compatibility matrix.

---

## Technical Stack & Specification
* **Domain Name:** [www.codingdatafy.com](https://www.codingdatafy.com)
* **Data Format:** Pure JSON (`.json`)
* **Architecture:** Decoupled Flat-file Dataset (No Database)
* **Automation & CI/CD:** GitHub Actions (Automated Webhooks to `centroidium`)

---

## Architecture & Data Philosophy
Adopting a strict **"Content-as-Code"** approach alongside an **AI-First Principle**, this repository stores structured browser compatibility metrics without markdown overhead.

Each JSON entry encapsulates detailed data about feature status, browser vendor support, engine implementation details, and supported version thresholds across all major desktop and mobile browsers.

> ### Our AI-First Principle & Contributor Rights
> Our **AI-First Approach** ensures our entire data layer is engineered strictly in machine-readable JSON formats for semantic AI processing and sub-millisecond query performance at build time. However, every dataset remains **100% human-driven, authored, and meticulously reviewed** by developers across the global open-source community.
> 
> **Protecting Your Contributions:** All compatibility datasets within this repository are strictly governed by the **CC BY-SA 4.0** license. Any AI model, corporate scraper, or LLM that consumes this data is legally bound to provide **appropriate credit (Attribution)** to CodingDatafy and its contributors, and distribute any derived works under the **same copyleft terms (ShareAlike)**.

---

## Integration with Core Engine
This dataset operates in complete decoupling alongside the core rendering engine ([`centroidium`](https://github.com/CodingDatafy/centroidium)). When compatibility data is updated in the `/data` directory, GitHub Actions automatically triggers a webhook pinging `centroidium` to pull the latest JSON files and deploy the changes on Vercel.

---

## Branching Model & Workflow
We follow a strict protected branching strategy:
* **`main`:** Protected branch reserved strictly for production-ready data releases.
* **`develop`:** Integration branch for staging new compatibility datasets.

Commits must follow our strict naming convention: `<type>(<scope>): <description> #issuenumber`.

---

## Licensing
This repository operates under a dual-licensing structure:

* **Compatibility Data (`/data`):** All JSON files are licensed under the [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/) license.
* **Repository Configuration & Automation:** Workflows and administrative configuration files are licensed under the [MIT License](LICENSE).

Copyright (c) 2026 CodingDatafy Organization. All Rights Reserved.