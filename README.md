# Benetech Food Per Diem Calculator

A browser-based tool for Benetech employees to calculate food per diem reimbursements and generate expense summaries for submission in Concur.

**Live tools:**
- **USA:** https://benetech.github.io/PerDiem/PerDiem-USA.html
- **International:** https://benetech.github.io/PerDiem/PerDiem-International.html

---

## Features

- **US rates** — fetched live from the [GSA Per Diem API](https://open.gsa.gov/api/perdiem/) by fiscal year and location
- **International rates** — 228 countries sourced from the [US State Dept Per Diem database](https://allowances.state.gov/web920/per_diem.asp)
- **Daily meal grid** — one row per travel day with checkboxes to mark meals that were provided
- **Reimbursement summary** — calculates daily totals accounting for provided meals, with a grand total
- **Export to image** — saves the summary as a PNG for attaching to Concur expense items
- **Concur next steps** — step-by-step guidance for submitting the expense report after saving the image
- **Accessible** — WCAG 2.2 AA compliant, screen reader tested, keyboard navigable, dark mode supported

---

## How to Use

1. Enter your **Name**, **Conference**, and **Project Code**
2. Select your **Begin** and **Return Travel Dates**
3. Choose your **Country**, **State** (US only), and **City**
4. Click **Submit** to look up the per diem rates
5. In the **Daily Meal Grid**, check any meals that were provided (e.g. conference breakfast)
6. Click **Calculate** to generate the Reimbursement Summary
7. Click **Export Summary as Image** to save a PNG receipt
8. Follow the **Next Steps** to create the expense report in Concur

---

## Files

| File | Description |
|------|-------------|
| `PerDiem-USA.html` | USA calculator — rates fetched live from the GSA Per Diem API |
| `PerDiem-International.html` | International calculator — rates embedded from the US State Dept |

---

## Updating International Rates

International per diem rates are embedded in `PerDiem.html` and sourced from the US State Department. They typically update **January 1** and **July 1** each year. The tool displays a warning when the data may be out of date.

To refresh: open this project in Claude Code and say:
> *"Please refresh the international per diem rates in PerDiem.html"*

Claude will re-scrape the State Dept website and update the embedded data automatically.

---

## Updating US Rates

US rates are fetched **live** from the GSA Per Diem API on every search — no manual updates needed.

---

## Version History

Versions are tracked automatically in the `APP_VERSION` constant inside `PerDiem.html` and displayed in the app header.

---

## Created By

Charles LaPierre — Benetech  
Built with [Claude Code](https://claude.ai/claude-code)
