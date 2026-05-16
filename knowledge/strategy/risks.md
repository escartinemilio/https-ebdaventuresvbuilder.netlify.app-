---
title: Risks
description: What could kill or significantly damage EBDA Ventures — prioritized risk inventory across capital, competitive, regulatory, execution, founder, market, reputational, and technology categories
last_updated: 2026-05-16
updated_by: ion
status: active
---

# Risks

This file is the studio's honest risk inventory. It is intentionally pessimistic — the point of a risks file is to surface what could go wrong so it can be mitigated, not to reassure. Risks are prioritized into a **Top 3** (currently the most acute) and then catalogued by category.

This first version was drafted by Ion (2026-05-16) from the existing knowledge base and reviewed/approved by Emilio the same day. Future updates flow through the standard three-tier model.

## Top 3 risks — highest acute exposure

### 1. Fund I close failure (capital risk + structural gap)

**What:** EBDA Ventures cannot exist as a fund-backed studio without closing Fund I (EUR 20–50M). Without that capital, there is no studio operating budget, no shared AI platform investment, no ventures launched.

**Why it's #1:** The single largest risk converging from multiple structural factors:
- [[emilio]]'s LP network is predominantly European; the studio targets a US-domiciled fund with US LPs (see [[business-model]])
- First-time studio GP (Emilio has raised funds before but not for *this* vehicle / thesis)
- No anchor LP currently identified
- Fund I close typically takes 12–24 months for a first-time vehicle in this size range

**Mitigations to develop:**
- Resolve the US co-GP / placement agent question (top of [[hiring-plan]] *(planned)*)
- Build a documented anchor LP target list early (see [[capital-plan]] *(planned)*)
- Consider a smaller "seed" or "warehouse" structure to launch the first 1–2 ventures and create proof points before Fund I close
- Frame the European-founder / US-LP structure as a feature (transatlantic deal flow) rather than a bug — but only if backed by concrete US team additions

### 2. "AI-native" becomes table stakes faster than EBDA can prove it (positioning risk)

**What:** The primary wedge from [[positioning]] is **AI-native architecture** versus Redesign Health's workflow-native chassis. If by 2026–2027 every healthcare studio claims AI-native — and several already are pivoting in that direction — the wedge erodes before EBDA's first spin-out can validate it.

**Why it's #2:** This is the *thesis-decay* risk. The market window from [[market-thesis]] (roughly 2025–2028) means EBDA has to compound differentiation before competitors catch up.

**Mitigations to develop:**
- Build the shared AI platform as engineered reality, not slide deck (see [[studio-playbook]] *(planned)*)
- Publish technical specifications, blog posts, open-source components — make the claim verifiable
- Lead with portfolio proof points, not category claims, the moment first spin-outs ship
- Lock in defensible vendor relationships (foundation model commitments, EHR integration partnerships) before competitors do

### 3. Solo-founder bandwidth and key-person concentration (execution + founder risk)

**What:** [[emilio]] is currently the entire studio. Once Fund I closes, he cannot simultaneously: (a) run fund operations and LP reporting, (b) source/build 8–12 ventures, (c) recruit operating CEOs, (d) hold board seats across the portfolio, (e) develop US clinical and regulatory networks he doesn't currently have.

**Why it's #3:** This is structural and immediate. A solo founder can stand up a studio thesis; a solo founder cannot operate a studio at the pace and surface area Fund I requires. Sophisticated LPs will flag this in diligence as "key-person risk."

**Mitigations to develop:**
- Sequence hiring deliberately ([[hiring-plan]] *(planned)*): US head of healthcare → clinical advisory board → first EIRs in parallel with Fund I close
- Consider a US-based co-GP or co-founder explicitly (open question in [[business-model]])
- Document succession/key-person plan as part of the LP package
- Build the studio's operating playbook ([[studio-playbook]] *(planned)*) so it is institutional knowledge, not Emilio knowledge

---

## Other risks by category

### Capital

- **Anchor LP timing.** Even with a strong target list, anchor LP commitment timing is unpredictable. A delay of 6–9 months past target Fund I close pushes the entire venture pipeline back.
- **Macro funding cyclicality.** [[market-thesis]] notes 2025 was a strong year (+35% YoY for digital health). 2026–2027 funding could cool. If it does, both Fund I and portfolio follow-on rounds get harder simultaneously.
- **GP commitment liquidity.** Standard fund structures require the GP to commit 1–2% of the fund. For a EUR 20–50M fund this is EUR 200K–1M of personal capital — non-trivial.
- **Reserve policy.** If Fund I doesn't hold sufficient reserves for follow-on rounds in winners, the studio loses pro-rata in the most valuable spin-outs.

### Competitive

- **Redesign Health repositions and outspends on AI-native marketing.** Redesign has the resources to rebrand and outspend EBDA on category messaging — even if its underlying tech is the same workflow chassis.
- **GC Health Assurance or a16z launches a competing studio.** Either has the capital and brand to compress the market window from years to quarters.
- **A new AI-native studio enters with a US founder.** Removes EBDA's geographic disadvantage from the comparison without giving up the AI-native wedge.
- **Vertical-focused single-disease studios** (e.g. an oncology-only AI studio) attack EBDA's four disease verticals one at a time with more depth.

### Regulatory

- **FDA AI/ML guidance shift mid-build.** The FDA AI-enabled medical-device list is evolving. A guidance change could invalidate a portfolio company's regulatory pathway after substantial investment.
- **HIPAA enforcement on AI/ML inference.** Specifically, treatment of PHI in foundation-model context windows is unsettled. An enforcement action against any healthcare AI company could ripple to the portfolio.
- **EU AI Act high-risk classification.** If EBDA later expands portfolio companies into EU, high-risk classification adds 12–18 months and material cost per product. Mitigation: don't bake EU expansion into Fund I plans.
- **State-level data residency.** Texas, California, and others are layering additional healthcare AI rules. Compliance overhead per spin-out grows.
- **Reimbursement uncertainty.** Most AI workflow tools do not yet have dedicated CPT codes. If reimbursement evolves slowly, unit economics on provider-facing tools stay weaker than expected.

### Execution / operating

- **Pace of launch.** 8–12 ventures in Fund I (~2.5 ventures/year for a 4-year deployment) is aggressive for an unproven studio. Slipping to 5–6 ventures hurts both fund returns and Fund II positioning.
- **Operator-CEO recruitment.** EBDA needs A-tier operating CEOs in the US healthcare market, where the studio has no network. The 35–55% studio stake is operator-friendly compared to Atomic but operator-unfriendly compared to founding solo.
- **Clinical advisor network development.** Without strong US clinical advisors per disease vertical, spin-outs cannot run pilots, cannot get clinical validation, and cannot sell into health systems.
- **Shared AI platform engineering.** Building genuinely useful shared infrastructure (not just slide deck infrastructure) requires senior engineering leadership the studio has not yet hired.
- **Cross-portfolio cannibalization.** Two portfolio companies in adjacent spaces (e.g. two cardio-AI ventures) may end up competing for the same pilots, same talent, same KOLs.

### Portfolio concentration

- **Disease-vertical concentration.** If one of the four verticals (cardio, obesity, women's, oncology) sees a category downturn or regulatory shock, fund is materially exposed.
- **AI Healthcare Copilots commoditization.** If the horizontal Copilots layer commoditizes faster than the disease-vertical ventures mature, half the thesis erodes.
- **Foundation-model vendor dependency.** Heavy reliance on a single foundation model vendor (OpenAI, Anthropic, Google) creates platform risk if pricing, terms, or access change.

### Founder / key-person

- **Health / bandwidth.** [[emilio]] is the sole keeper of the studio's fundraising capability. Any health or availability disruption is existential to Fund I close.
- **Succession.** No documented succession plan currently exists.
- **EU residency / time zones.** Operating a US-focused studio from a European time zone limits real-time engagement with US LPs and portfolio operations.
- **Bus factor on the AI/clinical side.** The studio currently has *zero* permanent capacity in clinical or AI execution — every key skill is to-be-hired. Until those hires close, the founder risk extends to "the studio has no shipping capability."

### Market / macro

- **AI healthcare funding cycle reversal.** [[market-thesis]] Rock Health 2025 data could be peak. If 2026–2027 funding cools, both Fund I and portfolio follow-ons get harder.
- **US political / HHS shift.** A material shift in HHS leadership or Medicare AI policy could change the demand landscape on a 12-month timescale.
- **Provider buying-cycle elongation.** Health systems' AI procurement cycles are notoriously long (12–24 months); if they elongate further, portfolio companies burn cash through extended pilot phases.

### Reputational / trust

- **First spin-out failure brands the studio.** Early visibility means the first one or two ventures define EBDA's reputation regardless of fund-level performance.
- **Clinical AI safety incident in portfolio.** A patient-safety incident at any portfolio company (false negative diagnosis, hallucinated dosing recommendation, etc.) damages the entire portfolio and the studio brand. Healthcare buyers have long memories.
- **Founder reputation transferability.** Emilio's PE/VC reputation is European; in the US healthcare-investor community, the studio starts from near-zero brand equity.

### Technology

- **Foundation model commoditization or vendor lock.** Either direction is a risk: commoditization erodes the shared platform's value; vendor lock creates pricing exposure.
- **Open-source model parity.** If open-source clinical models reach quality parity by 2027, proprietary AI infrastructure becomes harder to defend as a wedge.
- **Hallucination and bias floors.** Clinical accuracy requirements may exceed what current foundation models can deliver in some verticals, limiting addressable use cases per spin-out.

## What this risk inventory implies for the immediate roadmap

Looking across the Top 3 and category list, three actions follow:

1. **Close the EU→US gap structurally** before serious LP outreach: US co-GP / advisory / hiring decisions are gating.
2. **Build the AI platform as engineered reality** in parallel with Fund I fundraising — so the positioning wedge is verifiable by the time LPs do technical diligence.
3. **Document the studio playbook** ([[studio-playbook]] *(planned)*) so the operation becomes institutional rather than founder-resident — directly addresses the key-person risk.

These three priorities should flow into [[hiring-plan]], [[capital-plan]], and the product/ layer.

## Related

- [[vision]] — the thesis these risks could damage
- [[business-model]] — capital structure and EU→US gap that drive risks 1 and 3
- [[positioning]] — wedge whose erosion is risk 2
- [[emilio]] — founder profile underlying the key-person risk
- [[market-thesis]] — macro context whose reversal is a category-level risk
- [[hiring-plan]] *(planned)* — primary mitigation surface for risks 1 and 3
- [[studio-playbook]] *(planned)* — primary mitigation surface for risks 2 and 3
- [[capital-plan]] *(planned)* — concrete Fund I path that directly addresses risk 1
