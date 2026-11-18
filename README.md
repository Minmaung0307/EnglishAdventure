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


## v0.7 additions
- Eight original, local SVG illustrated level banners (`public/art/levels/`). No remote image downloads or copyright-dependent stock assets.
- Guest profile with nickname, avatar, JSON progress export/import. No sign-in, Firestore, or paid APIs.
- Existing 80 lessons and 24 missions remain unchanged. The existing lesson illustrations remain in `public/art/lessons/`.
- Updated PWA shell cache to v7.
- Browser storage is per browser/device; export a backup before clearing data or changing devices.

### Checks
Run `npm ci && npm run build`; then test profile save/export/import, level cards, lessons, missions and offline PWA. Do not overwrite `.git` or existing local data.


## v0.8 illustration refresh
- Replaced all eight level illustrations with eight unique **people-free** illustrated scenes: welcome skyline, cafe, city navigation, workplace charts, discovery books, professional growth, microphone/podium, and leadership hall.
- Updated hover/focus/reduced-motion treatments and incremented the offline service-worker cache to v8.
- Kept all existing lessons, guest profile, XP, mission, audio and Firebase Hosting behavior unchanged.
- This update does **not** add real MP4 videos or claim new lessons. Those need separately produced/licensed assets and reviewed teaching content.
