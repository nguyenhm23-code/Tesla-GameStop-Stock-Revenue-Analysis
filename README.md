# Tesla and GameStop: Historical Stock Price and Revenue Analysis

Final assignment for **IBM Python Project for Data Science** on Coursera.

## Notebook

Open [Analyzing_Historical_Stock_Revenue.ipynb](Analyzing_Historical_Stock_Revenue.ipynb).
All six questions include code and saved results. Static charts are embedded for GitHub; rerunning also produces interactive Plotly charts.

## Assignment deliverables

| Question | Task | Image |
| --- | --- | --- |
| 1 | Tesla: yfinance, reset index, head() | [Q1](screenshots/question_1.png) |
| 2 | Tesla: web scraping, revenue cleaning, tail() | [Q2](screenshots/question_2.png) |
| 3 | GameStop: yfinance, reset index, head() | [Q3](screenshots/question_3.png) |
| 4 | GameStop: web scraping, revenue cleaning, tail() | [Q4](screenshots/question_4.png) |
| 5 | make_graph(tesla_data, tesla_revenue, 'Tesla') | [Q5](screenshots/question_5.png) |
| 6 | make_graph(gme_data, gme_revenue, 'GameStop') | [Q6](screenshots/question_6.png) |

The PNGs are code/result exports of the saved, executed notebook outputs.

## Run locally

Use Python 3.10 or newer:

```bash
python -m pip install -r requirements.txt
jupyter notebook Analyzing_Historical_Stock_Revenue.ipynb
```

Choose **Restart Kernel and Run All Cells**. Internet access is required for stock history and revenue HTML.

## Data and chart window

- Stock history uses `yf.Ticker(...).history(period='max', auto_adjust=True)`. Adjusted USD prices may change when the provider revises historical adjustments.
- Quarterly revenues come from the course HTML snapshots, with dollar signs and commas removed and values converted to numeric USD millions.
- The charts follow the lab window: prices through June 14, 2021; revenues through April 30, 2021.
- The GameStop revenue snapshot ends in April 2020. Later revenue values are not invented, and the comparisons do not establish causation.
- Saved outputs come from the previously executed assignment notebook. This publication pass reviewed and packaged them without a fresh live-data execution.

## Sources and attribution

- [IBM Skills Network lab template](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/Final%20Assignment.ipynb)
- [Tesla revenue snapshot](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/revenue.htm)
- [GameStop revenue snapshot](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/stock.html)
- [yfinance](https://github.com/ranaroussi/yfinance)

Original template: IBM Skills Network. Original author attribution and copyright notice are retained in the notebook.

