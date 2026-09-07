# EA Almanac Developmental-Window QA

This pass adds finer retrieval windows to the two prototype age bands without replacing the broad-band model.

## Windows

**1–2 Emerging Independence**
- 12–15 months
- 15–18 months
- 18–24 months

**2–5 Exploration & Agency**
- 24–30 months
- 30–36 months
- 36–48 months
- 48–60 months

## Retrieval rule

`age_windows` means the developmental window in which an entry is useful for retrieval; it is not a milestone deadline. Source-anchored windows are used where a category entry has a specific age-linked source. Otherwise, entries remain broad-band rather than receiving false precision.

## QA findings

- Both corpora meet the requested category counts: 1,125 entries each.
- 150 mechanical activity-template artifacts were identified per corpus and cleaned in the QA working copies.
- Duplicate text clusters remain flagged for editorial diversification rather than silently deleting entries and reducing density.
- Topic retrieval was improved by replacing the mostly generic `development` tag with topical tags such as `language`, `autonomy`, `motor`, `play`, `social`, `emotions`, `routines`, `safety`, `sleep`, `literacy`, and `parenting`.
- Warning-sign material remains informational and directs the parent toward professional discussion rather than diagnosis.

## Evidence anchors

CDC currently publishes milestone checkpoints at 15 months, 18 months, 2 years, 30 months, 3 years, 4 years, and 5 years. CDC defines its milestone lists as skills that most children (75% or more) can do by a given age and explicitly states that the lists are not substitutes for standardized developmental screening. The AAP recommends developmental surveillance throughout early childhood, general developmental screening at 9, 18, and 30 months, and autism-specific screening at 18 and 24 months.

## Editorial standard

The next QA pass should prioritize semantic diversification: two entries should not differ only by wording or by a mechanical activity modifier. Entries should provide genuinely different parent decisions, observations, skills, conversations, or experiences.
