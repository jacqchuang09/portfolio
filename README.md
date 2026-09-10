# Jacqueline Chuang — Portfolio ✿

A playful, hand-drawn, draggable-canvas personal site.

## What's in this folder
```
jacqueline-portfolio/
├── index.html        ← the whole site (one file)
├── photos/           ← your photos (already added & web-optimized)
└── README.md         ← this file
```

## Preview it locally
Double-click `index.html` to open it in your browser. That's it.
(If photos ever look missing when opening the file directly, run a tiny local server
instead: open Terminal, `cd` into this folder, run `python3 -m http.server 8000`,
then visit `http://localhost:8000`.)

---

## How to put it on the internet

Pick ONE. Easiest first.

### Option 1 — Netlify Drop (no account math, ~60 seconds) ⭐ recommended
1. Go to **https://app.netlify.com/drop**
2. Drag this entire **`jacqueline-portfolio`** folder onto the page.
3. Done. You get a live URL like `random-name-123.netlify.app`.
4. (Optional) Make a free account to rename it to something like `jacquelinechuang.netlify.app`,
   or connect a custom domain you own.

### Option 2 — Vercel
1. Make a free account at **https://vercel.com**.
2. Install the CLI: `npm i -g vercel`
3. In Terminal, `cd` into this folder and run `vercel`. Follow the prompts.

### Option 3 — GitHub Pages (best if you want it version-controlled)
1. Create a repo on GitHub (e.g. `portfolio`).
2. Upload the contents of this folder to it (drag files into the GitHub web uploader is fine).
3. Repo → **Settings → Pages → Source: main branch / root** → Save.
4. Your site appears at `https://<your-username>.github.io/portfolio/`.

### Custom domain (e.g. jacquelinechuang.com)
- Buy a domain (Namecheap, Cloudflare, Google Domains, etc.).
- In Netlify/Vercel/GitHub Pages settings, add the custom domain and follow their DNS steps.
- All three host HTTPS for free.

---

## Editing your content later
Everything lives in `index.html`. Open it in any text editor and search for:
- **`const BUILDS`** — your device projects
- **`const RESEARCH`** — internships / labs
- **`const WINS`** — awards / trophy shelf
- **`const INTO`** — interest stickers
- **`PHRASES`** — the rotating typewriter roles under your name
- **`photo(...)`** calls — each polaroid (filename + caption)

### Swapping / adding a photo
1. Drop the new image into the `photos/` folder.
2. Keep files web-friendly: `.jpg`, ideally under ~1 MB and max ~1500px wide.
   (On a Mac you can shrink one in Terminal:
   `sips -s format jpeg -Z 1500 -s formatOptions 80 input.jpg --out photos/output.jpg`)
3. Point a `photo("photos/yourfile.jpg", ...)` line at it.

## Current photo map
| file | where it shows |
|---|---|
| locus-selfie.jpg / locus-team.jpg | about + Locus Suit flagship |
| research-poster.jpg / lab-rig.jpg | research zone |
| venturewell.jpg / bmes.jpg | wins zone |
| liondance-team.jpg / liondance-stage.jpg | life |
| soccer.jpg / tsa-formal.jpg / tsa-newbies.jpg | life |
| newgen-selfie / -crew / -science / -kids3 / -cart .jpg | teaching |

## Still to add (placeholders welcome)
- GitHub / personal site links (I only had email + LinkedIn + Locus Suit).
- A solo photo of you for the "about" card if you'd prefer that over the team selfie.
