# Personal Calendar for Sanjit Chitturi

A single-file, minimal, and slightly playful calendar that **auto-crosses past days**, lets you **manually mark days**, and shows helpful lifetime statistics — **starts from April 9, 2005**.

---

## Features

* Single-file drop-in (`index.html`). No build step, no dependencies.
* Automatically treats any day **before today** as completed (visually muted).
* Click any calendar day to **toggle a manual completion** (overrides/adds to auto-completed days).
* **Lifetime stats**: total days since start date, passed days, manual marks, completion %, current & longest manual streaks.
* **Export / Import** manual marks as JSON so you can move them between devices.
* Simple Reset button to clear manual marks stored in your browser.
* Clean, modern UI with subtle playful touches.

---

## Quick start (3 steps)

1. **Download** or copy `index.html` into this repo.
2. Open `index.html` in your browser to run locally.
3. (Optional) Push this repo to GitHub and enable **GitHub Pages** (Settings → Pages) to host the page and link it from your profile README.

---

## How to use

* Click any day to toggle a manual mark. Past days (strictly before today) are automatically shown as completed.
* Use the **Export** button to download your manual marks as `milestone-marks.json`.
* Use **Import** to load a previously-exported JSON file (this replaces your current manual marks — you will be prompted to confirm).
* Use **Reset** to clear manual marks stored in this browser.
* Navigation: Prev / Next month, Jump to Start (Apr 9, 2005), and Today.

---

## Hosting on GitHub Pages

1. Create a repository (for example `milestone-calendar`) and add `index.html` at the repo root.
2. Push to GitHub.
3. In the repository settings → **Pages**, choose the branch (usually `main`) and the root folder, then **Save**.
4. GitHub will publish a site at `https://<your-username>.github.io/<repo-name>/` (example snippet for README):

```md

```

Replace `<your-username>` and `<repo-name>` with your details.

---

## Customization (easy)

The file is intentionally tiny and easy to read. Common edits:

* **Change the start date**: open `index.html`, find the line near the top of the script with `const START = atMid(new Date(2005,3,9));` and change the date values (note months are 0-based, so `3` is April).
* **Week start**: change `WEEK_START` (0 = Sunday, 1 = Monday).
* **Styling**: edit the CSS inside the `<style>` block to change colors, spacing, or fonts.

---

## Data & privacy

* Manual marks are stored only in your browser's `localStorage` under the key: `milestone:marks:final`.
* Nothing is sent to any server by default.
* If you export and upload the JSON somewhere, treat it like any personal file — it contains the dates you manually marked.

---

## Troubleshooting

* **Marks disappeared?** Check that `localStorage` is enabled and you didn't clear site data. Import a previously exported JSON to restore.
* **Export file cannot be read** — open it in a text editor to verify valid JSON. The import will refuse invalid JSON.
* **Page not updating time** — the page uses your browser clock; refresh if your device time changed.

---

## Contributing

This project is intentionally small. If you want features (heatmap, badge generator for README, dark mode toggle, smaller/minified build), open an issue or submit a PR.

If you’re new to GitHub, I can provide exact steps to:

* Create a repo
* Push this file
* Turn on Pages
* Add a link/badge to your profile README

---

## License

This repo is licensed under the **MIT License** — feel free to use it for personal projects and forks.

---
