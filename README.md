# Top Rated IMDb Movies Analysis — Power BI Project

## Project Overview
This project provides an interactive business intelligence dashboard analyzing the financial return on investment (ROI), production budgets, box office gross, and critical reception across top-rated IMDb films. It enables producers, film investors, and entertainment analysts to discover which film genres, runtime categories, content ratings, and production companies deliver the highest financial efficiency relative to their capital outlay.

---

## Live Dashboard Link
Explore the interactive Power BI report directly in your browser:

[View Live Power BI Dashboard](https://app.powerbi.com/groups/me/reports/a52f423e-1f12-4c99-82f5-5fe6311b1687/7aacc7dc9b3ffe2eb8ca?ctid=96e7b82d-bfbf-4ce0-87c2-77981e8ab6b9&experience=power-bi)

---

## Key Performance Indicators (KPIs)
- Movie Count: 200 films evaluated
- Total Box Office: $53.91 Billion
- Total Budget: $8.60 Billion
- Total Profit: $45.31 Billion
- Overall Portfolio ROI: 527.01%

---

## Key Visualizations and Insights

1. Budgets by Genre (Bar Chart): Action, Adventure, and Crime lead in aggregate production budget allocations, while genres like Horror, Mystery, and Comedy operate on leaner funding.
2. Box Office by Budgets (Scatter Plot): Correlates capital invested against total revenue generated across genres, highlighting high-margin commercial outliers.
3. Film Distribution by Content Rating (Donut Chart): Breaks down the catalog representation across ratings (R at 49.5%, PG-13 at 18%, PG at 17%, G at 15%).
4. Median ROI by Content Rating (Line Chart): Compares commercial efficiency across MPAA ratings, demonstrating varying financial yield patterns between general-audience and restricted releases.
5. Median ROI and Average Rating by Runtime Category (Combo Chart): Analyzes trade-offs across Short, Normal, and Long film lengths against critical IMDb rating averages and median return multiples.
6. Top Production Companies by ROI (Summary Table): Identifies historically high-performing production houses (such as Selznick International Pictures, Zanuck/Brown Productions, and Asghar Farhadi Productions) based on return efficiency.

---

## Tech Stack and Data Modeling
- Platform: Microsoft Power BI
- Data Source: Top Rated IMDb Movies Dataset
- Transformations: Power Query (data cleaning, type casting, handling currency conversions, handling missing values)
- Calculated Measures (DAX):
  - Total Profit = [Total Box Office] - [Total Budget]
  - Portfolio ROI = DIVIDE([Total Profit], [Total Budget], 0)
  - Runtime Grouping: Short, Normal, Long
