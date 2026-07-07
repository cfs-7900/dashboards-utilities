# 7900 Windrose Ave — Utility Dashboard

Interactive utility consumption dashboards for **7900 Windrose Ave, Plano TX 75024**.

Tracks electricity, water, compost, and recycling across time — built as self-contained HTML files that open in any browser with no internet required.

---

## How It Works

1. **You upload invoices** into the appropriate `input-data/` subfolder
2. **Claude reads them** and generates updated dashboards
3. **Finished dashboards** appear in `output-data/` — open any `.html` file directly in your browser

---

## Folder Structure

```
7900-Windrose-Utility-Dashboard/
├── input-data/
│   ├── Electricity/       ← drop electricity PDFs here
│   ├── Water/             ← drop water PDFs here
│   ├── Compost/           ← drop compost PDFs here
│   └── Recycle/           ← drop recycling PDFs here
├── output-data/           ← finished dashboards saved here
└── sample-dashboard/      ← reference example (do not modify)
```

---

## Dashboard Files

After each update, `output-data/` will contain:

| File | What It Shows |
|---|---|
| `index.html` | **Master dashboard** — all utilities in one view |
| `electricity.html` | Electricity usage and cost over time |
| `water.html` | Water consumption and cost over time |
| `compost.html` | Compost service history |
| `recycle.html` | Recycling service history |

Open any file directly in Chrome, Edge, or Safari — no internet or server needed.

---

## Adding New Data

1. Save the new invoice PDF to the correct `input-data/` subfolder
2. Tell Claude: *"Update the dashboards"* (or *"New invoice added to Water"*)
3. Claude will re-read all invoices and regenerate all 5 dashboard files

---

## Tips

- **File naming doesn't matter** — Claude reads the invoice content, not the filename
- **All years are always included** — dashboards show the full history, not just recent invoices
- **Year filter** — each dashboard has buttons to filter by year (All / 2023 / 2024 / 2025 / etc.)
- **No setup required** — just open the HTML files directly

---

*Property: 7900 Windrose Ave, Plano TX 75024 | Electricity: ENGIE Resources / Oncor | Water: City of Plano*
