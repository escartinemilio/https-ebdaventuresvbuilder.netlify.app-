---
title: Regulatory Watch
description: Ongoing tracking surface for the regulations that govern EBDA Ventures' studio and portfolio companies — HIPAA, FDA AI/ML, EU AI Act, MDR, state-level US rules, GDPR
last_updated: 2026-05-16
updated_by: ion
status: active
---

# Regulatory Watch

This file is the studio's living tracking surface for the regulations that govern EBDA Ventures and its portfolio. The studio's primary regulatory frame is **HIPAA + FDA** (US-focused per [[business-model]]); the secondary frame is **EU AI Act + MDR + GDPR** for any future EU expansion or EU LP exposure.

The file is intentionally light on detail per regulation — depth lives in the source materials and in the studio counsel's working files (once engaged per [[hiring-plan]]). What this file tracks: **what to watch, why it matters, how often to revisit, who owns the watch.**

## Owner

Current owner of regulatory watch: **Emilio**, supported by Ion (knowledge base updates) and Ion's `/ingest` skill when new guidance is published.

Future owner (post-hire): **studio counsel** + **clinical operating lead** (per [[hiring-plan]] Tier 1/2).

## Primary regulatory frame — US (HIPAA + FDA)

### HIPAA

**Why it matters:** Every EBDA portfolio company handling US patient data (PHI) is bound by HIPAA. Studio shared infrastructure (AI platform, EHR integrations, model monitoring) must be HIPAA-baseline by construction. A HIPAA enforcement action against any single portfolio company can ripple to the entire studio brand.

**What to watch:**
- HHS Office for Civil Rights (OCR) enforcement actions involving AI/ML systems
- HIPAA Privacy Rule modifications (reproductive health data treatment is actively evolving)
- HHS guidance on AI use in healthcare contexts under HIPAA
- 42 CFR Part 2 (substance use disorder records) — recent alignment with HIPAA changes scope
- BAA (Business Associate Agreement) template evolution

**Cadence:** Monthly review of HHS / OCR newsroom; ad-hoc on major enforcement actions.

**Sources:**
- HHS / OCR newsroom: https://www.hhs.gov/hipaa/index.html
- OCR enforcement settlements list
- Healthcare privacy law blogs (Hogan Lovells, Hall Render, Latham & Watkins)

### FDA AI/ML guidance

**Why it matters:** Many EBDA portfolio products will be regulated as Software-as-a-Medical-Device (SaMD) or Clinical Decision Support (CDS) tools. FDA's approach to AI/ML is the single biggest US regulatory question for healthcare AI. The list of AI-enabled medical devices is now a defined category per [[market-thesis]].

**What to watch:**
- FDA list of AI-enabled medical devices (periodic updates)
- Predetermined Change Control Plans (PCCPs) — FDA approach to evolving AI/ML models post-clearance
- Guidance on Clinical Decision Support (CDS) — the line between non-regulated CDS and regulated medical-device software
- Software Precertification (Pre-Cert) program evolution
- Total Product Life Cycle (TPLC) framework updates
- Generative AI / LLM-specific guidance (the most actively evolving area)

**Cadence:** Quarterly review of FDA Digital Health Center of Excellence; ad-hoc on major guidance releases.

**Sources:**
- FDA Digital Health Center of Excellence: https://www.fda.gov/medical-devices/digital-health-center-excellence
- FDA AI/ML in software as a medical device pages
- FDA AI-enabled medical device list (periodic updates)
- AdvaMed and CHAI (Coalition for Health AI) advocacy positions

## Secondary regulatory frame — EU (AI Act + MDR + GDPR)

### EU AI Act

**Why it matters:** Even with a US-primary focus per [[business-model]], the EU AI Act affects: (a) any future EU expansion of portfolio companies, (b) any EU-resident employees of the studio, (c) potentially the GP entity if EU-domiciled, and (d) deal-flow / hiring optics in EU markets.

**Status:** Entered into force August 2024 with phased implementation:
- February 2025: Prohibited AI practices apply
- August 2025: GPAI (general-purpose AI) obligations apply
- August 2026: High-risk AI system obligations apply (healthcare AI is largely high-risk)
- August 2027: Full applicability

**What to watch:**
- High-risk classification implementation (clinical AI = high-risk in most cases)
- Regulatory sandboxes for AI in healthcare (member-state level)
- Codes of practice for GPAI providers
- National competent authority designations per member state
- Interaction with EU MDR (overlap and divergence)

**Cadence:** Quarterly review; ad-hoc on guidance from European Commission AI Office.

**Sources:**
- European Commission AI Act portal
- European AI Office publications
- EU member-state competent authority bulletins (where any portfolio company operates)

### EU Medical Device Regulation (MDR)

**Why it matters:** MDR governs medical devices including SaMD across the EU. Has had significant capacity issues at Notified Bodies that affect timing for any EU launches.

**What to watch:**
- Notified Body capacity (historically a bottleneck)
- Class IIa / IIb / III classification rules for AI/ML SaMD
- Interaction with EU AI Act (especially for high-risk AI in medical devices — dual conformity assessment)
- Brexit equivalence / UK MHRA divergence

**Cadence:** Quarterly; deeper review if any portfolio company contemplates EU launch.

### GDPR + healthcare data

**Why it matters:** EU LPs may require GDPR-compliant data handling at the GP / ManCo level even if portfolio companies are US-only. Any EU-resident employee data is GDPR-bound.

**What to watch:**
- Data Protection Authority (DPA) enforcement actions involving healthcare data
- Standard Contractual Clauses (SCCs) updates for international transfers
- Schrems III equivalent decisions (US data-flow legal basis)
- Interaction with US Data Privacy Framework

**Cadence:** Semi-annual; ad-hoc on major DPA actions.

## State-level US regulatory layer

Several US states are layering their own healthcare-AI and data-privacy rules on top of HIPAA. Each portfolio company will need to track the states where it operates.

**Active state activity:**
- **California:** SB-1120 (LLMs / AI in healthcare decisions, 2024); SB-1223 (genetic data); CCPA/CPRA on health data; AB-3030 (AI disclosure)
- **Texas:** TDPSA (Texas Data Privacy & Security Act); pending AI-specific bills
- **Colorado:** Colorado AI Act (2024) — first US comprehensive AI law, takes effect Feb 2026
- **Washington:** My Health My Data Act (consumer health data, 2024)
- **New York:** SHIELD Act, expanding AI use rules in employment + healthcare
- **Illinois:** BIPA (biometric data — affects voice and imaging AI)

**Cadence:** Quarterly scan; per-portfolio-company watch once ventures operationally deploy.

**Source:** National Conference of State Legislatures health/AI tracking; healthcare privacy specialist law firms.

## Foundation-model vendor compliance

Because the [[studio-playbook]] commits to a maximalist shared AI platform that uses foundation models, vendor-level compliance posture is part of the regulatory surface:

**What to watch:**
- OpenAI, Anthropic, Google, Microsoft BAA availability and terms
- HIPAA-compliant deployment options (Azure OpenAI Service for Healthcare, Anthropic on AWS Bedrock with appropriate configuration, etc.)
- Vendor data-retention and training-use policies for healthcare data
- Foundation-model bias and accuracy disclosures relevant to clinical contexts

**Cadence:** Semi-annual review; ad-hoc on major vendor policy changes.

## How this file gets used

The intent is light:

1. **Monthly Ion check.** Ion scans HHS/OCR and EU AI Office for major updates; flags anything significant in `ops/inbox/`.
2. **Quarterly review.** Emilio + (eventually) studio counsel review this file; update status, add new tracked items.
3. **Ad-hoc deep dive.** When a portfolio company hits a regulatory question, use `/ingest` to digest the relevant guidance into specialized child files (e.g. `legal/fda-pccp-playbook.md`, `legal/eu-ai-act-high-risk-process.md`).
4. **Each portfolio company maintains its own regulatory file** post-spin-out; the studio file stays at the studio-relevant abstraction level.

## Open questions

- **In-house counsel vs. fractional vs. outside firm** — to be resolved with the studio counsel hire from [[hiring-plan]] Tier 2.
- **Specific specialist firms** to engage on retainer: US side (Goodwin / Cooley / K&L Gates / Sidley) for fund structuring; healthcare-specialist firms (Hall Render, Manatt, Polsinelli) for HIPAA / FDA work.
- **AI/ML SaMD pathway templates** — does the studio build standardized FDA pathway templates per disease vertical as part of shared infrastructure? Likely yes — should be added to [[studio-playbook]] when the clinical lead and studio counsel are both in place.
- **EU AI Act sandbox participation** — worth pursuing for any future EU portfolio company; not relevant for US-only Fund I focus.

## Related

- [[market-thesis]] — macro framing that includes the regulatory landscape
- [[business-model]] — US-primary geographic frame that drives HIPAA + FDA as primary
- [[studio-playbook]] — shared AI platform whose compliance posture is anchored in this file
- [[risks]] — regulatory risks (Top-3 risk #2's mitigations + dedicated regulatory risk category)
- [[hiring-plan]] — studio counsel hire (Tier 2) and clinical operating lead who own this file going forward
