# Project Overview

## 1. Project Identity

- **Working title:** Bank Loan Repayment Risk Assessment System
- **Project type:** Bachelor's degree project
- **Domain:** Credit risk assessment
- **Current phase:** Problem definition and requirements analysis
- **Scope version:** 1.0 (initial scope selection; details remain open)

## 2. Problem Context

A lender needs to assess whether a loan applicant may fail to meet repayment obligations. The proposed system will use applicant-related information and a model trained on historical loan data to estimate the risk of default.

The system should present its result in an understandable form so that a human reviewer can use it as decision support.

## 3. Selected Scope

The selected direction is the **focused, research-oriented version**:

- Assess an applicant before a new loan is granted.
- Estimate the probability or risk of loan default.
- Assign an interpretable risk category only after its thresholds have been justified.
- Present an analytical result or report.
- Keep final lending decisions under human responsibility.

Monitoring repayments of already-issued loans is outside the initial scope and may be considered as future work.

## 4. Initial Scientific Framing

The current working formulation is a supervised prediction task. Binary classification is a plausible initial formulation if the target is defined as default versus non-default.

This is not yet a finalized modeling decision. The operational definition of default, observation window, prediction horizon, and label construction must be specified before dataset selection and model training.

## 5. Expected High-Level Flow

1. Receive applicant information.
2. Validate the submitted information.
3. Apply the required data preparation and feature transformations.
4. Generate a model-based estimate of default risk.
5. Present the estimate and relevant explanatory information.
6. Store the assessment result where appropriate.

This flow is preliminary and will be refined during requirements analysis and design.

## 6. Constraints and Limitations

- A prediction is an estimate, not a guarantee of future repayment behavior.
- Model quality depends on the relevance, quality, and representativeness of the data.
- Performance on one dataset does not guarantee performance in another bank, country, or population.
- The system is a decision-support tool, not an autonomous loan-approval authority.
- Predictive associations must not automatically be interpreted as causal relationships.
- Privacy, fairness, and responsible use of financial data must be considered.

## 7. Decisions Still Open

- Operational definition of default.
- Prediction horizon and observation/performance windows.
- Dataset and its suitability.
- Input features and target-label construction.
- Data preprocessing and leakage prevention.
- Candidate algorithms and model-selection procedure.
- Evaluation metrics and validation strategy.
- Application architecture, programming language, database, and interface.
- Security, privacy, fairness, and explainability requirements.
