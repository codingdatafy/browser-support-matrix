# Contributing to CodingDatafy - Browser Support Matrix

Thank you for your interest in contributing to CodingDatafy. To maintain high data precision, schema integrity, and professional standards across our browser compatibility dataset, please follow these guidelines.

---

## Dataset Workflow

### 1. Issue First Policy
Every contribution or JSON dataset update must address an existing Issue or a newly created one. This ensures that technical tracking efforts are coordinated and align with our platform roadmap.

### 2. Branching Strategy
We follow a strict protected branching model to ensure production stability:
- **`main`**: Reserved for stable, production-ready compatibility releases. Merges here trigger automated production deployment on Vercel.
- **`develop`**: The primary integration branch for staging new JSON datasets and features.
- **`feature/`**: All work must be performed on a dedicated feature branch created from `develop` (e.g., `feature/add-flexbox-support-matrix`).

### 3. Commit Convention
Use professional English for all commit messages. Commits must follow our structured syntax and link to an issue number:
`type(scope): description #issuenumber`

*Example:* `docs(json): add initial browser compatibility matrix for CSS grid #1`

---

## Submission Process

### Step 1: Fork and Branch
- Fork the `browser-support-matrix` repository.
- Create your feature branch from the **`develop`** branch.

### Step 2: Data Implementation
- Ensure all browser compatibility datasets are created strictly as valid, formatted **`.json`** files inside the `/data` directory.
- Verify JSON syntax integrity and check that version numbers match verified browser engine specifications.

### Step 3: Quality Assurance
- Push your changes to your fork.
- Submit a Pull Request (PR) to trigger the automated CI check and preview build pipeline on Vercel.

### Step 4: Pull Request (PR)
- Direct your PR from your feature branch into the CodingDatafy **`develop`** branch.
- Include a clear description of the added or modified web features and reference the related Issue number.

---

## Data Standards & Validation

### Pure JSON Structure
To ensure optimal processing by our core engine (`centroidium`) and compatibility with AI semantic processors, all entries in the `/data` folder must follow strict, unpolluted JSON formatting without inline markdown wrap.

Copyright (c) 2026 CodingDatafy Organization. All Rights Reserved.