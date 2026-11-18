# Initial Requirements Register

**Status:** Draft — preliminary requirements, not yet baselined.

Requirements will receive stable IDs. Their wording and acceptance criteria will be refined as the project is analyzed.

## 1. Functional Requirements

| ID | Initial requirement | Status |
|---|---|---|
| FR-01 | The system shall receive the information required to assess a loan applicant. | Draft |
| FR-02 | The system shall validate submitted information and identify invalid or missing values. | Draft |
| FR-03 | The system shall prepare input data using the transformations required by the selected model. | Draft |
| FR-04 | The system shall estimate the applicant's risk of default using a trained model. | Draft |
| FR-05 | The system shall present the estimated risk in an understandable form. | Draft |
| FR-06 | The system shall provide an assessment summary or analytical report. | Draft |
| FR-07 | The system shall store assessment results if storage is confirmed as a system requirement. | To validate |

## 2. Non-Functional Requirements

| ID | Quality attribute | Initial expectation | Status |
|---|---|---|---|
| NFR-01 | Reliability | The model and application behavior shall be evaluated and documented. | Draft |
| NFR-02 | Security and privacy | Personal and financial information shall be protected. | Draft |
| NFR-03 | Performance | Assessment response time shall be measured against a defined target. | To specify |
| NFR-04 | Maintainability | The codebase shall be modular, readable, and testable. | Draft |
| NFR-05 | Explainability | The system should provide understandable information about model outputs and limitations. | Draft |
| NFR-06 | Fairness | Potential bias and limitations across relevant groups shall be considered where data and law permit. | To investigate |

## 3. Out of Scope for the Initial Version

- Monitoring installment payments after a loan has been issued.
- Direct integration with a real bank's production systems.
- Payment processing or money transfers.
- Automatic and final approval/rejection of loan applications.

## 4. Items Requiring Further Analysis

- Exact applicant fields and their definitions.
- Meaning of missing, invalid, and inconsistent values.
- Operational definition of default.
- Prediction horizon and outcome window.
- Report contents and risk-category thresholds.
- User roles and authentication needs.
- Data retention and access-control requirements.
- Measurable acceptance criteria for each requirement.
