# Expert Roles for a GES M&A Decision-Support Application

*Compiled November 26, 2026 · Companion to [ges-company-research.md](ges-company-research.md)*

This is the full list of expert roles needed to build a world-class M&A application for GES (Global Experience Specialists). You don't need to hire most of them full-time. Interview them to capture their judgment, then turn it into the app's scoring models, checklists and workflows. The 15 starred (★) roles are built as Claude Code agents in [`.claude/agents/`](../.claude/agents/). See [ma-agents-guide.md](ma-agents-guide.md).

## 1. M&A and deal strategy

| Role | Why GES needs it | What it adds to the app |
|---|---|---|
| ★ Corporate development / M&A director | Runs GES's buy-and-build process day to day | Deal stages, pipeline workflow, decision gates, investment committee memo |
| ★ Private equity operating partner | Truelink owns GES and plans an exit in about 4–6 years | Thesis-fit scoring, exit-value logic, sponsor reporting |
| ★ Investment banker / M&A advisor | Knows how founder-owned agencies and contractors are priced | Valuation ranges, deal structures (earn-outs, rollover), negotiation milestones |
| ★ Deal sourcing analyst | Targets are small, private and hard to find | Target database, enrichment, outreach tracking |

## 2. Finance and valuation

| Role | Why | App contribution |
|---|---|---|
| ★ Financial modeling / valuation analyst | Fast "what is it worth?" answers | Multiples, discounted cash flow and comparable-deal models |
| ★ Quality of earnings accountant | Small agencies have messy books and owner add-backs | Earnings-adjustment checklist, red flags |
| ★ Synergy and accretion analyst | Does the deal lift GES's thin blended margin? | Synergy tracker, margin-mix effect |
| ★ Tax advisor (M&A, international) | Deals in the UK, France, Middle East and India | Share vs. asset structure, cross-border tax flags |
| Leveraged finance / treasury specialist | PE acquisition debt has loan limits | Debt capacity and covenant checks |
| FP&A lead | Connects deals to the budget | Post-close performance vs. plan |

## 3. Legal and compliance

| Role | Why | App contribution |
|---|---|---|
| ★ M&A transactional attorney | NDA, LOI, purchase agreement, contract change-of-control clauses | Templates, key-terms tracker, clause library |
| ★ Antitrust / competition counsel | Buying direct rivals may trigger regulator review | Filing flags (U.S. HSR, EU, UK), market-overlap analysis |
| ★ Employment and labor attorney | Unionized trade-show labor and key-person retention | Union contract and retention checklists |
| Commercial contracts attorney | Value sits in multi-year show and venue contracts | Contract inventory (folded into the M&A attorney agent) |
| International counsel (EMEA, GCC, India) | Expansion into France, Qatar, Dubai, India | Country checklists |
| Data privacy counsel | Event-tech targets hold attendee personal data | Privacy diligence (folded into the event tech agent) |
| IP attorney | Creative and software IP | IP ownership checklist |

## 4. Live events industry (GES-specific)

| Role | Why | App contribution |
|---|---|---|
| ★ Trade show / exhibition industry veteran | Players, show rotation, venues, labor | Industry data fields, show-contract risk |
| ★ Experiential agency expert | Spiro, 2Heads and CSG are agencies | Agency scoring (client concentration, talent dependency) |
| ★ Event technology expert | The new "Event Intelligence" strategy | Event-tech scoring (recurring revenue, data, privacy) |
| Association / show organizer advisor | Organizers are GES's main buyers | Cross-sell scoring |
| Event logistics and freight expert | Logistics is part of Truelink's thesis | Logistics diligence |
| International market specialist | Geographic expansion priority | Market-entry scoring |

## 5. Due diligence specialists
Commercial DD consultant, operational DD expert, IT and cybersecurity DD expert, HR and culture DD specialist, ESG analyst, insurance and risk advisor.

## 6. Post-merger integration

| Role | Why | App contribution |
|---|---|---|
| ★ Integration management lead | Turns signed deals into results; GES keeps acquired brands standalone | 100-day plans, retention and earn-out tracker, cross-sell tracker |
| Change management / HR integration lead | Founder retention | Retention plans |
| Sales integration / cross-sell lead | Most of the deal value is cross-selling | Cross-sell pipeline |
| Systems integration lead | ERP and CRM migration | Migration checklist |

## 7. Data, analytics and AI
Data analyst / BI developer, data engineer, data scientist / ML engineer, competitive intelligence analyst (★ partly covered by the deal sourcing agent).

## 8. Product and technology (to build the app)
Product manager, UX/UI designer, software engineers, solutions architect, security engineer, QA engineer, DevOps engineer.

## 9. Governance and end users
Executive sponsor (GES CEO/CFO), Truelink board / investment committee representative, deal administrator, information security and compliance officer.

## Lean starting team
1. Corporate development / M&A director
2. Valuation analyst
3. M&A attorney (plus antitrust counsel when needed)
4. Trade show industry veteran
5. PE operating partner advisor
6. Product manager
7. Full-stack engineer and data engineer
8. UX designer
