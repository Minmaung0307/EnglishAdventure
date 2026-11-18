# English Adventure USA — GitHub + Firebase (no-cost-first)

This package preserves the existing interactive HTML prototype and adds a Vite build, GitHub CI, and Firebase Hosting configuration. **It is not yet a React/TypeScript conversion.** No paid AI or database services are enabled.

## Run on your Mac in VS Code terminal

```bash
npm install
npm run dev
```

Open the local URL printed by Vite (usually http://localhost:5173).

## Git + GitHub

Create an **empty** repository on GitHub (do not initialize README), then run:

```bash
git init
git add .
git commit -m "Initial English Adventure USA Vite prototype"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/english-adventure-usa.git
git push -u origin main
```

If you already have a git repository, **do not run `git init` or overwrite `.git`**. Copy these project files into your existing repo, then use `git status`, `git add .`, `git commit`, and `git push`.

## Firebase Hosting — Spark (no-cost)

1. In Firebase Console, create a **new project**; select **Spark (No-cost)**. Do not enable billing or upgrade to Blaze.
2. Install Firebase CLI on your Mac: `npm install -g firebase-tools`
3. Run `firebase login`
4. Build: `npm run build`
5. Deploy using the exact project ID: `firebase deploy --only hosting --project YOUR_FIREBASE_PROJECT_ID`
6. If the CLI asks to initialize Hosting, this repo **already contains** `firebase.json`; do not overwrite it.
7. To use a custom subdomain later, configure it through Firebase Hosting > Add custom domain and your DNS provider. Keep existing game domains unchanged.

**Cost controls:** The prototype uses localStorage, local browser speech synthesis, and browser-dependent speech recognition. No Firestore reads/writes, Cloud Functions, Storage uploads, or paid AI requests. Spark quotas still apply; high traffic can hit service limits. The domain registration, if purchased, is a separate cost.

**Security:** Never commit service-account keys or private AI API keys. `.env` files are ignored. Firestore and Storage rules included as deny-all examples; they are **not deployed by the Hosting-only command**. Do not replace existing Firebase project rules with these examples if other apps use that project. Use a dedicated Firebase project.

## Project layout

- `index.html` — original interface markup
- `public/app.js` — original game/lesson logic, browser local progress
- `public/style.css` — original visual design
- `firebase.json` — Hosting only
- `.github/workflows/ci.yml` — GitHub push / PR build validation

## Next milestone

Refactor into React + TypeScript components, move lessons into JSON, add validated offline assets, and then opt-in Firebase Authentication + private Firestore progress sync only if necessary. Avoid any unbounded AI usage.
