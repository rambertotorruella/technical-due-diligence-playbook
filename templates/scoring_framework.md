# Technical Due Diligence – Scoring Framework

This framework scores a company’s technical health across six dimensions on a 0–5 maturity scale.  
Scores must be backed by evidence, not intuition alone.

---

## Maturity Scale (0–5)

- **0 – Non-existent**  
  No process, practice, or capability in place.

- **1 – Ad hoc**  
  Inconsistent, depends on individuals, little or no documentation.

- **2 – Emerging**  
  Some patterns or tools in place; partially documented; gaps are common.

- **3 – Defined & Repeatable**  
  Documented processes; generally followed; results are predictable.

- **4 – Measured & Optimized**  
  Metrics and feedback loops exist; continuous improvement is visible.

- **5 – Best-in-Class**  
  Exemplary for the company’s stage and domain; a reference model for others.

---

## Six Dimensions

1. Architecture & Scalability  
2. Security & Risk  
3. DevOps & Reliability  
4. Data & AI Engineering  
5. Team & Process  
6. Roadmap & Technical Debt  

---
## Scoring Table Template

Use this table to capture scores, justification, and risk implications.

| Dimension | Score (0–5) | Justification | Key Evidence | Risk Level (L/M/H) | Priority (L/M/H) |
|-------------------------|-------------|-----------------------------------------|------------------------------------------|--------------------|------------------|
| Architecture & Scalability | | | | | |
| Security & Risk | | | | | |
| DevOps & Reliability | | | | | |
| Data & AI Engineering | | | | | |
| Team & Process | | | | | |
| Roadmap & Technical Debt| | | | | |

---

## 5. `templates/exec_readout_template.md`

# Technical Due Diligence – Executive Readout (1 Page)

**Company:** [Company Name]  
**Stage:** [e.g., Seed / Series B / Growth]  
**Date:** [YYYY-MM-DD]  
**Assessor:** [Name / Firm]  

---

## Overall Technical Assessment

**Overall Rating:** [🟢 Low Risk / 🟡 Moderate Risk / 🔴 High Risk]  

**Summary (3–5 sentences):**  
- [Short narrative of overall technical health, feasibility, and alignment with the business and roadmap.]

---

## Key Strengths

1. [Clear, investor-relevant strength – e.g., “Modern, cloud-native architecture with clean service boundaries.”]  
2. [Strength – e.g., “Strong senior engineering leadership with relevant domain expertise.”]  
3. [Strength – e.g., “Healthy deployment cadence and incident response practices.”]  

---

## Key Risks

1. **[Risk Name]** – [One-line description of the issue]  
   - **Impact:** [e.g., Revenue risk, SLA breaches, security exposure]  
   - **Timeframe:** [e.g., Near-term / 6–12 months / 12–24 months]

2. **[Risk Name]** – [One-line description]  
   - **Impact:** [...]  
   - **Timeframe:** [...]

3. **[Risk Name]** – [One-line description]  
   - **Impact:** [...]  
   - **Timeframe:** [...]

(Optionally list up to 5–7.)

---

## Six-Dimension Snapshot

| Dimension                | Score (0–5) | Risk Level (L/M/H) | Short Comment                          |
|-------------------------|-------------|--------------------|----------------------------------------|
| Architecture & Scalability |           |                    | [e.g., Modern core, some hotspots]     |
| Security & Risk         |             |                    | [e.g., Gaps in IAM, solid basics]      |
| DevOps & Reliability    |             |                    | [e.g., Automated CI/CD, weak rollback] |
| Data & AI Engineering   |             |                    | [e.g., Early-stage but promising]      |
| Team & Process          |             |                    | [e.g., Strong leadership, key-person]  |
| Roadmap & Technical Debt|             |                    | [e.g., Ambitious vs capacity]          |



---

## 6. `templates/risk_register_template.md`

# Technical Due Diligence – Risk Register Template

Use this register to track technical risks identified during diligence, along with severity, probability, impact, and remediation plans.

---

## Risk Scoring

- **Severity (1–5):** How bad is it if this risk materializes?  
- **Probability (1–5):** How likely is it to occur in the next 12–24 months?  
- **Risk Score:** Severity × Probability (higher = worse)  
- **Remediation Window:** 30 days / 90 days / 180+ days  

---

## Risk Register Table


| ID | Risk Description                          | Dimension                | Severity (1–5) | Probability (1–5) | Risk Score | Business Impact               | Remediation Recommendation                          | Owner | Target Window |
|----|-------------------------------------------|--------------------------|----------------|-------------------|------------|------------------------------|----------------------------------------------------|-------|---------------|
| R1 | Single point of failure in API gateway    | DevOps & Reliability     | 4              | 3                 | 12         | Outages, SLA breaches        | Implement HA failover and automated failover tests | Eng   | 90 days       |
| R2 | No MFA on admin accounts                  | Security & Risk          | 5              | 3                 | 15         | Account takeover, data breach| Enforce MFA, tighten IAM roles                      | Sec   | 30 days       |
| R3 | Roadmap exceeds current team capacity     | Roadmap & Technical Debt | 3              | 4                 | 12         | Missed milestones, burnout   | Re-scope roadmap; hire or defer initiatives        | Exec  | 180+ days     |

---

## 7. `examples/acme-analytics-example.md`

# Example – Acme Analytics (Hypothetical B2B SaaS)

This example shows how to apply the templates to a fictional Series B analytics company.

---

## Context

- **Company:** Acme Analytics  
- **Stage:** Series B  
- **Product:** B2B analytics platform for mid-market customers  
- **Environment:** Single cloud provider, multi-tenant SaaS  

---

## Six-Dimension Scoring (Example)

| Dimension                | Score (0–5) | Risk Level (L/M/H) | Short Comment                                      | Key Evidence                                  |
|-------------------------|-------------|--------------------|---------------------------------------------------|-----------------------------------------------|
| Architecture & Scalability | 3         | M                  | Generally sound microservice architecture; some   | Architecture diagrams, capacity planning docs |
|                         |             |                    | hotspots around reporting engine under peak load. |                                               |
| Security & Risk         | 2           | H                  | Basic controls in place; gaps in IAM and vendor   | IAM config, pen-test summary, access reviews  |
|                         |             |                    | management; no formal threat modeling.            |                                               |
| DevOps & Reliability    | 
