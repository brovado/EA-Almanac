# EA Almanac — Core Specification

## Purpose

The EA Almanac is a developmental reference system designed to answer:

> Given a child's current age and stage of life, what wisdom, opportunities, challenges, and guidance are most relevant right now?

It is **not** a child-tracking or diagnostic system. It is a reusable knowledge library for daily, weekly, and monthly parent guidance, eventually integrated with the personal vault.

## Developmental age bands

- `0-1` — Attachment Foundations
- `1-2` — Emerging Independence
- `2-5` — Exploration & Agency
- `6-9` — Competence & Mastery
- `10-13` — Identity Formation
- `14-18` — Independence Testing
- `19-25` — Launch & Adulthood

These are developmental seasons, not hard milestone boundaries.

## Core categories and density

| Category | 1–2 | 2–5 |
|---|---:|---:|
| Experiencing | 50 | 50 |
| Needs | 50 | 50 |
| Teach | 100 | 100 |
| Encourage | 75 | 75 |
| Avoid | 50 | 50 |
| Healthy Development | 50 | 50 |
| Warning Signs | 50 | 50 |
| Weekly Focus | 100 | 100 |
| Monthly Focus | 100 | 100 |
| Books | 50 | 50 |
| Activities | 100 | 100 |
| Conversations | 100 | 100 |
| Life Skills | 100 | 100 |
| Opportunities | 50 | 50 |
| Parent Reminders | 100 | 100 |
| **Total** | **1,125** | **1,125** |

**Note:** the category values above sum to 1,125. The earlier 1,175 total was an arithmetic error and is superseded by this specification.

## Category philosophy

Categories are intentionally distinct. `experiencing` describes the developmental season; `needs` describes supporting conditions; `teach` names capabilities; `encourage` identifies behaviours and interests to make room for; `avoid` identifies counterproductive responses and preventable risks; `healthy_development` provides observational examples; `warning_signs` remains non-diagnostic and routes concerns toward professional assessment; `weekly_focus` and `monthly_focus` turn knowledge into themes; `books` and `activities` supply concrete experiences; `conversations` supports responsive language and thinking; `life_skills` decomposes independence into teachable steps; `opportunities` connects development with real-world experiences; and `parent_reminders` keeps attention on the adult's role in the developmental environment.

## Entry requirements

Entries should be atomic, reusable, age-appropriate, and category-specific. Avoid merely repeating the same idea with different wording. Where a claim is evidence-sensitive, preserve source IDs and avoid presenting philosophy as scientific fact.

## Evidence standard

Research should prioritize primary or professional sources: government developmental guidance, pediatric organizations, WHO/UNICEF, established early-childhood frameworks, and library/educational organizations. Health, safety, and warning-sign material should be conservative and explicitly non-diagnostic.

## Current research build

The initial research pass covers `1-2` and `2-5` across all 15 categories. The audited source registry and research synthesis live under `RESEARCH/`.

The full working corpus has been generated and validated locally; GitHub currently contains the research/audit layer and data manifests. The next repository ingestion step should materialize the validated corpus into human-readable JSON/JSONL without losing source provenance.

## Selection model

Daily output should rotate entries while respecting age fit, category balance, recent-use avoidance, and developmental themes. Weekly output should synthesize a coherent theme. Monthly output should behave like a seasonal developmental chapter rather than a checklist.

## Guiding principle

> **What matters about this stage of my child's life that I might otherwise miss?**

The Almanac should help a parent see the larger developmental picture while still giving them something useful to do today.