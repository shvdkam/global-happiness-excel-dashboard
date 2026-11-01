# Global Happiness Dashboard | Excel

**Happiness follows money, but not only money. GDP per capita has the strongest link with a country's happiness score (correlation 0.78), and social support (0.72) and life expectancy (0.71) are almost as strong.**

An interactive Excel dashboard built on World Happiness Report data, 2005–2023.

![Global Happiness Excel Dashboard](dashboard-preview.png)

## Data

| | |
|---|---|
| Source | World Happiness Report |
| Period | 2005–2023 |
| Countries | 165 |
| Observations (country-years) | 2,363 |

Indicators: happiness score, GDP per capita, social support, life expectancy, freedom, generosity, corruption, positive and negative emotions.

## What I did

1. Cleaned the raw data on a separate sheet and kept the original untouched.
2. Created my own metrics:
   - **Happiness Tier:** Flourishing, Happy, Stable, Vulnerable
   - **Quality of Life Index**
   - **Emotional Balance Score**
3. Built Pivot Tables and Pivot Charts for trends, country rankings and tier comparisons.
4. Put it together in one dashboard with 4 KPI cards: average happiness 5.48, happiest country Denmark (7.66 on average), 165 countries, 2005–2023.

## Key findings

**1. Nordic countries lead.** Denmark (7.66), Finland (7.62), Iceland (7.47) and Norway (7.46) have the highest average scores.

**2. The happiest group is better on every indicator.**

| Tier | Social support | Life expectancy | Freedom |
|---|---:|---:|---:|
| Flourishing | 0.93 | 70.2 | 0.89 |
| Happy | 0.89 | 68.1 | 0.82 |
| Stable | 0.82 | 64.4 | 0.73 |
| Vulnerable | 0.71 | 57.5 | 0.68 |

**3. The global average is stable.** From 2006 to 2023 it stays between 5.2 and 5.7. The 2005 value (6.45) is higher only because just 27 countries, mostly richer ones, were surveyed that year.

## Files

- `Global_Happiness_Dashboard.xlsx`: open the **Dashboard** sheet. The other sheets show raw data, clean data and the pivot analysis.
- `dashboard-preview.png`: screenshot of the dashboard.

## Limitations

- Correlation is not causation.
- Country averages hide differences inside a country.
- Not every country has data for every year.

**Tools:** Microsoft Excel (Pivot Tables, Pivot Charts, calculated fields, KPI cards, scatter plot)
