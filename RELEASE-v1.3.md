# English Adventure USA v1.3 — Guided Conversation & Spaced Review

## Added
- Each of the existing 80 lessons has a guided role-play using its own question and correct response.
- Listening and speaking controls use browser speech APIs (availability varies by browser).
- Each lesson now includes a spaced-repetition review with 10-minute retry and 1/3/7/14/30-day intervals.
- Review schedule is saved under the existing guest progress writing map and is included in existing JSON export/import.
- Offline-first: no paid AI, no Firestore writes, no login.

## Limits
- This is guided role-play, not AI conversation or a verified pronunciation assessment.
- The existing 80 lesson content items are not 80 newly authored multi-scene scripts.
- No MP4 videos are included. Existing animated-caption clips remain.
- Browser text-to-speech voices and speech recognition depend on device/browser; recognition may use an online service.

## Deploy
Run npm ci && npm run build, then firebase deploy --only hosting --project english-mm. Check the app in a browser before committing.
