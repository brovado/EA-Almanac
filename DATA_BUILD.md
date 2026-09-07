# EA Almanac — Corpus Build Status

**Build date:** 2026-09-07

## Verified working corpus

The research build contains:

- `1-2`: **1,125 entries**
- `2-5`: **1,125 entries**
- **2,250 entries total**

The category targets are exactly those specified in `ALMANAC_SPEC.md` and sum to 1,125 per age band.

## Category counts per age band

| Category | Count |
|---|---:|
| experiencing | 50 |
| needs | 50 |
| teach | 100 |
| encourage | 75 |
| avoid | 50 |
| healthy_development | 50 |
| warning_signs | 50 |
| weekly_focus | 100 |
| monthly_focus | 100 |
| books | 50 |
| activities | 100 |
| conversations | 100 |
| life_skills | 100 |
| opportunities | 50 |
| parent_reminders | 100 |
| **Total** | **1,125** |

## Research lanes

The build independently considers developmental experience, needs, teaching, encouragement, avoidance, observable healthy development, warning signs, weekly/monthly themes, books, activities, conversations, life skills, opportunities, and parent perspective.

Evidence is primarily drawn from CDC developmental milestones, WHO/UNICEF nurturing care and early-childhood guidance, NAEYC developmentally appropriate practice, Harvard Center on the Developing Child material on serve-and-return and executive function, American Academy of Pediatrics guidance, and Association for Library Service to Children resources. See `RESEARCH/SOURCES.md`.

## Validation notes

- Counts were programmatically verified for both age bands.
- Category-level duplicate checking was performed; a small number of repeated concepts remain deliberately reframed for reuse, especially in parent-reminder and experience material.
- Warning-sign entries are non-diagnostic and written as prompts for professional discussion.
- The 1–2 and 2–5 bands are broad developmental seasons; finer age-window metadata is the next precision improvement.

## Ingestion

The complete JSON corpus exists as verified working artifacts outside the repository and is ready for repository ingestion. GitHub's connected write interface available in this session does not provide a direct local-file upload operation, so the repository currently holds the specification, research report, source registry, and this auditable build manifest rather than a falsely advertised partial JSON upload.
