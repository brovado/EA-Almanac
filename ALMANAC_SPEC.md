# EA Almanac — Core Specification

## Purpose

The EA Almanac is a developmental reference system designed to answer:

> Given a child's current age and stage of life, what wisdom, opportunities, challenges, and guidance are most relevant right now?

The Almanac is **not** a child-tracking system. It is a structured library of developmental knowledge that can be queried to generate useful daily, weekly, and monthly guidance for parents.

The intended end state is integration with a personal vault, where the Almanac can supply age-appropriate material to an existing daily snapshot system.

---

# Developmental Age Bands

The Almanac should be organized around broad developmental seasons rather than requiring a separate document for every birthday.

Initial planned bands:

- `0-1` — Attachment Foundations
- `1-2` — Emerging Independence
- `2-5` — Exploration & Agency
- `6-9` — Competence & Mastery
- `10-13` — Identity Formation
- `14-18` — Independence Testing
- `19-25` — Launch & Adulthood

These bands are a starting structure and may be refined as the Almanac develops.

---

# Core Content Categories

Every age band should eventually contain material in the following categories.

## 1. What They Are Experiencing

Developmental realities, internal changes, emotional development, cognitive changes, social changes, and common experiences during the stage.

**Target: 50+ entries per age band**

## 2. What They Need

Core developmental needs, environmental needs, relational needs, and conditions that support healthy growth.

**Target: 50+ entries per age band**

## 3. What To Teach

Skills, concepts, habits, knowledge, and practical understanding that should be introduced or reinforced.

**Target: 100+ entries per age band**

## 4. What To Encourage

Behaviors, attitudes, interests, habits, and opportunities that should be actively supported.

**Target: 75+ entries per age band**

## 5. What To Avoid

Common parenting mistakes, environmental risks, counterproductive approaches, and developmental traps.

**Target: 50+ entries per age band**

## 6. Signs Of Healthy Development

Observable indicators that development appears to be progressing in a healthy direction.

This is informational rather than diagnostic. Where appropriate, entries should distinguish normal variation from situations where professional advice may be useful.

**Target: 50+ entries per age band**

## 7. Warning Signs

Potential concerns, persistent difficulties, or situations worth monitoring or discussing with an appropriate professional.

This category must avoid presenting the Almanac as a diagnostic tool.

**Target: 50+ entries per age band**

## 8. Weekly Focus Ideas

Small developmental themes suitable for a week-long emphasis.

Examples:

- Practice letting the child make two meaningful choices each day.
- Spend one week naming emotions during ordinary situations.
- Give the child one additional household responsibility.

**Target: 100+ entries per age band**

## 9. Monthly Focus Ideas

Broader developmental themes suitable for sustained attention over several weeks.

Examples:

- Building independence
- Developing frustration tolerance
- Exploring nature
- Building early money awareness

**Target: 100+ entries per age band**

## 10. Books

Books for the parent and age-appropriate books or reading material for the child.

Entries should eventually contain enough metadata to distinguish:

- Parent reference
- Child reading/listening
- Developmental purpose
- Suggested age

**Target: 50+ entries per age band**

## 11. Activities

Games, projects, outings, experiments, exercises, creative activities, and experiences that support development.

**Target: 100+ entries per age band**

## 12. Conversations

Questions, discussion prompts, storytelling prompts, and opportunities for meaningful conversation.

**Target: 100+ entries per age band**

## 13. Life Skills

Practical capabilities that gradually build independence and competence.

**Target: 100+ entries per age band**

## 14. Opportunities

Programs, certifications, experiences, clubs, hobbies, competitions, volunteering, travel, employment opportunities, and other age-dependent possibilities.

**Target: 50+ entries per age band**

## 15. Parent Reminders

Guidance aimed directly at the parent rather than the child.

This is a core category, not an afterthought.

Many parenting situations are improved not by changing the child, but by changing the parent's perspective, expectations, behavior, or response.

**Target: 100+ entries per age band**

Example reminders:

- They aren't giving you a hard time; they're having a hard time.
- Connection before correction.
- Their pace is slower than yours.
- Curiosity beats punishment.
- Independence looks messy.
- Repetition is learning.
- Play is work.
- Most behavior is communication.

---

# Content Density

The target density for a mature age band is:

| Category | Target Entries Per Age Band |
|---|---:|
| Experiencing | 50 |
| Needs | 50 |
| Teach | 100 |
| Encourage | 75 |
| Avoid | 50 |
| Healthy Development | 50 |
| Warning Signs | 50 |
| Weekly Focus | 100 |
| Monthly Focus | 100 |
| Books | 50 |
| Activities | 100 |
| Conversations | 100 |
| Life Skills | 100 |
| Opportunities | 50 |
| Parent Reminders | 100 |
| **Total** | **1,175** |

The 1,175 figure is a target, not a requirement that every age band be completely filled before the system is useful.

The important goal is **content variety without sacrificing quality**.

---

# Daily Snapshot Philosophy

The Almanac should not change its underlying developmental guidance every day.

Instead, it should provide a large enough pool of relevant material that daily output can vary naturally while remaining consistent with the child's developmental season.

A daily snapshot should therefore select a small number of relevant entries from the current age band.

Example query:

```text
Child Age: 2y 10m

Return:
- One thing she's experiencing
- One thing she needs
- One thing I should encourage
- One thing I should avoid
- One activity suggestion
```

Possible output:

```text
Child Age: 2y 10m

Experiencing:
Testing where her influence ends and yours begins.

Needs:
Safe opportunities to make choices.

Encourage:
Helping with simple household tasks.

Avoid:
Turning ordinary delays into unnecessary power struggles.

Activity:
Help prepare part of breakfast.
```

A richer snapshot may additionally request:

```text
- One conversation prompt
- One life skill
- One parent reminder
```

---

# Weekly Snapshot Philosophy

Weekly output should synthesize several entries into a practical theme rather than simply listing seven random tips.

Example:

```text
Weekly Theme: Growing Independence

Why it matters:
The child is increasingly motivated to do things independently but still lacks the physical, emotional, and cognitive ability to manage everything alone.

This week:
- Offer two meaningful choices each day.
- Let the child attempt tasks before helping.
- Give one recurring household responsibility.
- Praise persistence rather than speed.

Parent Reminder:
Independence is often messy before it becomes competent.
```

---

# Monthly Snapshot Philosophy

Monthly output should identify a broader developmental theme and provide a small collection of suggested actions, activities, conversations, and life skills.

The monthly layer should feel like a **seasonal chapter in development**, not a checklist of milestones.

---

# Selection Rules

The future query system should prefer:

1. Age-appropriate entries.
2. Entries that have not appeared recently.
3. A mixture of categories.
4. A mixture of practical actions and perspective.
5. Entries relevant to the current developmental season.
6. Occasional unexpected or less-obvious suggestions to prevent the system from becoming repetitive.

The system should avoid repeatedly returning the same high-level advice simply because it is important.

For example, "encourage independence" may be foundational guidance, but daily snapshots should surface different manifestations of that principle.

---

# Atomic Content Principle

Content should be written as small, reusable units wherever practical.

Prefer:

```text
Children are beginning to understand that other people have different thoughts and feelings.
```

over:

```text
At this age children experience a huge amount of social, cognitive, and emotional development. They are beginning to understand other people and should therefore be encouraged to...
```

Atomic entries allow the same knowledge to be reused across daily, weekly, monthly, activity, and thematic queries.

---

# Future Entry Metadata

As the repository grows, entries should eventually support structured metadata such as:

```yaml
id: E-2-5-001
category: experiencing
age_band: 2-5
priority: normal
text: "..."
tags:
  - autonomy
  - emotional-development
  - social-development
source_status: researched
```

Metadata should be expanded only when it solves an actual retrieval problem.

Do not over-engineer the schema before the content model has been tested.

---

# Research Standard

The Almanac is intended to become a serious long-term reference rather than a collection of generic parenting tips.

Content should eventually distinguish between:

- Evidence-backed developmental guidance
- Professional recommendations
- Educational philosophies
- Cultural practices
- Practical parenting wisdom
- Opportunities and programs
- Personal family philosophy

Sources and confidence should be retained where practical, especially for health, safety, development, and warning-sign material.

The Almanac should never present a philosophical preference as if it were universally established scientific fact.

---

# Initial Test Scope

The first complete prototype will focus on two age bands:

- **1-2 — Emerging Independence**
- **2-5 — Exploration & Agency**

These two bands will be used to test:

- Content structure
- Entry quality
- Retrieval
- Daily variation
- Weekly synthesis
- Monthly synthesis
- Parent Reminder usefulness
- Age-band boundaries
- Future integration with the personal vault

Once the model proves useful, the remaining age bands can be expanded using the same architecture.

---

# Guiding Principle

The Almanac should help a parent answer one question:

> **What matters about this stage of my child's life that I might otherwise miss?**

It should not attempt to produce perfect parents or perfectly optimized children.

Its purpose is to keep the parent looking at the larger developmental picture while still providing concrete things that can be done today.
