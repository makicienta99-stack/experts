# GES M&A Expert Agents: User Guide

The 15 most important M&A roles from [ma-expert-roles.md](ma-expert-roles.md) are built as **Claude Code subagents** in [`.claude/agents/`](../.claude/agents/). Each agent reads [ges-company-research.md](ges-company-research.md) first, so it starts with GES context.

Docs: https://code.claude.com/docs/en/sub-agents

## The team

| # | Agent | Area | Use it for |
|---|---|---|---|
| 1 | `corp-dev-director` | Deal lead | Framing a deal, running the process, IC memo, go/no-go |
| 2 | `pe-operating-partner` | Sponsor view | Does this create value for Truelink? Exit story |
| 3 | `investment-banker` | Deal advisory | Price range, earn-outs, LOI terms, negotiation |
| 4 | `deal-sourcing-analyst` | Sourcing | Finding and screening targets, competitor tracking |
| 5 | `valuation-analyst` | Finance | Multiples, DCF, returns, max price |
| 6 | `qoe-accountant` | Finance | Normalized EBITDA, revenue quality, working capital |
| 7 | `synergy-analyst` | Finance | Cross-sell and cost synergies, margin accretion |
| 8 | `ma-tax-advisor` | Tax | Deal structure, cross-border tax, tax risks |
| 9 | `ma-attorney` | Legal | Purchase agreement terms, show and venue contract change-of-control |
| 10 | `antitrust-counsel` | Legal | HSR, EU and UK filings, competitor overlap |
| 11 | `labor-employment-attorney` | Legal | Unions, pension withdrawal liability, retention, TUPE |
| 12 | `trade-show-industry-expert` | Industry | Show contracts, rotation, venues, competitor reaction |
| 13 | `experiential-agency-expert` | Industry | Agency targets (Spiro, 2Heads, CSG models) |
| 14 | `event-tech-expert` | Industry | Event-tech targets for Event Intelligence |
| 15 | `integration-lead` | Post-close | Day 1, 100-day plan, KPIs |

## How to use them

Open Claude Code in this repository. The agents load automatically (check with `/agents`).

**Let Claude pick the expert:**
> Evaluate acquiring a 40-person experiential agency in Munich with $18M revenue for Spiro.

**Call a specific expert:**
> Use the antitrust-counsel agent to check whether buying a regional trade-show contractor in Texas needs an HSR filing.

You can also @-mention an agent in your message.

**Run a full deal review.** Subagents can't call other subagents, so the main session coordinates them:
> Use corp-dev-director to frame the CSG-style deal for [Target], then run valuation-analyst, ma-attorney, trade-show-industry-expert and synergy-analyst in parallel, then have corp-dev-director write the IC memo.

**Make the deal lead your main session:**

```bash
claude --agent corp-dev-director
```

## Customizing
- Edit any `.claude/agents/*.md` file to change an agent's instructions, tools, `model` or `color`.
- Add target data (P&Ls, contracts) to a `deals/<target-name>/` folder and point agents at it.

## Important
These agents provide **decision support**. They are not a substitute for licensed legal, tax, accounting or investment professionals, who must sign off on real transactions. Keep confidential deal data out of public repositories.
