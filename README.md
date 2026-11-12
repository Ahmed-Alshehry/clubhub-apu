# ClubHub APU

One place to find every club at APU. Built for the **APU Cloud Innovation Hackathon 2026** (Smart Campus & Student Experience).

**Problem:** clubs and events are only announced on scattered social media pages, so students miss them.
**Solution:** a calm website that groups clubs by domain and recommends clubs from how a student feels ("stressed", "lonely") using Gemini.

## Google Cloud
- **Firebase Hosting:** serves the website over HTTPS
- **Firebase AI Logic + Gemini API:** reads the student's message and picks clubs, with a reason. No API key is stored in the code.

If the AI is unavailable, the site falls back to simple keyword matching.

## Deploy
1. `npm install -g firebase-tools` then `firebase login`
2. `firebase use --add` and choose your project
3. Paste your Firebase web config into `public/index.html`
4. `firebase deploy --only hosting`

## Notes
- Club data is sample data.
- Built with help from AI tools.
