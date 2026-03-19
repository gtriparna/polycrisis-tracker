# Global Polycrisis Cascade Tracker

Interactive tracker showing how five simultaneous global crises interact and amplify each other — traced 10 layers deep.

**Research & Analysis:** Triparna de Vreede, Ph.D., University of South Florida

## Deploy to Netlify (2 minutes)

### Option A: Drag and Drop (Easiest)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag this entire `polycrisis-tracker` folder onto the page
3. Done. You'll get a URL like `random-name.netlify.app`
4. Click "Site settings" → "Change site name" to customize (e.g., `polycrisis-tracker.netlify.app`)

### Option B: GitHub + Auto-Deploy
1. Push this folder to a GitHub repository
2. Go to [app.netlify.com](https://app.netlify.com) → "Add new site" → "Import from Git"
3. Select your repo → Deploy
4. Every time you push changes, Netlify auto-deploys

## Deploy to Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in this folder
3. Follow the prompts
4. Or: push to GitHub and import at [vercel.com/new](https://vercel.com/new)

## Deploy to GitHub Pages (Free)

1. Create a GitHub repo (e.g., `polycrisis-tracker`)
2. Push this folder's contents to the repo
3. Go to Settings → Pages → Source: "Deploy from a branch" → Branch: main → Folder: / (root)
4. Your URL: `yourusername.github.io/polycrisis-tracker`

## Updating the Tracker

The tracker is a single `index.html` file. To update:
1. Edit the data arrays at the top of the `<script>` section
2. Change layer statuses (`happened`, `happening`, `developing`, `emerging`, `projected`)
3. Add new events to the `EVENTS` array
4. Update the date in the header
5. Push/redeploy

## Structure

```
polycrisis-tracker/
├── index.html          # Everything — self-contained, no build step
├── README.md           # This file
└── netlify.toml        # Netlify config (optional)
```

No build step. No npm install. No dependencies to manage. Just one HTML file with React loaded from CDN.
