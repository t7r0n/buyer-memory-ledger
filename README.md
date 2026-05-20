# Buyer Memory Ledger

A buyer-preference memory and explainability ledger that replays synthetic sell-side mandates against acquirer criteria, explains why buyers were ranked, and detects stale or contradictory buyer memory.

![Buyer Memory Ledger working dashboard](outputs/project_working.svg)

## Why it exists

AI-native SME M&A depends on remembering buyer preferences, deal structures, and owner constraints without creating a black-box matching process.

Most internal demos stop at a pretty chart. This repository is built around the harder part: a repeatable path from fixture, to failure, to evidence, to the operator action a serious team would actually trust.

## What is inside

- A deterministic replay harness tuned around ai-native, depends, and remembering.
- Company-specific strategy code in `src/buyer_memory_ledger/strategy.py`, not just README-level customization.
- Citation-locked reports where every decision claim has to point back to a generated evidence ID.
- Two visual artifacts generated from the latest run: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, and benchmark artifacts.

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

## Sources

- https://www.dealflowagent.com/about
- https://www.dealflowagent.com/partnerships
- https://www.eu-startups.com/2026/03/dealflowagent-raises-e646-2k-led-by-early-uber-and-spacex-backer-to-scale-ai-native-investment-bank-for-sme-ma/

## Boundary

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.
