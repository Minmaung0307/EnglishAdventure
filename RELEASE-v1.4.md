# English Adventure USA v1.4 — 80 Scenario Rehearsals

## Delivered
- Preserves the 80 lessons, eight levels, missions, guest profile, offline PWA and existing studios.
- Adds a four-turn topic-aware guided scenario to **each existing lesson**, including narration, slow playback, Burmese reference translation, writing autosave and a self-check rubric.
- Scenarios are **template-guided** using each lesson's authored target expression, not 80 independently authored natural dialogues.
- Does not include filmed MP4 clips, live AI dialogue, reliable pronunciation scoring or automated writing evaluation. These require separate authored media/technology and validation.
- No paid API or new Firebase services required.

## Release checks
Run `npm ci && npm run build`, test representative lessons across all eight levels, confirm audio and microphone support in target browsers, then `firebase deploy --only hosting --project english-mm`.
