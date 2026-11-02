# Global Happiness Dashboard | Excel

**The world average hardly moved between 2006 and 2023, but individual countries changed a lot. Of 114 countries with data for both 2010 and 2023, Afghanistan fell by 3.3 points and Serbia rose by 2.0. Across all years, happiness is most closely linked with income (log GDP per capita, correlation 0.78), social support (0.72) and life expectancy (0.71).**

An interactive Excel dashboard built on World Happiness Report data, 2005–2023.

![Global Happiness Excel Dashboard](dashboard-preview.png)

## Data

| | |
|---|---|
| Source | World Happiness Report |
| Period | 2005–2023 |
| Countries | 165 |
| Observations (country-years) | 2,363 |

Indicators: happiness score (Life Ladder, 0–10), log GDP per capita, social support, healthy life expectancy, freedom, generosity, perceptions of corruption, positive and negative emotions. Some indicators have gaps, for example corruption is missing in 125 rows and life expectancy in 63, so averages for them are based on fewer rows.

## What I did

1. Kept the raw data untouched and cleaned it on a separate sheet (clearer column names, same values).
2. Created my own metrics:
   - **Happiness Tier:** Flourishing (7+), Happy (6–7), Stable (5–6), Vulnerable (under 5)
   - **Quality of Life Index:** social support 35%, freedom 25%, life expectancy (scaled 0–1) 25%, positive emotions 15%
   - **Emotional Balance Score:** positive emotions minus negative emotions
3. Built Pivot Tables and Pivot Charts for the yearly trend, country rankings and tier comparisons.
4. Compared each country's score in 2010 and 2023.
5. Put it together in one dashboard with 4 KPI cards: average happiness 5.48, happiest country Denmark (7.66 on average), 165 countries, 2005–2023.

## Key findings

**1. The global average is stable, but countries are not.** From 2006 to 2023 the world average stays between 5.2 and 5.7. Behind that flat line, countries moved in both directions between 2010 and 2023:

| Biggest falls | 2010 | 2023 | Change |
|---|---:|---:|---:|
| Afghanistan | 4.76 | 1.45 | -3.31 |
| Venezuela | 7.48 | 5.76 | -1.71 |
| Lebanon | 5.03 | 3.59 | -1.44 |

| Biggest rises | 2010 | 2023 | Change |
|---|---:|---:|---:|
| Serbia | 4.46 | 6.44 | +1.98 |
| Kosovo | 5.18 | 6.88 | +1.70 |
| Bulgaria | 3.91 | 5.59 | +1.68 |

**2. Two years look unusual because of who was surveyed.** 2005 has a high average (6.45) because only 27 countries, mostly richer ones, were surveyed. In 2020 the average rises to 5.73, but only 116 countries have data that year, compared with 143 in 2019. So these jumps say more about the sample than about the world.

**3. Nordic countries lead.** Denmark (7.66), Finland (7.62), Iceland (7.47) and Norway (7.46) have the highest average scores over the period.

**4. The happiest group is better on every indicator.**

| Tier | Country-years | Social support | Life expectancy | Freedom |
|---|---:|---:|---:|---:|
| Flourishing | 262 | 0.93 | 70.2 | 0.89 |
| Happy | 538 | 0.89 | 68.1 | 0.82 |
| Stable | 723 | 0.82 | 64.4 | 0.73 |
| Vulnerable | 840 | 0.71 | 57.5 | 0.68 |

**5. In the latest year, social support matters as much as income.** Over all years, log GDP per capita has the strongest correlation with happiness (0.78). In 2023 alone, social support (0.79) is just as strong as income (0.78).

## Files

- `Global_Happiness_Dashboard_.xlsx`: open the **Dashboard** sheet. The other sheets have the raw data, the clean data, the pivot analysis and the country changes.
- `dashboard-preview.png`: screenshot of the dashboard.

## Limitations

- Correlation is not causation. Richer countries also tend to have better health and social support, so the effects overlap.
- GDP is on a log scale, as in the original report.
- Country averages hide differences inside a country.
- Not every country has data for every year, so the yearly world average depends on which countries were surveyed.

**Tools:** Microsoft Excel (Pivot Tables, Pivot Charts, XLOOKUP, UNIQUE, AVERAGEIFS, KPI cards, scatter plots)
