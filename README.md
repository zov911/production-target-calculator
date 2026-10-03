# Production Target Calculator: Assembly Line Cases, Cycle Time & Staffing

**Live demo:** https://zov911.github.io/production-target-calculator/

A multi-line production planning tool for assembly and packing operations. Pick products for each line and instantly see daily and hourly case targets, cycle time, labor minutes per case, and how targets change with actual shift length and headcount.

## Features

- **Multi-line mode:** plan several product lines at once, with combined totals
- **Optional quantities** per line for order-based planning
- **Adjustments** for actual shift hours and actual people on the line, against a standard baseline (7 h, 10 people)
- **Summary table** with cycle time (min/sec), hourly rate, labor min/case, and time- and staff-adjusted targets
- **Formula reference** and a searchable product standards table (sample catalog)

## Formulas

```
Cycle time (min)  = shift minutes ÷ standard cases
Labor min / case  = cycle min × standard headcount
Adj. by staffing  = standard cases × actual people ÷ standard people
Adj. by time      = available minutes ÷ cycle min
```

## Tech

A single `index.html`: vanilla JS with no dependencies. The product catalog is a plain JS array, so it's easy to swap in your own SKUs and standards.

---

## Want a calculator like this for your operation?

I build production, capacity and planning tools around your real product catalog and line standards.

**Reach out → [zov911.com](https://zov911.com)**

© zov911. All rights reserved.
