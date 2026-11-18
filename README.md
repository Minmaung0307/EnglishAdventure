# English Adventure USA v0.6 — Illustrated Academy

Based on v0.5, preserving existing app, missions, PWA and Firebase Spark hosting.

- 80 guided sample lessons across 8 levels (10 per level).
- Unique locally bundled SVG title illustrations per lesson; no external images or image API charges.
- Smooth card motion and reduced-motion accessibility.
- Animated dialogue storyboard with speech synthesis (not actual video footage).
- No paid AI, Firestore, Storage, Functions or analytics calls.

## Run

```bash
npm install
npm run build
firebase deploy --only hosting --project english-mm
```

## Limitations

The additional lessons are guided examples, not comprehensive accredited course material. Writing is not AI graded. Speech recognition and TTS depend on browser support. Animated clips use caption/voice sequences, not prerecorded videos. No user data sync across devices.

Back up the current project and preserve your `.git` directory before replacing files.
