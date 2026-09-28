# Hooks Workout — Demo

A shareable demo of the Hooks Workout tracker. It runs entirely in the visitor's browser:

- **No login, no database, no environment variables.**
- Loads **five years of sample** lifting history (fake, and identical for everyone): beginner gains, a plateau, a second climb, stagnation, a drop with a short layoff, then a gradual rebuild.
- Anything a visitor logs or changes is saved **only in their own browser** (localStorage). Nothing is sent anywhere, and nobody sees anyone else's changes.
- The **Reset** button in the bar at the top restores the original sample data.

## Deploy (about 5 minutes)

**Important: this goes in a NEW GitHub repo — not your personal `hooks-workout` repo.**
Uploading it over the personal one would replace your real app.

1. On github.com create a new repository, e.g. `hooks-workout-demo` (Public or Private both work).
2. Click **uploading an existing file** and drag in *the contents of this folder*: `package.json`, `package-lock.json`, `next.config.js`, `README.md`, and the `pages`, `styles` and `public` folders (`public` holds the home-screen icon). Commit.
3. On vercel.com: **Add New → Project → import that repo → Deploy.** Leave every setting at its default.
4. Vercel gives you a `*.vercel.app` link. Send it to friends. On iPhone they can tap Share → Add to Home Screen.

There is nothing else to set up, and nothing to update on the server side.

## Notes
- The page asks search engines not to index it, so the link is only as public as the people you send it to.
- To refresh the sample data later, change `buildDemoData()` in `pages/index.js` and bump `DEMO_KEY` (e.g. `...V3`) so visitors' old saved copies are ignored.

## Getting it on an iPhone Home Screen
The demo shows a one-time tip with these steps to anyone opening it in iPhone/iPad Safari. To share the steps yourself:

> Open the link in **Safari** → tap the **Share** button (square with an arrow) → scroll down → **Add to Home Screen** → **Add**.
> It then opens full screen with its own icon, like a regular app.

Notes: it has to be Safari for the tip's steps (other iPhone browsers hide the option in different places). A home-screen copy keeps its own saved data, separate from the copy in Safari.
