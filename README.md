# Worker Productivity Dashboard

A Power BI dashboard for tracking labor productivity across vehicle processing facilities. It measures how efficiently labor is scheduled and used relative to the number of vehicles released, and lets operations drill into the data by facility, car line, process, and time period.

<img width="1276" height="610" alt="image" src="https://github.com/user-attachments/assets/84afddf8-17bc-40f2-ac6a-3fd5732d22a3" />

## What it does

Vehicle processing runs on labor — vehicles need a set amount of work, and that work has to be scheduled and assigned to staff. This dashboard answers a few operational questions:

- Is labor being scheduled to match what's actually needed?
- How much labor are we spending per vehicle released, and is that trending up or down?
- Are production staff being fully assigned, or is there slack in the schedule?
- How do these numbers break down across facilities and car lines?

## Key metrics

The top row tracks the headline KPIs, each with 7-day and 30-day period-over-period comparisons and a trend strip across This Week, prior weeks, MTD, QTD, and YTD:

- **Needed / Scheduled labor** — how scheduled labor compares to labor actually needed
- **Productivity** — produced minutes against assigned minutes
- **Daily Plans Closed** — share of daily plans completed
- **% Days Production Staff Fully Assigned** — how often staff are fully assigned to work
- **Minutes per Released Vehicle** — labor spent per vehicle released, the core efficiency measure

## Interactivity

- **Per-vehicle toggle** — switch the per-vehicle metric between actual *labor* minutes and *assigned* minutes to compare planned vs. real labor spend
- **Metric selector** — the center trend chart swaps between metrics using the button panel on the right
- **Filters** — facility, car line, process, and date range slicers on the left, consistent with the rest of the dashboard suite
- **Summary tables** — breakdowns at the bottom split every metric out by car line and by facility for side-by-side comparison

## Tech

- Power BI · DAX · Power Query
- Data source: [your pipeline — e.g. Microsoft Fabric lakehouse fed from AS/400 / SharePoint]
- Refresh: [scheduled? how often?]

## Notes

Part of a suite of operational dashboards built for vehicle processing at Amports (Benicia Port). All dashboards in the suite share a common filter layout (facility, car line, date) for consistent navigation.
