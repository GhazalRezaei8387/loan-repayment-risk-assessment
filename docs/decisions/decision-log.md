# Project Decision Log

This file records project decisions that have been discussed and explicitly selected. Proposals and assumptions are labeled separately from confirmed decisions.

## Decision 001 — Select the Initial Project Scope

- **Date:** 2026-11-18
- **Status:** Confirmed
- **Decision:** Select the focused, research-oriented scope: estimate the risk of default for a loan applicant before a new loan is granted.
- **Options considered:**
  1. Assess applicants before granting a loan.
  2. Monitor repayment behavior of existing borrowers.
  3. Build a broad system covering both.
- **Reason:** The focused scope provides a clearly bounded research problem, supports comparison and evaluation of machine-learning methods, and is more manageable for a bachelor's project while retaining meaningful software-engineering work.
- **Included in initial scope:** Applicant assessment, default-risk estimation, risk presentation, and analytical reporting.
- **Excluded from initial scope:** Ongoing monitoring of existing loans, direct integration with a real bank, payment processing, and automatic final lending decisions.
- **Consequences:** Requirements and research will focus first on pre-loan risk assessment. Monitoring may be documented as future work.

## Working Assumptions — Not Final Decisions

### A. Supervised learning
Historical examples with known repayment outcomes are expected to be useful. Supervised learning is therefore the current working direction, subject to dataset and target feasibility.

### B. Binary classification
Default versus non-default is a plausible initial target formulation. It cannot be finalized until default and the relevant time windows are operationally defined.

### C. Human-in-the-loop decision support
The system is intended to support a human reviewer. It should not be presented as an authority that automatically approves or rejects loans.

## Open Decisions

- **D-002:** Define default operationally, including delinquency thresholds and any applicable dataset-specific definition.
- **D-003:** Define the observation window, prediction horizon, and outcome/performance window.
- **D-004:** Select and justify a dataset.
- **D-005:** Define the target variable and eligible input features.
- **D-006:** Select model candidates and the evaluation/validation protocol.
- **D-007:** Select the software architecture and implementation technologies.

New decisions should be appended with an ID, date, status, alternatives, rationale, and consequences. Do not silently overwrite a previous decision; record a superseding decision when needed.
