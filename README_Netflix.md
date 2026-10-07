# Netflix Content Strategy Analysis

Exploratory data analysis of Netflix's movie and TV show catalog to understand its composition, content additions, regional contributions, genre mix, and acquisition timing. The project uses Python to turn catalog-level data into business observations and recommendations.

## Project Objective

Analyze the Netflix title catalog to understand how its content strategy has evolved and identify patterns that may inform future content investment and global expansion.

## Business Questions

- How is the catalog divided between Movies and TV Shows?
- How have movie releases and catalog additions changed over time?
- Which countries contribute the most titles, and how do their leading genres differ?
- Which genres are most represented among Movies and TV Shows?
- How do content ratings and movie runtimes compare?
- When are TV Shows most often added to the catalog?
- How much time typically passes between a title's release and its addition to Netflix?
- How has the mix of Movies and TV Shows among additions changed in recent years of the dataset?

## Dataset

The project uses `netflix.csv`, a catalog dataset with **8,807 titles and 12 columns**. Fields include title type, title, director, cast, country, date added, release year, rating, duration, genres, and description. The dates and findings reflect the historical dataset supplied with the project; this is not a live snapshot of Netflix's current catalog.

The report identifies missing values in director, cast, country, date added, rating, and duration. Missing data was retained where possible and excluded only for analyses requiring the relevant field. Multi-value fields such as country, cast, director, and genre were split or expanded for relevant comparisons. Fourteen records with an impossible negative gap between release year and year added were excluded from that timing analysis. No duplicate rows were found.

## Key Findings

- Movies account for **69.6%** of titles in the catalog; TV Shows account for **30.4%**.
- Movie releases in the catalog rose sharply after 2015, with the largest counts around 2017–2018; counts declined after 2018.
- December had the most TV Show additions in the dataset, closely followed by July and September. Additions occurred throughout the year.
- International Movies were the most common movie genre, while International TV Shows led among TV Show genres. Drama and comedy also appeared prominently across both types.
- The overall catalog remains movie-heavy, but TV Shows' share of yearly additions increased from **25.0% in 2018** to **33.7% in 2021**.
- The median gap between release and addition was **0 years for TV Shows** and **2 years for Movies**. The report excluded 14 records with negative gaps from this comparison.
- Movie median runtimes across the five most common ratings were broadly similar, roughly **90–105 minutes**.
- The genre trend analysis found that International Movies peaked at roughly **670 additions in 2018**.

## Recommendations from the Analysis

- Prioritize further TV Show production and acquisition as the category's share of new additions grew in the analyzed years.
- Continue investing in international content, especially through partnerships in markets already contributing distinct content strengths.
- Maintain a mix of genres rather than concentrating the catalog in only the largest categories.
- Explore ways to reduce movie acquisition delays while retaining older titles that add catalog value.
- Use runtime as a storytelling decision; the analysis found similar median movie runtimes across major audience ratings.

These recommendations are based on descriptive patterns in the dataset. The analysis does not establish why the trends occurred or measure viewer engagement, title performance, or profitability.

## Skills and Tools

- **Python** for data analysis
- **Pandas** and **NumPy** for data cleaning and transformation
- **Matplotlib** and **Seaborn** for charts and exploratory visualization
- Missing-value and duplicate checks
- Date parsing and time-based feature creation
- Exploding multi-value columns for country, cast, director, and genre analysis
- Grouping, aggregation, distribution analysis, and business interpretation

## Repository Structure

```text

netflix-content-strategy-analysis/
├── README.md
├── netflix_analysis.ipynb
└── netflix.csv
```

The notebook `netflix_analysis.ipynb` is the exported Google Colab analysis and contains the code, charts, findings, and recommendations. The separate PDF report is omitted because it overlaps with the notebook.

## How to Review the Project

1. Read this README for the project question and headline findings.
2. Open `netflix_analysis.ipynb` to review the Colab code, analysis, visualizations, and recommendations.
3. Use `netflix.csv` as the dataset referenced by the notebook.

## Author

**Aravinth Baskar**

