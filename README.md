# Blue Ocean Strategy Workbench

A single-file, browser-based toolkit for running a full **value-innovation analysis** — from mapping your current value proposition against peers, through designing a defensible to-be position, to auditing capabilities, focusing product owners, and tracking the move over time.

No install, no build step, no backend. One HTML file that runs entirely in the browser. Bilingual **EN / UA**.

> **Live demo:** `https://<your-username>.github.io/blue-ocean-workbench/`
> Click **Load example** in the app to explore a worked case (monobank vs PrivatBank / PUMB / Raiffeisen — illustrative data, fully editable).

---

## What it does

The workbench is organised as an eight-step strategy workflow:

| Step | Tool | Purpose |
|------|------|---------|
| 01 | **Strategy Canvas + ERRC grid** | One master table: score each competing factor 0–10 for your company, each peer **and the to-be level**, side by side. Add a short note per factor, drag rows to reorder, and classify each factor as Eliminate / Reduce / Raise / Create. The value curves draw live. |
| 02 | **To-be canvas + Barriers register** | Read-only recap of now vs to-be with the uplift, the to-be value curve overlaid on today and the peer average, plus a barriers-to-imitation register (9 moat types, 1–5 strength) for every Raise/Create factor. |
| 03 | **Portfolio map — current** | Pioneer–Migrator–Settler bubble chart for all players. X = value-innovation level, Y = market/revenue share, bubble size = revenue. |
| 04 | **Portfolio map — future** | Your products only, with migration arrows from today's position toward the target. |
| 05 | **Value deployment** | Focus the organisation on the value factors. Toggle between a simple **Value-Deployment matrix** (units × factors → owner / objective / KPI) and a **Hoshin Kanri X-matrix**. |
| 06 | **Capabilities & resources** | Existing vs to-be audit split into **People / Technology / Assets / Processes**, each item flagged with a gap priority. |
| 07 | **Product stages** | Product-owner focus matrix across **Idea refinement → Idea development → Deployment → Go-to-market**: owner focus, objectives, key activities and an exit KPI/gate per stage. |
| 08 | **Measurement** | Take dated snapshots; a dashboard trends value lead, barrier strength, portfolio mix by zone, and deployment completion over time. |

---

## Using it

- **Load example** — fills every tool with an illustrative banking case so you can see the shape of the output.
- **New / clear** — start a blank project.
- **Export JSON / Import JSON** — save your work to a file and reload it later or on another device.
- **Save as PDF** — print-optimised layout; use your browser's "Save as PDF" destination. Each tool prints as its own page block.
- **EN / UA** — switches the interface language. Your own text (factor names, notes, products, etc.) is left as you typed it.
- **Reorder factors** — drag the ⠿ handle on any factor row in step 01; the new order flows through every table and chart.
- **Factor notes** — keep names short; the note shows as a footnote under the canvas and as a tooltip on the chart points.
- Work **autosaves** to your browser's local storage between sessions.

---

## Publishing on GitHub Pages

Using only the GitHub website (no git required):

1. Create a new **public** repository, e.g. `blue-ocean-workbench`.
2. **Add file → Upload files**, drag in `index.html` (and this `README.md`), then **Commit changes**.
3. **Settings → Pages → Source:** *Deploy from a branch*, branch **main**, folder **/ (root)**, **Save**.
4. Wait ~1 minute; the live URL appears on that settings screen:
   `https://<your-username>.github.io/blue-ocean-workbench/`

The file is named `index.html` so Pages serves it at the repo root with nothing extra in the path.

---

## Technical notes

- **Stack:** plain HTML / CSS / vanilla JavaScript, with [Chart.js](https://www.chartjs.org/) and Google Fonts loaded from CDNs.
- **Connectivity:** an internet connection is needed to render charts (Chart.js is loaded from a CDN). All logic and data handling are local.
- **Data:** stored in each visitor's own browser (`localStorage`). Nothing is sent anywhere. Anyone opening the link starts with a blank workbench and can use **Load example** or **Import JSON**. Older saved files load fine — missing sections are filled in automatically.
- **Browser support:** any current Chrome, Edge, Firefox, or Safari.

---

## Framework background

The tools follow the value-innovation logic of *Blue Ocean Strategy* (Kim & Mauborgne): the Strategy Canvas and Four Actions (ERRC) framework for steps 01–02, the Pioneer–Migrator–Settler map for steps 03–04, Hoshin Kanri strategy deployment for step 05, a capability/resource gap audit for step 06, and a stage-gate product-owner focus matrix for step 07. The example data is illustrative placeholder positioning to demonstrate the tools, not researched figures.

---

## License

MIT
