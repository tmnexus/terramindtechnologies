Terramind Technologies — Static Landing Page

Files added:

- `index.html` — The static landing page (Coming Soon) with a 30-day countdown timer (default behavior).

How to preview locally (Windows PowerShell):

1. Open PowerShell and change directory to the project folder, for example:

```powershell
cd "D:\Terramind Technologies\Landing Page"
```

2. Serve the folder with a simple HTTP server (Python must be installed):

```powershell
python -m http.server 8000
```

Then open http://localhost:8000 in your browser.

Tip: You can also just open `index.html` directly in your browser, but some features (fonts/CSP) are best tested via a local server.

How to change the launch date:

Open `index.html` and find the script section near the bottom. The page currently sets the launch date to 30 days from the current date with:

```js
const launchDate = new Date();
launchDate.setDate(launchDate.getDate() + 30);
```

Replace this with a specific date if you want a fixed launch date, for example (UTC):

```js
// Set fixed launch date: 2025-12-15T00:00:00Z
const launchDate = new Date('2025-12-15T00:00:00Z');
```

Next steps I can help with:
- Wire the newsletter form to Netlify Forms, Mailchimp, or a backend endpoint.
- Add SEO/meta improvements or Open Graph images.
- Generate small assets (favicon, logos) and optimize images for web.

If you want, tell me where you'd like the files placed (different folder) or if you want form integration now.