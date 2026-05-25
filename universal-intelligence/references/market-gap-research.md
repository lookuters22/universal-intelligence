# Market Gap Research Loop

## Purpose

Find product and business ideas in less saturated territory by combining current research, adversarial doubt, and the UI wrong-road loop. Use for startup ideas, product strategy, monetizable wedges, competitor avoidance, market maps, and "unsaturated market" requests.

Goal: produce a high-conviction, testable opportunity. Never present market certainty as 100%; name confidence, counterevidence, the riskiest assumption, and the first validation probe.

## Trigger

Run this before Step 1 when the request includes products, startups, markets, niches, monetization, business ideas, competitors, market gaps, demand, saturation, distribution, pricing, or "what should we build?"

If current market facts matter and browsing tools are available, research live. If browsing is unavailable or the user forbids it, say the market read is stale/limited and turn the loop into assumptions plus validation tasks.

## Loop Contract

Complete at least two research passes:

1. **Terrain pass** - map the current alternatives.
2. **Doubt pass** - search against your own conclusion and try to kill each promising gap.
3. **Refusal layer** - route, narrow, rerun, or refuse the surviving candidate using `refusal-layer.md`.

Repeat the loop when the top candidate is generic, crowded, weakly painful, unbuyable, or only differentiated by branding.

Stop only when one of these is true:

- A candidate survives with specific segment, urgent pain, weak current workaround, plausible buyer, distribution wedge, counterevidence, kill criteria, and next validation probe.
- Evidence shows the arena is saturated or low-value; restart around a sharper user segment, narrower job, overlooked workflow, or adjacent market.
- The user asks to stop or choose from partial candidates.

## Terrain Pass

Gather evidence from current and adjacent sources:

- Competitors: product pages, pricing, changelogs, reviews, comparison pages, app stores, GitHub, marketplaces.
- Demand signals: forums, Reddit, Hacker News, Discord/Slack communities if available, review complaints, support threads, search trends, job posts, procurement language.
- Money signals: pricing pages, agency/service substitutes, paid templates, consultants, enterprise roles, compliance costs, manual labor budgets.
- Timing shifts: regulation, platform changes, AI capability shifts, data availability, distribution changes, macro pressure, new buyer urgency.
- Failure signals: shutdowns, stale repos, "why X failed" posts, low-retention complaints, feature parity races.

Prefer primary sources and fresh evidence. Cite links in user-facing market claims when the final answer contains factual assertions.

## Saturation Map

Before ideas, write a compact map:

| Cluster | Examples | Saturation read | Why users still suffer |
|---------|----------|-----------------|------------------------|
| Incumbents | named tools/companies | crowded / fragmented / thin / emerging | concrete unmet job |
| Substitutes | spreadsheets, agencies, scripts, internal ops | workaround strength | failure mode |
| Neglected segment | buyer/user group | why ignored | urgency/budget clue |

No "no competitors" fantasy. A useful gap is often a segment incumbents serve badly, not an empty desert.

## Gap Hypotheses

Generate 3-5 hypotheses. Each must include:

- **Segment**: who hurts, narrowly.
- **Job**: what they are trying to get done.
- **Current workaround**: how they solve it now.
- **Pain proof**: evidence, quote, pattern, or observable cost.
- **Why incumbents miss**: pricing, workflow mismatch, compliance, distribution, data access, trust, switching cost, ignored buyer, bad timing.
- **Wedge**: why this could enter before incumbents react.
- **UI dogma break**: which market assumption Step 1 should violate.

Reject candidates that are only "AI for X" or "better UX for X" unless the evidence proves a specific wedge.

## Doubt Pass

For every promising hypothesis, run hostile search:

- Search direct competitors: `best [job] software`, `[segment] [pain] startup`, `[pain] automation`, `[workflow] AI tool`, `[category] alternatives`.
- Search substitutes and open source: `[job] spreadsheet`, `[job] template`, `[job] github`, `[job] zapier`, `[job] consultant`.
- Search failure: `[category] failed startup`, `[tool] reviews`, `[pain] not worth paying`, `[category] churn`, `[category] shutdown`.
- Search buyer reality: `[segment] budget`, `[role] job description`, `[workflow] compliance`, `[category] procurement`.

Write the strongest reason the idea is bad. If the reason is decisive, kill or narrow the candidate. If it is not decisive, convert it into a risk, constraint, or validation probe.

## Survivor Ledger

Only carry survivors into the Evidence Refusal Layer when this ledger is explicit:

| Field | Requirement |
|-------|-------------|
| Candidate | one-sentence product/opportunity |
| Segment | narrow buyer/user, not a broad industry |
| Market gap | specific underserved job or workflow failure |
| Evidence for | source-backed demand/suffering/budget/timing signals |
| Evidence against | strongest saturation, substitute, adoption, or pricing threat |
| Confidence | low / medium / high, never certain |
| Rarest assumption | the single assumption most likely to break the idea |
| Kill criteria | what evidence would make you abandon it |
| First probe | cheapest test that can validate or kill in days |

After the ledger, run `refusal-layer.md`. Only a `ROUTE` decision may feed The Forest of Wrong. `NARROW`, `RERUN`, and `REFUSE` decisions stop routing and force the specified next action unless the user explicitly requests speculation despite the warning.

## Integration With UI

- Use the saturation map to feed **Dogma & Heresy Mapping** in `the-forest-of-wrong.md`.
- Make Garbage Exploratories violate saturated category logic, not random taste.
- In Friction Analysis, include buyer friction, adoption friction, market timing, and incumbent retaliation.
- In The Pivot, prefer the candidate with novelty payoff **and** a `ROUTE` decision after the refusal layer.
- In Refinement, ship a product concept with wedge, user segment, first validation test, kill criteria, and traceable evidence.

## Failure Modes

- Declaring a market unsaturated after one search.
- Treating absence of evidence as opportunity.
- Confusing "competitors are bad" with "buyers will switch."
- Selling a feature when the gap is distribution, trust, compliance, or budget.
- Averaging all candidates into generic SaaS.
- Claiming 100% certainty instead of high-conviction uncertainty with tests.
- Routing a candidate forward because it sounds exciting before it survives refusal.
