# Blue Ocean Strategy Workbench

A single-file, browser-based toolkit for running a full **value-innovation analysis** — from mapping your current value proposition against peers, through designing a defensible to-be position, to deploying it across the organisation and tracking the move over time.

No install, no build step, no backend. One HTML file that runs entirely in the browser. Bilingual **EN / UA**.

> **Live demo:** `https://<your-username>.github.io/blue-ocean-workbench/`
> Click **Load example** in the app to explore a worked case (monobank vs PrivatBank / PUMB / Raiffeisen — illustrative data, fully editable).

---

## What it does

The workbench is organised as a six-step strategy workflow:

| Step | Tool | Purpose |
|------|------|---------|
| 01 | **Strategy Canvas + ERRC grid** | Score each competing factor 0–10 for your company and peers; draw the value curves; classify factors as Eliminate / Reduce / Raise / Create. |
| 02 | **To-be canvas + Barriers register** | Set target levels per factor; for every Raise/Create factor, log the moats that protect the lead and rate their strength (barrier-strength index). |
| 03 | **Portfolio map — current** | Pioneer–Migrator–Settler bubble chart for all players. X = value-innovation level, Y = market/revenue share, bubble size = revenue. |
| 04 | **Portfolio map — future** | Your products only, with migration arrows from today's position toward the target. |
| 05 | **Value deployment** | Focus the organisation on the value factors. Toggle between a simple **Value-Deployment matrix** (units × factors → owner / objective / KPI) and a **Hoshin Kanri X-matrix**. |
| 06 | **Measurement** | Take dated snapshots; a dashboard trends value lead, barrier strength, portfolio mix by zone, and deployment completion. |

---

## Using it

- **Load example** — fills every tool with an illustrative banking case so you can see the shape of the output.
- **New / clear** — start a blank project.
- **Export JSON / Import JSON** — save your work to a file and reload it later or on another device.
- **Save as PDF** — print-optimised layout; use your browser's "Save as PDF" destination. Each tool prints as its own page block.
- **EN / UA** — switches the interface language. Your own text (factor names, products, etc.) is left as you typed it.
- Work **autosaves** to your browser's local storage between sessions.

---

## Publishing on GitHub Pages

Using only the GitHub website (no git required):

1. Create a new **public** repository, e.g. `blue-ocean-workbench`.
2. **Add file → Upload files**, drag in `index.html`, then **Commit changes**.
3. **Settings → Pages → Source:** *Deploy from a branch*, branch **main**, folder **/ (root)**, **Save**.
4. Wait ~1 minute; the live URL appears on that settings screen:
   `https://<your-username>.github.io/blue-ocean-workbench/`

The file is named `index.html` so Pages serves it at the repo root with nothing extra in the path.

---

## Technical notes

- **Stack:** plain HTML / CSS / vanilla JavaScript, with [Chart.js](https://www.chartjs.org/) and Google Fonts loaded from CDNs.
- **Connectivity:** an internet connection is needed to render charts (Chart.js is loaded from a CDN). All logic and data handling are local.
- **Data:** stored in each visitor's own browser (`localStorage`). Nothing is sent anywhere. Anyone opening the link starts with a blank workbench and can use **Load example** or **Import JSON**.
- **Browser support:** any current Chrome, Edge, Firefox, or Safari.

---

## Framework background

The tools follow the value-innovation logic of *Blue Ocean Strategy* (Kim & Mauborgne): the Strategy Canvas and Four Actions (ERRC) framework for steps 01–02, the Pioneer–Migrator–Settler map for steps 03–04, and Hoshin Kanri strategy deployment for step 05. The example data is illustrative placeholder positioning to demonstrate the tools, not researched figures.

---

## License

Add your preferred license here (e.g. MIT) before sharing publicly.
