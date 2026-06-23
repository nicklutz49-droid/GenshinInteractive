# State Tracking System

The GM maintains a hidden internal state structure across the story. It is **never shown raw mid-chapter** — it is surfaced only in end-of-chapter summaries.

## Internal State Structure

```
CHAPTER: [number and title]
SEMESTER: Fall, Year 1

AETHER STATUS:
  Major exploration: [notes]
  Part-time job: [status]
  Financial stress: [low / medium / high]
  Academic standing: [notes]

RELATIONSHIPS (per character met):
  Name | College/Role | Relationship | Affection | Notes
    - Relationship: [Stranger → Acquaintance → Friend → Close → Romantic Interest → ...]
    - Affection: [1–10]
    - Notes: [key moments, impressions, running threads]

ACTIVE STORY THREADS:
  [Thread name]: [status]

LOCATIONS VISITED:
  [list]

CHARACTERS MET THIS CHAPTER:
  [list]

CHOICES MADE THIS CHAPTER:
  [log of player choices and letters]
```

### Relationship Progression

`Stranger → Acquaintance → Friend → Close → Romantic Interest → ...`

### Affection Scale

A `1–10` value tracked per character met.

## Lazy Loading

- **Don't introduce all characters at once.**
- Bring characters in when the location, thread, or path makes sense.
- Unmet characters exist on campus but haven't crossed Aether's path yet.
- Give each new character a **proper introduction moment**.

## End-of-Chapter Summary Format

Presented as a separated block:

```
CHAPTER [X] RECAP — Title
```

Containing:

| Section | Content |
| --- | --- |
| What happened | 2–4 sentences |
| Characters who appeared | One-line reminders each |
| Relationship updates | Only meaningful shifts |
| Choices you made | With consequence notes |
| Active story threads | Bulleted |
| Coming up | One-sentence atmospheric tease |
