# Buyer Memory Ledger

A buyer-preference memory and explainability ledger that replays synthetic sell-side mandates against acquirer criteria, explains why buyers were ranked, and detects stale or contradictory buyer memory.

![Buyer Memory Ledger working dashboard](outputs/project_working.svg)

## Why it exists

AI-native SME M&A depends on remembering buyer preferences, deal structures, and owner constraints without creating a black-box matching process.

The project is intentionally built as a local replay harness instead of a slide. It creates fixtures, plants realistic failure modes, produces citation-locked evidence, and turns the result into a dashboard a reviewer can inspect without credentials or hosted services.

## What is inside

- Deterministic fixture generation for the company-specific risk surface.
- Strategy code in `src/buyer_memory_ledger/strategy.py` with project-specific scoring and visual evidence.
- Citation-locked reports where every decision claim points to a generated evidence ID.
- Two regenerated visual artifacts: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, benchmark, and test artifacts.

![Buyer Memory Ledger evidence map](outputs/evidence_map.svg)

## Signals it measures

- `ai-native coverage`
- `depends risk`
- `remembering precision`
- `buyer latency`

## Failure modes it plants

- ai-native drift
- depends gap
- remembering misroute
- buyer blindspot

## Run it locally

```bash
uv sync
uv run buyer-memory-ledger all
uv run pytest -q
uv run ruff check .
```

## Outputs worth opening

- `outputs/dashboard.html`
- `outputs/project_working.svg`
- `outputs/evidence_map.svg`
- `outputs/operator_brief.md`
- `outputs/decision_report.md`
- `outputs/strategy_model.json`
- `outputs/demo_pack.zip`

## Boundary

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.
