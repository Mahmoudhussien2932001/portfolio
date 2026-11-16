# Mahmoud Hussien Marof — Portfolio

Static site (HTML/CSS/JS + Three.js from CDN). No build step.

## Deploy on Vercel
**Option A — Dashboard:** vercel.com → Add New → Project → upload/import this folder (or push it to a GitHub repo and import it). Framework preset: **Other**. Build command: none. Output directory: `./`.

**Option B — CLI:**
```
npm i -g vercel
cd portfolio
vercel        # preview
vercel --prod # production
```

## Files
- `index.html` — the whole site (EN/AR content lives in the `I18N` and `PROJECTS` objects in the script)
- `assets/me.jpg` — profile photo
- `assets/projects/*.jpg` — project screenshots
- `favicon.svg`

## Adding the CV
1. Put the PDF at `assets/Mahmoud-Hussien-CV.pdf`
2. In `index.html`, change `<a class="btn" href="#" id="cvBtn">` to
   `<a class="btn" href="assets/Mahmoud-Hussien-CV.pdf" id="cvBtn" download>`
3. Delete the line that starts with `$("#cvBtn").addEventListener`
