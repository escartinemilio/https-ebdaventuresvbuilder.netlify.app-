---
title: Studio Playbook
description: How EBDA Ventures operates — idea origination, incubation lifecycle, shared AI infrastructure, and spin-out mechanics
last_updated: 2026-05-16
updated_by: ion
status: active
---

# Studio Playbook

This is the operating manual for EBDA Ventures itself. It defines how the studio takes an opportunity from disease-thesis to spun-out company. The playbook has three load-bearing decisions:

| Decision | Choice | Why |
|---|---|---|
| Idea origination | **Hybrid — studio sets disease theses; EIRs co-design ventures** | Preserves [[vision]]'s curatorial discipline (cardio/obesity/women's/cancer) while giving operating CEOs real ownership of the venture they'll run |
| Incubation length | **6–12 months per venture** | Healthcare needs clinical validation, regulatory pathway design, and first pilot site before spin-out; software-only fast-launch (3 months) is too short for clinical AI |
| Shared AI infrastructure | **Maximalist — build a real AI platform** | The "AI-native" wedge from [[positioning]] is verifiable engineering, not slide deck. The shared platform IS the differentiator. |

The three decisions are mutually reinforcing. A hybrid origination model only works if the studio has a credible disease thesis (so the maximalist AI platform earns its weight). A 6–12 month incubation only works if shared infrastructure absorbs the heavy lifting (otherwise pace collapses). And a maximalist AI platform only earns its cost if it serves many ventures (so the hybrid origination model must produce a credible launch cadence).

## Idea origination

EBDA does not source ideas opportunistically. It runs a **two-layer origination funnel**:

**Layer 1 — Studio sets disease theses.** Within each of the four disease verticals (cardio, obesity, women's, oncology) plus the AI Copilots horizontal, the studio team — Emilio + clinical advisory board + AI engineering leadership — maintains an active *opportunity map*: which workflows are most painful, which buyer segments are most addressable, which AI capabilities are now production-grade for that vertical. This map is the studio's curatorial layer.

**Layer 2 — EIRs co-design specific ventures.** The studio recruits founders-in-residence (EIRs) into a thesis area. The EIR + studio team co-design the actual venture: ICP, product, technical architecture, go-to-market motion. The EIR owns the venture they'll later run as CEO. This preserves operator-grade equity ([[business-model]]) while keeping thesis discipline.

**What this rules out:**
- Pure opportunistic deal-flow ("we saw a great founder, let's back them") — that's a VC, not a studio
- Pure studio-internal design ("we have an idea, go find a CEO") — that produces ventures with weak operator commitment
- Open-call founder programs ("apply to our studio") — wrong shape for healthcare, where deep clinical context per founder is required

## Incubation lifecycle (6–12 months, in phases)

The lifecycle is structured in four phases. The exact duration of each varies by venture, but the *gates between phases* are non-negotiable: a venture cannot advance until the gate is met, and the studio can elect to kill the venture at any gate.

### Phase 1 — Discovery (4–8 weeks)

**Goal:** Validate the disease/workflow thesis and confirm the venture is worth incubating.

**Activities:**
- 15–30 expert interviews (clinicians, payors, health-system buyers, KOLs)
- Competitive map within the workflow target
- Initial technical feasibility: which AI capabilities exist, which need to be built
- Regulatory pathway scoping (FDA AI/ML applicability, HIPAA posture)
- Initial economic model: TAM, willingness-to-pay, sales-cycle assumptions

**Gate to Phase 2:** Studio investment committee (Emilio + clinical lead + AI lead) approves continued investment based on a written investment memo. Roughly 30–50% of Discovery-phase candidates are expected to fail this gate — that's the point.

### Phase 2 — Validation (8–16 weeks)

**Goal:** Build a working prototype; get it in front of real clinical users; secure a Letter of Intent (LOI) from at least one pilot site.

**Activities:**
- EIR onboarded as committed founder/CEO candidate
- Working AI prototype built using shared platform components
- 2–4 user-validation sessions at real clinical sites
- LOI negotiation with first pilot site
- Initial team plan: which roles, which timing, which equity grants
- Regulatory pathway confirmed; compliance posture documented

**Gate to Phase 3:** Signed LOI with at least one credible pilot site + EIR formal commitment to be CEO + investment committee approval to fund Phase 3.

### Phase 3 — Build & Pilot (12–24 weeks)

**Goal:** Ship the production-grade product; run the first paid or paid-equivalent pilot; demonstrate measurable ROI in line with [[vision]]'s selection rule (hours saved, revenue recovered, claims processed, etc.).

**Activities:**
- Production engineering on the venture's vertical-specific product (built on the shared AI platform)
- Pilot execution at first site; structured measurement of clinical/operational KPIs
- Founding team hires (typically 3–6 people: CTO, clinical lead, GTM lead, ML engineers)
- Pricing model finalized; second pilot site in discussion
- Initial fundraise narrative prepared for spin-out round

**Gate to Phase 4:** Pilot ROI demonstrated (or credible early signal); founding team in place; spin-out documents drafted; capitalization table modeled.

### Phase 4 — Spin-out (4–6 weeks)

**Goal:** Formal company formation, first external capital round, transition from studio to standalone operating entity.

**Activities:**
- Legal incorporation (Delaware C-Corp default)
- Studio takes 35–55% equity per [[business-model]]; balance allocated to founding team
- Cap table finalized; ESOP established (typically 10–15%)
- Seed round closed (studio + external co-investors)
- Board formed (studio + CEO + independent director)
- Spin-out company assumes its own commercial agreements

**Post spin-out:** Studio remains as largest shareholder and board member; provides ongoing portfolio support but no longer drives day-to-day operations.

## Shared AI platform — scope and intent

**Owner of platform spec:** TBD (to be filled by senior AI/ML engineering leader hire — see [[hiring-plan]] *(planned)*). This section is the intended scope; the production spec is v0.1 pending that hire.

The shared AI platform is the **single largest investment** the studio makes outside of individual venture funding. It exists because the "AI-native" positioning ([[positioning]]) is only credible if every spin-out genuinely inherits production-grade AI infrastructure.

### What the platform provides

**Agentic and conversational layer**
- Pre-built agent scaffolding with healthcare-appropriate guardrails
- Voice interface infrastructure for clinical use cases (intake, dictation, patient communication)
- Conversational orchestration framework — multi-turn, role-aware, audit-logged

**Retrieval and knowledge management**
- Shared RAG infrastructure with healthcare-tuned embedding and chunking strategies
- Pre-integrated clinical knowledge sources (where licensed): drug interactions, ICD-10, CPT, SNOMED, common clinical guidelines
- Per-venture private knowledge layer for proprietary data

**Clinical documentation**
- Ambient documentation primitives (audio capture → structured notes)
- SOAP-note templating, billing-code suggestion scaffolding
- HIPAA-compliant transcription pipeline

**Integration layer**
- Pre-built EHR integration adapters (Epic, Cerner/Oracle, athenahealth, eClinicalWorks at minimum)
- CRM and billing-system integrations (Salesforce Health Cloud, scheduling tools)
- Standard FHIR-based interfaces

**Compliance, monitoring, auditability**
- HIPAA-baseline data handling: encryption, access controls, BAA templates
- Foundation-model audit logging (every inference logged with input/output/model version)
- Bias and accuracy monitoring scaffolding (per the FDA AI/ML guidance direction)
- Incident response runbook templates

**Foundation model and vendor management**
- Studio-level commercial relationships with OpenAI, Anthropic, Google, and selected open-source providers
- Negotiated pricing benefiting the portfolio
- Model-routing infrastructure (each venture picks models per use case; routing is shared)

### What the platform does NOT provide

Each venture builds its own:
- Disease-specific product surface and clinical workflow
- Vertical-specific data labeling, fine-tuning, evaluation harnesses
- Customer-facing brand, UI/UX, marketing

The split is: **horizontal AI infrastructure is shared; vertical product is owned by the venture.**

### Why "maximalist" and not "selective"

The selective alternative ("share what's hard, let ventures build the rest") seems cheaper but is strategically wrong for EBDA:

- If the AI platform is thin, the studio is essentially a healthcare incubator with shared legal — competitors do that already
- The platform IS the wedge. Underinvesting in it undermines [[positioning]] and aligns with Top 3 risk #2 from [[risks]] ("AI-native becomes table stakes faster than EBDA can prove it")
- The maximalist platform is what justifies the studio's 35–55% equity stake to operating CEOs — they're getting real infrastructure, not just legal docs

The platform is a defensible cost only if the launch cadence is high enough to amortize it (8–12 ventures in Fund I makes this work, per [[business-model]]).

## Shared non-AI infrastructure

In addition to the AI platform, the studio provides each venture with:

- **Legal and regulatory scaffolding:** standardized incorporation, BAA templates, HIPAA baseline, FDA AI/ML pathway templates, employment agreements, advisor agreements, IP assignment
- **Clinical advisory network:** shared per-vertical clinical advisory boards; introductions to KOLs and pilot sites
- **Go-to-market motion:** shared playbook for health-system selling, including procurement navigation, IT-security questionnaires, value-analysis-committee preparation
- **Recruiting:** shared talent network for clinical, engineering, GTM hires
- **Finance & operations:** shared accounting, payroll, HR backbone during incubation; transitions to standalone post spin-out
- **Brand and PR:** shared launch playbook; spin-outs benefit from EBDA Ventures portfolio branding

## Studio operating cadence

- **Quarterly:** Studio-level investment committee reviews all in-flight ventures against phase gates; kill / continue / accelerate decisions made
- **Monthly:** Per-venture operating reviews
- **Weekly:** Studio leadership standup; cross-venture issue surfacing
- **Daily:** Per-venture EIR + studio embed standup during active build phases

This cadence is operationally heavy and is part of why solo-founder bandwidth is Top 3 risk #3 in [[risks]]. The cadence cannot be Emilio-only.

## Implications for hiring (deferred to [[hiring-plan]] *(planned)*)

The playbook as written requires, at minimum:
- Senior AI/ML engineering leader (owns the shared AI platform spec and build)
- US-based clinical operating lead (manages clinical advisory boards across the four verticals)
- Head of platform engineering (builds and maintains EHR integrations, compliance, monitoring)
- 2–3 EIRs in pipeline at any time (so Phase 1 Discovery has candidates)
- Operating support: finance/legal/HR

These hires gate the playbook's execution. They should be sequenced and budgeted in [[hiring-plan]] and reflected in [[capital-plan]].

## Open questions

- **Per-venture incubation budget cap.** What's the spend ceiling per venture across Phases 1–3 before spin-out? Drives Fund I deployment pace.
- **Kill rate target.** What % of Discovery-phase candidates should die at the gate? Industry norm is 50%+. Too low = studio is rubber-stamping; too high = origination is wasteful.
- **Pilot economics during Phase 3.** Free pilots, paid pilots, or pilot-with-credits? Healthcare buyer expectation varies.
- **Post-spin-out studio service offering.** Does the studio continue to provide ongoing AI platform services to spin-outs (paid? at-cost? free?), or do they fork their own infrastructure at spin-out?
- **Cross-portfolio coordination.** When two ventures need adjacent capabilities, who arbitrates? Studio? CEOs?

## Related

- [[vision]] — the studio thesis this playbook executes
- [[business-model]] — the fund + equity structure that funds the playbook
- [[positioning]] — the AI-native wedge this playbook makes real
- [[risks]] — Top 3 risks #2 and #3 are directly addressed by this playbook
- [[emilio]] — founder whose bandwidth limits the playbook's pace
- [[hiring-plan]] *(planned)* — the hires required to execute this playbook at pace
- [[capital-plan]] *(planned)* — the budget required to build the AI platform + sustain the cadence
- [[regulatory-watch]] *(planned)* — FDA AI/ML and HIPAA tracking that feeds platform compliance updates
