# Universal Intelligence Codex Skill

Universal Intelligence is a Codex skill for building stronger product ideas, market-gap hypotheses, and creative strategies without drifting into generic "sounds good" answers.

It combines two modes:

- **Market-gap precision**: research current alternatives, map saturation, doubt the findings, and refuse weak ideas before brainstorming begins.
- **Wrong-road invention**: deliberately generate strange but inspectable exploratory passes, analyze their friction, quarry the useful shard, and refine it into a usable result.

The skill is built for moments where ordinary best-practice answers are too flat: unsaturated market discovery, startup/product ideas, product strategy, positioning, UX direction, architecture forks, naming, process design, critique, and other creative or diagnostic work where the first obvious answer is probably not enough.

## Why This Exists

Most AI brainstorming produces polished median output. It can sound confident while quietly averaging the same visible patterns everyone else can ask for.

Universal Intelligence pushes against that in two ways:

1. **It refuses market delusion first.** Product ideas must survive evidence, counterevidence, saturation pressure, buyer reality, and a routing decision.
2. **It keeps weird exploration inspectable.** Wrong ideas are not used as decoration. They become reviewable raw material for discovering a non-obvious mechanism.

The goal is not fake certainty or novelty theater. The goal is a high-conviction, testable direction with visible reasoning, kill criteria, and a first validation probe.

## Product And Market Workflow

For product, startup, business, monetization, competitor, or unsaturated-market requests, the skill runs a pre-flight evidence loop before ideation.

### 1. Market Gap Research

The skill maps the current terrain:

- named incumbents and direct competitors
- substitutes such as spreadsheets, agencies, scripts, templates, or internal labor
- demand signals from reviews, forums, job posts, support threads, communities, and procurement language
- money signals such as pricing pages, paid services, compliance costs, and labor budgets
- timing shifts such as platform changes, regulation, new data availability, or AI capability changes
- failure signals such as stale tools, shutdowns, churn complaints, or "why this failed" evidence

The output is not allowed to pretend "no competitors" means opportunity. A real gap is usually a specific segment or workflow that existing alternatives serve badly.

### 2. Doubt Pass

The skill then attacks its own promising finding:

- searches for direct competitors and alternatives
- checks open-source, templates, service businesses, and manual workarounds
- looks for failed startups, poor retention signals, and reasons users may not pay
- asks whether the problem is actually product, distribution, trust, compliance, data access, or budget

Weak ideas are killed or narrowed before they become brainstorming fuel.

### 3. Evidence Refusal Layer

Every product candidate must receive exactly one routing decision:

| Decision | Meaning | Next action |
| --- | --- | --- |
| `ROUTE` | Evidence is strong enough to feed ideation | Continue into the four-phase creative workflow |
| `NARROW` | The broad idea is too loose, but a sharper segment may work | Re-scope the segment/job and rerun research |
| `RERUN` | Research is too thin, stale, contradictory, or one-sided | Run another terrain and doubt pass |
| `REFUSE` | The candidate is saturated, unbuyable, unsafe, or built on false demand | Kill it and restart from another market or segment |

Only `ROUTE` can continue. This is the key guardrail: the skill must doubt findings before routing further.

## Four-Phase Creative Workflow

After a market candidate survives, or when the task is creative/problem-solving rather than market research, the skill runs the Universal Intelligence loop.

1. **The Forest of Wrong**
   Map the dogmas of the problem, then generate 4-5 load-bearing exploratory passes that deliberately break those dogmas.

2. **Friction Analysis**
   Review each exploratory like an engineer: what breaks for people, systems, trust, operations, incentives, and adoption? No premature fixes.

3. **The Pivot**
   Select one high-value wrong fragment and turn it into a powering mechanism the orthodox route would likely have discarded.

4. **Refinement**
   Produce the usable artifact with traceability, rejected alternatives, control surfaces, risks, and a teaching payload so the user can understand and steer the result.

## What A Good Output Includes

For product and market work, a strong final answer should include:

- narrow segment and buyer/user distinction
- current workaround and why it hurts
- saturation map and why incumbents miss the wedge
- strongest evidence for and against the idea
- refusal memo with `ROUTE`, `NARROW`, `RERUN`, or `REFUSE`
- confidence level, never literal certainty
- riskiest assumption and kill criteria
- first validation probe that can be run quickly
- the creative hinge or quarried shard that makes the result non-generic

## What It Refuses

The skill is designed to push back on:

- "AI for X" ideas with no specific wedge
- "better UX" as the only differentiation
- absence of competitors as proof of opportunity
- broad markets with no narrow buyer, budget, or switching moment
- ideas where the real blocker is distribution, trust, compliance, or data access
- generic SaaS concepts dressed up with edgy language
- claims of 100% certainty in a live market

## Install

From this repository:

```powershell
python scripts\install-skill-from-github.py --repo lookuters22/universal-intelligence --path universal-intelligence
```

Or copy the skill folder manually:

```powershell
Copy-Item -Recurse -Force .\universal-intelligence "$env:USERPROFILE\.codex\skills\universal-intelligence"
```

Restart Codex after installing or updating the skill.

## Update An Existing Install

If you already installed the skill manually, replace the installed folder with the repository skill folder:

```powershell
Remove-Item -Recurse -Force "$env:USERPROFILE\.codex\skills\universal-intelligence"
Copy-Item -Recurse -Force .\universal-intelligence "$env:USERPROFILE\.codex\skills\universal-intelligence"
```

Then restart Codex.

## Invocation Examples

```text
Use $universal-intelligence to find an unsaturated market gap and refuse weak ideas before brainstorming.
```

```text
Use $universal-intelligence to research product opportunities in wedding photographer operations and only route ideas that survive the refusal layer.
```

```text
Use $universal-intelligence to rethink this product idea from first principles.
```

```text
Use $universal-intelligence on this roadmap and find a non-obvious stronger direction.
```

## Repository Layout

```text
.
|-- universal-intelligence/
|   |-- SKILL.md
|   |-- agents/
|   |   `-- openai.yaml
|   `-- references/
|       |-- anti-patterns.md
|       |-- friction-analysis.md
|       |-- market-gap-research.md
|       |-- refusal-layer.md
|       |-- refinement-heuristics.md
|       |-- required-checks.md
|       |-- the-forest-of-wrong.md
|       `-- the-pivot.md
|-- README.md
|-- LICENSE
`-- .github/workflows/validate-skill.yml
```

The `universal-intelligence/` directory is the actual Codex skill. Repository-level files are packaging, license, and validation support.

## Important Limit

The skill does not promise literal certainty. Markets change, competitors react, and evidence can be incomplete. It converts "find me a 100% good idea" into a stricter and more honest target: a high-conviction idea that has survived adversarial research, has named risks, and can be validated or killed quickly.

## License

MIT
