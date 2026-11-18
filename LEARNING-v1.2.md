# English Adventure USA v1.2 — Individual Practice Expansion

Adds an **individual practice panel to each of the 80 existing lessons**. Each panel uses the lesson’s existing, individually authored title, key phrase, Burmese translation, explanation, question, answer choices, and writing prompt.

Activities: listening gap-fill, reading comprehension, repeat-and-speak, autosaved writing, and review. The existing eight shared level studios, dialogues, 24 missions, guest progress, and PWA remain.

**Scope transparency:** The 80 new panels are generated from existing lesson content, not 80 newly authored full-length dialogues. No MP4 clips, paid AI, or automatic writing/pronunciation scoring are included.

## Deploy

```sh
npm ci
npm run build
firebase deploy --only hosting --project english-mm
```

Test on mobile and desktop before deploying. Back up the existing project first.
