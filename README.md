# Universal Intelligence Codex Skill

Universal Intelligence is a Codex skill for deliberate exploratory thinking and product opportunity discovery: research market gaps, refuse weak findings before ideation, generate wrong-road material, inspect its friction, quarry the useful shard, and refine it into an actionable artifact with visible reasoning and human control.

Use it for unsaturated market research, product/startup ideas, product strategy, UX direction, architecture forks, naming, positioning, process design, critique, and other creative or diagnostic work where ordinary best-practice answers are too flat.

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

## Repository Layout

```text
.
├── universal-intelligence/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/
├── README.md
├── LICENSE
└── .github/workflows/validate-skill.yml
```

The `universal-intelligence/` directory is the actual Codex skill. The repository-level files are packaging, license, and validation support.

## What The Skill Does

For product and market work, the skill runs a pre-flight evidence loop before ideation:

1. **Market Gap Research**: map current alternatives, demand signals, saturation, substitutes, timing shifts, and failure signals.
2. **Doubt Pass**: search against the promising finding and try to kill it.
3. **Evidence Refusal Layer**: route the candidate as `ROUTE`, `NARROW`, `RERUN`, or `REFUSE`; only `ROUTE` can feed ideation.

Then the skill runs a four-phase method:

1. **The Forest of Wrong**: map dogmas, then generate 4-5 load-bearing exploratory passes.
2. **Friction Analysis**: inspect each pass for human and systemic breakage without fixing it early.
3. **The Pivot**: select one high-value wrong fragment and turn it into a powering mechanism.
4. **Refinement**: produce the usable artifact with traceability, rejected alternatives, control surfaces, and a teaching payload.

The goal is not novelty theater or fake certainty. The goal is to escape interchangeable 7/10 answers while keeping the user in the cockpit, with market claims backed by evidence, counterevidence, kill criteria, and a first validation probe.

## Invocation

```text
Use $universal-intelligence to rethink this product idea from first principles.
```

```text
Use $universal-intelligence to find an unsaturated market gap and refuse weak ideas before brainstorming.
```

```text
Use $universal-intelligence on this roadmap and find a non-obvious stronger direction.
```

## License

MIT
