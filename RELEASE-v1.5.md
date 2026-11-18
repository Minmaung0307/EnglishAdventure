# English Adventure USA v1.5 — Captioned Mini-Clip Studio

- Added a four-scene captioned mini-clip to every existing lesson using its scenario dialogue.
- Play, Pause, Replay, Stop; optional browser speech synthesis and silent caption fallback.
- Uses no video hosting, paid APIs, or new Firebase services.
- These are **animated captions**, not filmed or MP4 videos, and do not replace independently authored lesson scripts.
- Existing 80 lessons and 24 missions remain as-is; no new lessons were authored.
- PWA shell cache bumped to v15.

## Verify before deployment

`npm ci && npm run build`

Then test lesson clips, browser Back/navigation, microphone permissions, offline install and saved guest progress in a browser. Deploy with `firebase deploy --only hosting --project english-mm` only after verifying.
