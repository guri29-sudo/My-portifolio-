# Portfolio Site

A static site (plain HTML/CSS/JS — no build step, no framework) showcasing
four real projects with live-captured screenshots and honest metrics.

## Before you deploy — edit these

Open `index.html` and search for these placeholders, then replace them:

- `[Your Name]` — in the header (appears once)
- `[ your.email@example.com ]` and `REPLACE_WITH_YOUR_EMAIL` — in the Contact section
- `[ github.com/your-username ]` — update both the visible text and the `href="#"`
- `[ linkedin.com/in/your-username ]` — same, update text and `href="#"`

Everything else on the page — the four project write-ups, the metrics
tables, the screenshots — is real and doesn't need editing. If you add new
projects later, follow the same `<section class="project">` pattern already
in the file.

## Deploy to Vercel

**Option A — no GitHub needed (fastest):**
1. Go to https://vercel.com/new
2. Drag this whole folder onto the upload area
3. Deploy — Vercel serves static HTML with zero configuration

**Option B — via GitHub (better if you'll keep editing it):**
1. Create a new repo, push this folder to it
2. In Vercel, "Import Project" → pick the repo
3. Framework preset: "Other" / static — no build command needed
4. Deploy

Either way you'll get a live `https://your-project.vercel.app` URL in
under a minute.

## Files

```
index.html      the whole page — content lives here
style.css       the "lab notebook" design system (paper background,
                serif headlines, monospace data readouts)
script.js       ~15 lines, just highlights the active nav section
assets/         the 4 live screenshots used in the project sections
```

## A note on the content

Every metric on this page was pulled directly from your project's own
output — `pipeline_metrics.json`, the AERIS live API response, the
NeuroCache benchmark baked into the app, and the trading simulator's
source code — not invented. If an interviewer asks a follow-up question
about any number on this page, you should be able to open the
corresponding file in your project and show them where it came from.
That's the whole point of building it this way: it holds up under
questioning, which a portfolio designed to survive an actual interview
needs to do.
