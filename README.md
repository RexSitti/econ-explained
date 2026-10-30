# Econ, Explained

Short explainer videos for every chapter of Intermediate Macroeconomics, by Rex Sitti.
This repository is the course hub. The videos themselves live on YouTube.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole site (one page, no build step). |
| `chapters.csv` | Chapter numbers and titles. |
| `clips.csv` | Every clip: `chapter, clip, title, youtube_id`. |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is. |

## Releasing a clip

When a clip goes public on YouTube, open `clips.csv` on GitHub (pencil icon), find its row, and:

1. Paste the video ID into the last column. The ID is the part after `youtu.be/`
   (for `https://youtu.be/p3SY_KEKvTc` the ID is `p3SY_KEKvTc`).
2. Optionally replace the working title with the final YouTube title (wrap it in double quotes if it contains a comma).
3. Commit. The site updates in about a minute.

Rows with an empty `youtube_id` show as "Coming soon". The release counter and chapter bars update automatically.

## Turning on GitHub Pages (one time)

Settings → Pages → Source: "Deploy from a branch" → Branch: `main`, folder `/ (root)` → Save.
The site appears at `https://r3xstar.github.io/<repo-name>/`.

## Previewing locally

From this folder: `python3 -m http.server`, then open http://localhost:8000.
(Opening `index.html` directly from disk will not load the CSV files.)
