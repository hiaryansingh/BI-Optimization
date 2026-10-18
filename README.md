# Supply Chain BI Optimization Hub

A single-page tool for checking and speeding up Power BI reports: Report analyzer, DAX checker,
Model check, Lineage flowchart (with zoom, fit and full screen), Fabric CU guide and more.

Built by Aryan Singh.

## How to use it

- **Online:** open the GitHub Pages link for this repo (Settings → Pages shows it).
- **Offline:** download `index.html` and double-click it. It runs fully in your browser.

Your files (Performance Analyzer exports, PBIP projects, DAX) are read only inside your own browser.
Nothing is uploaded anywhere.

## Try it with the examples

The `examples` folder has made-up sample files (a fictional sales model, no real data), so anyone can
try every feature in a couple of minutes:

| File | Where to load it in the hub |
|---|---|
| `1-performance-analyzer-before.json` | **Report analyzer** → Load file |
| `2-performance-analyzer-after.json` | **Report analyzer** → Compare (the "after" run, once fixes are made) |
| `3-dax-measures.txt` | **DAX checker** → paste the text in |
| `4-vertipaq-column-stats.tsv` | **Model check** → paste into column stats |
| `5-sample-pbip-project.zip` (or the folder) | **Model check** → Open .zip / Open folder, then **Lineage** to see the flowchart |

To use your own reports: in Power BI Desktop, open **View → Performance analyzer → Start recording**,
click around, then **Export** the JSON. For Model check, save the report as a **Power BI project (.pbip)**.

## Push a project to GitHub from the page

On **Model check**, load a .pbip project (or the sample), then use **Push this project to GitHub**:
enter `username/repo`, a branch, a folder (for example `reports/sales`) and a fine-grained token with
**Contents: Read and write** for this repo only. The page sends everything as one commit, straight from
your browser to GitHub. It asks for confirmation before pushing to a public repo.

## Notes

- Only sample data is included. Don't commit company files, data or screenshots to this repo.
- Fonts, Mermaid diagrams and the zip reader load from public CDNs; without internet the page still
  works, with plainer fonts.
