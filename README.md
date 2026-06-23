# Menny's Command Center

A self-contained AE ramp tool built on Nilus treasury knowledge + the AFP Essentials textbook.

## What's inside

- **Dashboard** — 10-day ramp overview with completion stats
- **Ramp Plan** — Daily task checklist (integrated with Growth Plan items)
- **Flashcards** — 1,016 Anki-style SM-2 spaced repetition cards across 3 decks:
  - Treasury Domain (992 cards from AFP Essentials 7th Ed., all 20 chapters)
  - Nilus Product (12 cards)
  - Sales Skills (12 cards)
- **Progress** — Per-deck and per-chapter completion tracking
- **Objection Bank** — Common objections + Nilus responses
- **Resources** — Key links (AFP, Nilus docs, etc.)
- **Growth Plan** — 62-item self-rating tracker (32 sales skills + 30 product modules)

## Tech

Single self-contained HTML file — no backend, no build step, no dependencies.  
All data (flashcards, ramp plan, progress) persists in `localStorage`.

## Deployment

Deployed to Vercel as a static site. Connected to this repo — push to `main` = auto-deploy.

## Integration

To slot this into the existing Nilus GTM Command Center:
1. The full flashcard + SM-2 engine lives in the `<script>` block
2. The CSS variables follow the Nilus design system (purple `#7c3aed`, white main area, dark sidebar)
3. Drop `menny_command_center.html` as a route in the existing app, or lift the individual page sections as needed
