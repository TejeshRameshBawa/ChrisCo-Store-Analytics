# ChrisCo Store Analytics

Retail customer behaviour and store-performance analysis using Python and eight complementary visualisations. MSc Data Science (FinTech) coursework, University of Greenwich.

![Correlation heatmap of ChrisCo store summary metrics](preview.png)

## Business question

How do customer volumes differ across stores, and how do store size, staffing and marketing spend relate to those differences?

## What I did

- Combined five supplied datasets covering daily customer counts, marketing, overheads, floor space and staffing.
- Built an eight-chart narrative: segmented customer totals, distributions, daily trends, a high-volume-store comparison, a correlation heatmap, autocorrelation, resource-efficiency comparisons and a radar chart.
- Used Pandas and NumPy for preparation, Matplotlib and Seaborn for plotting, and hvPlot/HoloViews for interactive views.

## Findings

The project found correlations of approximately 0.94 or higher between customer volume and store size, staffing and marketing spend. Comparing customers per staff member and per square metre also highlighted trade-offs between absolute volume and resource efficiency.

These are associations within the coursework dataset. They do not establish that increasing marketing or staffing would cause a particular increase in customers.

## Explore the work

- [Portfolio report](portfolio-report.pdf): the written analysis and all eight visualisations.
- [Original notebook](COMP1800_DATA_VISUALISATION.ipynb).
- CSV inputs: `StoreDailyCustomers.csv`, `StoreMarketing.csv`, `StoreOverheads.csv`, `StoreSize.csv` and `StoreStaff.csv`.

## Run or inspect

1. Open the notebook in Jupyter or Google Colab. The saved outputs can also be inspected on GitHub.
2. Install the libraries imported by the notebook: `pandas numpy matplotlib seaborn hvplot holoviews bokeh` and Jupyter if running locally.
3. The original loading cells use coursework URLs. For a self-contained local run, change each `pd.read_csv(...)` URL to the matching CSV filename in this repository, retaining `index_col=0`.
4. Run cells from top to bottom. Interactive hvPlot output may require a live notebook rather than GitHub's static preview.

The original notebook is preserved. A clean execution in a newly created environment has not been verified, and library-version differences may require adjustments.

## Context

Academic analysis by Tejesh Ramesh Bawa. The preview is a figure extracted from the project report. The portfolio PDF omits the student identifier from its cover.
