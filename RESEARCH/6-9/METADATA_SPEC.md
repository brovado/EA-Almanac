# 6–9 Corpus Metadata Specification

## Required fields
- `id`: stable unique identifier
- `category`: one of the 15 Almanac categories
- `domain`: one primary domain from DOMAIN_MODEL.md
- `window`: age window code
- `tags`: searchable concepts
- `weight`: retrieval priority, integer 1–5
- `source_type`: evidence, professional_guidance, educational_framework, practical_wisdom, or family_philosophy
- `text`: atomic reusable content

## Recommended fields
- `source_ids`: references into the age-band source registry
- `secondary_domains`: additional relevant domains
- `notes`: editorial or retrieval notes

## Age windows
- `6-6.9`: 72–83 months
- `7-7.9`: 84–95 months
- `8-9.9`: 96–119 months
- `6-9-broad`: guidance intentionally not tied to a narrower window

## Editorial rule
A window describes when content is especially relevant; it is not a developmental deadline. Avoid converting population-level patterns into requirements for an individual child.
