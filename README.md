# Power BI — Supply Chain View

Part of the **Business Insights 360** Power BI project. This repo isolates the **Supply Chain** dashboard for focused viewing.

**Live dashboard:** https://app.powerbi.com/view?r=eyJrIjoiZTRmOWQzOWMtZGIxYi00NTIyLWE0OWQtNjA0YzcwYjVkMGVjIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9 (open the report, then click **Supply Chain** in the top navigation bar)

![Supply Chain View](https://github.com/user-attachments/assets/ac2db02f-126b-4e51-9230-3226c48b6832)

## Key insights

Compared forecast accuracy against the actual dollar exposure of forecast misses, by segment:

- **Accuracy % improved, but the dollar exposure got worse.** Forecast Accuracy rose from 72.99% to 80.21% YoY, yet Absolute Error grew from $5.74M to $10M (+70.3%) as the business scaled roughly 3x. A rising accuracy percentage alone would have hidden this — the real financial exposure of forecast misses nearly doubled.
- **Accessories is the stockout risk to watch.** It carries the largest net forecasting error (-2.13M units, under-forecast) and is flagged Out-of-Stock risk — on one of the company's two largest revenue segments.
- **Most-improved isn't always healthiest.** Networking posted the biggest forecast-accuracy jump of any segment (52.5% → 90.4% YoY, +37.9pp) but flipped to Excess Inventory risk from over-forecasting — the improvement came with a new problem.
- **The portfolio is split between overstock and stockout.** Storage and Desktop run Excess Inventory risk (over-forecast); Accessories, Notebook, and Peripherals run Out-of-Stock risk (under-forecast) — a single company-wide forecasting adjustment would fix one problem while making the other worse. This needs segment-specific tuning.

## Dashboard scope

Forecast Accuracy%, Net Error, and Absolute Error KPIs, an accuracy/net-error trend chart, and risk-flagged key metrics by customer and by product. Filterable by Region, Year, Quarter, Last Year, Target, Stores, Category, YTG, and YTD.
