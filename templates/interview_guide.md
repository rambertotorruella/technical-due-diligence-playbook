# Technical Due Diligence – Interview Guide

This guide provides structured questions for key roles during a Technical Due Diligence engagement.  
Adapt and prioritize based on company stage, domain, and time constraints.

---

## 1. CTO / Head of Engineering

**Goals:** Strategy, constraints, architecture direction, key risks.

- What are the top 3 engineering constraints slowing the business today?
- If we’re successful in 12–24 months, what does the architecture look like?
- Where is the biggest concentration of technical debt right now?
- If we doubled traffic/users tomorrow, what breaks first?
- What keeps you up at night from a technical or operational perspective?
- What are the 2–3 most important technical bets you’re making for the next 18 months?
- Where do you feel the team is overextended or under-resourced?
- How do you decide what *not* to build?

---

## 2. Lead Architect / Principal Engineer

**Goals:** System decomposition, coupling, scalability, debt.

- Walk me through the current high-level architecture. What are the core services and data flows?
- Where is the system most tightly coupled or fragile?
- Which components are hardest to change safely?
- How do you think about scale limits? What breaks first under 10× load?
- What are the top 3 areas of technical debt you would pay down if you had budget and time?
- What major rewrites or replatforming efforts are on the horizon, if any?

---

## 3. DevOps / SRE / Platform Lead

**Goals:** CI/CD, reliability, observability, incident handling.

- How do changes move from idea to production? Walk me through your deployment pipeline.
- How often do you deploy, and how much of that is automated?
- What is your typical time to restore service after an incident?
- How do you monitor the system? Which dashboards/alerts do you rely on most?
- Describe a recent high-severity incident. What happened, and what changed afterward?
- What is your strategy for backups and disaster recovery? How often do you test restores?
- Where are the biggest sources of operational toil or fragility?

---

## 4. Security Lead / Security Owner

**Goals:** Security posture, controls, gaps, and attitude to risk.

- Who is accountable for security, and how is that responsibility structured?
- How is identity and access management handled for engineers, admins, and services?
- Where are your known MFA or privileged access gaps?
- What does your vulnerability management process look like (detection → triage → remediation)?
- When was the last penetration test or third-party security review? What were the high-level findings?
- How do you handle secrets management?
- What is your approach to compliance (e.g., privacy, industry-specific obligations)?
- What security risks worry you the most today?

---

## 5. Data / AI Lead (if applicable)

**Goals:** Data model, pipelines, quality, ML lifecycle.

- What are your primary data sources, and how does data flow through the system?
- How is the data model documented and governed?
- What does your ETL / ELT pipeline look like? Where are the main failure points?
- How do you ensure data quality and correctness?
- If you use ML/AI:
  - What are the main models in production?
  - How are they trained, deployed, and monitored?
  - What can break or drift silently?
- How do you handle data access control and privacy concerns?

---

## 6. Product Lead / Head of Product

**Goals:** Alignment between roadmap, tech capacity, and risk.

- How do you prioritize the product roadmap? Who is involved?
- How confident are you that the current roadmap is achievable with existing capacity?
- Where do technical constraints most limit product strategy today?
- How do you measure engineering productivity and delivery?
- Describe a recent major product initiative: what went well, what didn’t?
- How do you and engineering handle trade-offs between new features and paying down technical debt?
- What are the biggest product and technology risks to the business over the next 12–18 months?

---

## Cross-Verification & Follow-Ups

After interviews:

- Compare answers across roles to identify:
  - Misalignment (e.g., CTO vs Product on roadmap feasibility)
  - Key-person dependencies (“Only Alice understands this subsystem”)
  - Overconfidence or evasiveness (e.g., no concrete examples, no metrics)
- Ask for **artifacts** to validate claims:
  - Diagrams, dashboards, incident reports, test coverage, security findings

Use the insights to populate the **scoring framework**, **risk register**, and **executive readout**.
