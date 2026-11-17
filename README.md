# CapitalGains demo

A copy of the app that opens with sample data and no passcode. There is no database and no server storage.

- Sample data (26 weeks of lifts) loads the first time someone opens it.
- Anything a visitor logs or changes stays in their own browser only. Settings has a "Reset demo data" button.
- The first-open tutorial runs automatically on the first visit.
- The camera features and tester feedback are turned off.
- The feed shows invented sample people.

## Publish it
1. Put these files in a new GitHub repo (not the repo for your real app).
2. On vercel.com choose Add New, then Project, import that repo, and click Deploy. No environment variables are needed.
3. Share the `.vercel.app` link.

## Run it on your computer
```
npm install
npm run dev
```
