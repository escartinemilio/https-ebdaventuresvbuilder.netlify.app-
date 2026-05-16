---
title: Changelog
description: Append-only log of every change made to knowledge files
last_updated: 2026-04-06
updated_by: system
status: active
---

# Changelog

> Append-only. Ion writes here after every knowledge modification using a parseable format.
>
> Format: `## [YYYY-MM-DD] <action> | <subject>` followed by a one-line reason and `— by: <name>`.
>
> Greppable: `grep "^## \[" ops/changelog.md | tail -10`

## [2026-04-06] created | ion/state.md
Initial template scaffold from /bootstrap.
— by: system

## [2026-04-07] bootstrap | ops/inbox/, sources/
v1.1 additions: source ingestion layer, frictionless capture inbox, parseable log format, custom skill creation.
— by: ion

## [2026-05-16] bootstrap | knowledge/ structure for EBDA Ventures (company mode)
Provisioned 9 knowledge subfolders (strategy, product, customers, financials, legal, team, intelligence, decisions, meetings) with READMEs. Set partner = Emilio Escartin, mode = company. State.md and identity.md populated.
— by: ion

## [2026-05-16] created | strategy/vision.md, team/emilio.md, intelligence/market-thesis.md
First /interview round captured: studio thesis (30–35 AI Healthcare companies; cardio/obesity/women's/cancer + Copilots), founder bio (30+ yrs PE/VC, ~20 funds, €1B+ AUM), and macro evidence (WHO 2030, Peterson $350B, McKinsey adoption, Rock Health 2025, FDA AI list, EU AI Act). Parent READMEs and state.md updated; open questions list refreshed.
— by: ion

## [2026-05-16] created | strategy/business-model.md
Second /interview round: fund-backed studio (GP/LP), EUR 20–50M Fund I funding ~8–12 ventures, 35–55% studio equity at formation, US-primary geography (HIPAA/FDA), 30–35 ventures reframed as multi-fund lifetime target. Surfaced central strategic challenge: European founder, US-focused studio — requires US co-GP/advisors/team. Open questions list refreshed in state.md.
— by: ion

## [2026-05-16] created | strategy/positioning.md
Third /interview round: primary comparable = Redesign Health; primary wedge = AI-native architecture vs Redesign's workflow-native chassis; supporting wedges = disease-vertical focus (cardio/obesity/women's/cancer) + operator-friendly equity (35–55% vs heavy-studio 70–80%). Honest weakness flagged: EBDA is smaller, newer, less-networked than Redesign; must win on sharpness not scale. Strategy layer substantially complete.
— by: ion

## [2026-05-16] created | strategy/risks.md
Fourth /interview round: Ion-drafted risk inventory pending Emilio validation. Top 3: (1) Fund I close failure (EU→US LP gap converging with first-time-studio-GP timing), (2) "AI-native" wedge commoditizing before EBDA proves it, (3) solo-founder bandwidth + key-person risk. Full catalog across capital, competitive, regulatory, execution, portfolio-concentration, founder, market, reputational, and technology categories. Strategy layer (vision/business-model/positioning/risks) now complete.
— by: ion

## [2026-05-16] updated | strategy/risks.md, ops/action-items.md
Emilio validated risks.md as written — Top 3 and full inventory approved without edits. Risk mitigations promoted into ops/action-items.md as living checklist (gating Fund I + gating spin-out launch + knowledge-base continuation).
— by: ion

## [2026-05-16] created | product/studio-playbook.md
Fifth /interview round: operating manual for the studio. Three load-bearing decisions captured — (1) hybrid idea origination (studio sets disease theses; EIRs co-design ventures), (2) 6–12 month four-phase incubation lifecycle (Discovery → Validation → Build & Pilot → Spin-out) with gates between phases, (3) maximalist shared AI platform (agentic/RAG/voice/clinical-docs/EHR/compliance/foundation-model layers). Pace math reconciles: ~2 launches/year × 4-year deployment = 8 ventures in Fund I, matching [[business-model]]. Playbook intensifies hiring urgency (senior AI/ML lead + clinical operating lead) before pace is achievable.
— by: ion

## [2026-05-16] created | team/hiring-plan.md + updated state.md, action-items.md
Sixth /interview round: back-calculated hiring plan from Q2 2027 Fund I first close. Resolved sole-GP question (no US co-GP; substitute = load-bearing US advisory board + US healthcare-specialist placement agent). Tier 1 sequence: AI/ML lead Q3 2026 → clinical lead Q4 2026 → head of platform Q4 2026 → US MD Q1 2027 → COO Q1 2027. Geographic policy: US-mandatory for clinical/MD, flexible for AI/ML. Surfaced new most-urgent open question: pre-Fund I funding (~EUR 2–4M for 12 months of Tier 1 hires) — gates entire hiring sequence. action-items.md and state.md refreshed accordingly.
— by: ion

## [2026-05-16] created | financials/capital-plan.md + updated state.md, action-items.md
Seventh /interview round: closes the Fund I narrative loop. Pre-Fund I funding resolved (Emilio personal capital, ~EUR 2–4M, credited to GP commitment). Fund I anchor LP target = family office with healthcare allocation (faster cycle than institutional; matches Emilio's network strengths); HNW syndicate behind; optional strategics. Proposed fund terms: 2/20, 8% hurdle, European waterfall, key-person provision required. Entity structure proposal: Delaware LP + Cayman feeder + Spain/Lux ManCo (pending specialist confirmation). Detailed pre-Fund I use-of-funds breakdown, base + slip + headwind scenarios. Whole studio thesis now internally consistent and operationally specified: strategy → operating model → team build → capital → timeline.
— by: ion

## [2026-05-16] created | customers/segments.md
Eighth /interview round: two customer surfaces formalized. Surface A (clinical buyers) = provider-side primary (IDNs, AMCs, specialty clinic chains, community hospitals, physician groups) with payor/employer/pharma as secondary per-venture options. Surface B (LPs) = personas formalized from [[capital-plan]] plus three anticipated LP objections with prepared answers (first-time studio / European founder US gap / why-not-Redesign). Cross-surface coordination noted: provider reference customers become LP proof points; LP strategics can become portfolio customers.
— by: ion

## [2026-05-16] created | legal/regulatory-watch.md
Ninth /interview round: scaffolding for ongoing regulatory tracking. Primary frame = HIPAA + FDA AI/ML (US-focused per [[business-model]]); secondary frame = EU AI Act + MDR + GDPR (for EU LP and future EU expansion). State-level US layer tracked (CA SB-1120, CO AI Act, TX TDPSA, WA My Health My Data, IL BIPA, NY SHIELD). Foundation-model vendor compliance included. Cadence, owners, and sources specified per area. /interview substantively complete.
— by: ion
