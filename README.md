# HanuAi-ML-Assessment

Submitted by **Velamala Balakrishna**

This repository has two tasks. Each task has an annotated notebook, a dataset and a written report.

## Task 1: BestBuy Canada Review Scraper and Sentiment Analysis

Product: Sony WH-1000XM5 headphones (bestbuy.ca)

| File | What it is |
|---|---|
| `Task1_Scraper_Sentiment_executed.ipynb` | Annotated notebook: Playwright + BeautifulSoup scraper, cleaning, sentiment analysis and aspect tags (already run) |
| `bestbuy_reviews_sentiment.csv` / `.xlsx` | Final dataset: 60 reviews with sentiment and category tags |
| `manual_reviews.xlsx` | The 60 reviews as collected, before analysis |
| `Task1_Report.docx` | Report: anti-scraping solutions, satisfaction drivers, pain points, recommendations, limitations |

**Important note:** BestBuy returned "Access Denied" to the automated browser, so I did not bypass it. I copied 60 reviews by hand from the product page and ran the same pipeline on them. The scraper code is included but was not tested on the live site.

**Results:** 53 positive, 6 negative, 1 neutral. Average rating 4.53 (58 rated reviews). The sentiment label blends VADER text scores with the star rating, because text alone missed the negative reviews.

## Task 2: EDA, Text Mining and Clustering

| File | What it is |
|---|---|
| `Task2_EDA_TextMining_Clustering.ipynb` | Annotated notebook: EDA, text mining, entity tagging, issue categories, TF-IDF K-Means clustering and root causes (already run) |
| `Hanuai task2 assignment.csv` | Original dataset |
| `Hanuai_task2_tagged.csv` / `.xlsx` | Updated dataset with extracted tags, issue categories and cluster IDs |
| `Task2_Stakeholder_Report.docx` | Report: findings, business impact, key learnings, future improvements |
| `figures/` | Charts used in the notebook and report |

## How to run

1. Install Python 3 and the packages: `pandas numpy scikit-learn matplotlib seaborn vaderSentiment openpyxl`
2. Open a notebook in VS Code or Jupyter and click **Run All**.
3. For Task 1, keep `manual_reviews.xlsx` in the same folder as the notebook.

Note: GitHub cannot preview large notebooks or Word and Excel files. Download them to open.