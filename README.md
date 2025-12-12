# Technical Due Diligence Playbook

This repository provides a practical, field-tested framework for running Technical Due Diligence (TDD) on software and technology companies.

It’s designed for:

- **Investors (VC / PE)** who need a structured view of technical risk and feasibility  
- **Founders / CTOs** preparing for diligence or doing self-assessment  
- **Advisors / fractional CTOs** who want a repeatable TDD workflow

The focus is on being **evidence-driven, business-informed, and action-oriented** rather than theoretical.

---

## What This Playbook Covers

This playbook organizes TDD into three main phases:

1. **Discovery** – interviews, artifact collection, system review  
2. **Analysis** – scoring across six dimensions, risk identification  
3. **Reporting** – a clear 1–2 page executive readout plus deeper detail where needed

All evaluations are framed through **six dimensions of technical health**:

1. Architecture & Scalability  
2. Security & Risk  
3. DevOps & Reliability  
4. Data & AI Engineering  
5. Team & Process  
6. Roadmap & Technical Debt  

Each dimension is scored on a 0–5 maturity scale with supporting evidence, justification, and risk assessment.

---

## Repository Contents

- `templates/interview_guide.md`  
  Structured question sets for:
  - CTO / Head of Engineering
  - Lead Architect
  - DevOps / SRE Lead
  - Security Lead
  - Data / AI Lead
  - Product Lead

- `templates/scoring_framework.md`  
  The maturity model (0–5), six-dimension scoring grid, and guidance for tying scores to risk and priority.

- `templates/exec_readout_template.md`  
  A 1-page executive readout format investors and founders can use immediately in deal docs and board materials.

- `templates/risk_register_template.md`  
  A simple but rigorous risk register structure (severity × probability, remediation windows, ownership).

- `examples/acme-analytics-example.md`  
  A worked example of how these templates fit together for a hypothetical B2B SaaS company.

---

## How to Use This Playbook

### For Investors (VC / PE)

- Use the **interview guide** to frame initial diligence calls.  
- Use the **scoring framework** to normalize technical assessments across deals.  
- Use the **exec readout template** to plug directly into IC memos:  
  - Overall rating (Green / Yellow / Red)  
  - Top 5–7 risks  
  - 90–180 day remediation priorities  

### For Founders / CTOs

- Use the **six dimensions** as a self-assessment lens ahead of a fundraise or sale.  
- Pre-fill the **risk register** with your honest view of weaknesses and remediation plans.  
- Bring the **exec readout** to your board or prospective investors to control the narrative around technical risk and roadmap feasibility.

### For Advisors / Fractional CTOs

- Treat this as a **baseline methodology**:
  - Adapt questions to the specific vertical and stage.
  - Extend the scoring model with domain-specific criteria (e.g., regulated data, safety-critical systems).
  - Use the same structure across engagements for consistency and comparability.

---

## Six Dimensions at a Glance

All TDD work in this playbook rolls up to these six dimensions:

1. **Architecture & Scalability**
   - System decomposition, boundaries, coupling
   - Scalability constraints and bottlenecks
   - “What breaks first?” under growth

2. **Security & Risk**
   - Identity and access management
   - Data protection, backups, DR
   - Vulnerability management, secure SDLC
   - Regulatory exposure (e.g., privacy, financial)

3. **DevOps & Reliability**
   - CI/CD maturity and deployment safety
   - Observability (logs, metrics, traces, alerts)
   - Incident response and postmortems
   - SRE practices where applicable

4. **Data & AI Engineering**
   - Data model, lineage, and quality
   - ETL / ELT pipelines and governance
   - ML lifecycle (if applicable): training, deployment, monitoring
   - AI risk posture and controls

5. **Team & Process**
   - Org structure and key-person risk
   - Hiring, onboarding, and turnover
   - SDLC practices (planning, code review, testing)
   - Velocity and alignment with product strategy

6. **Roadmap & Technical Debt**
   - Realism of the roadmap versus capacity
   - Known debt and remediation plans
   - Cost-to-achieve key milestones
   - Readiness for scale, integrations, or new markets

---

## Maturity Scale (0–5)

All six dimensions use the same maturity model:

- **0 – Non-existent**  
- **1 – Ad hoc** (inconsistent, depends on individuals)  
- **2 – Emerging** (some patterns, partially documented)  
- **3 – Defined & repeatable** (documented, generally followed)  
- **4 – Measured & optimized** (metrics, feedback loops, continuous improvement)  
- **5 – Best-in-class** (exemplary for stage and context)

Scores should always be backed by **evidence** (logs, code, dashboards, documentation, and cross-checked interviews).

---

## Disclaimer

This playbook is provided for educational and informational purposes only.  
It does not constitute legal, regulatory, or investment advice.

Always adapt the framework to the specific company, domain, and stage you’re evaluating.

