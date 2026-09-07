# EA Almanac — Semantic QA Status

## Prototype corpus audit

Both prototype age bands contain 1,125 entries across the 15 requested categories.

### Editorial semantic pass

| Measure | 1–2 | 2–5 |
|---|---:|---:|
| Entries audited | 1,125 | 1,125 |
| Exact duplicate entries rewritten | 83 | 91 |
| Exact duplicate text remaining after rewrite | 0 | 0 |
| Terse/generic entries flagged | 230 | 312 |

### Retrieval windows

**1–2:** 12–15m, 15–18m, 18–24m

**2–5:** 24–30m, 30–36m, 36–48m, 48–60m

Age windows are retrieval scopes, not milestone deadlines. Broad developmental guidance is not given false age precision.

## What this pass fixed

- Removed mechanically repeated activity entries by replacing them with genuinely different activity variants.
- Removed exact duplicate developmental and parent-reminder text.
- Expanded topical tagging so retrieval can distinguish language, autonomy, motor, play, social, emotions, routines, safety, literacy, numeracy, science, self-care, executive function, and parenting.
- Added explicit QA status and quality flags for entries that are too terse or generic for long-term reference use.

## What remains

The next editorial pass should rewrite the flagged terse/generic entries and then run semantic-near-duplicate clustering within each category. Books and opportunities should receive a separate current-availability/age-fit review before being treated as production data.

## Canonical files

The complete QA-enriched JSONs are retained as conversation data uploads. This repository contains the QA specification, status, and overlay so that the source corpus is not silently replaced by a truncated GitHub Contents API write.
