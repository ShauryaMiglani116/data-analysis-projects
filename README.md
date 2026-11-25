# Data Analysis & Machine Learning Projects

Three exploratory-analysis and machine-learning notebooks on real-world datasets.

| Notebook | What it does | Key tools |
|---|---|---|
| [Facebook Live Sellers Analysis](Facebook_Marketplace_Analysis.ipynb) | Engagement by upload hour, reaction/comment/share relationships, K-Means clustering of posts | pandas, scikit-learn |
| [Advertising → Sales Prediction](Sales_Prediction.ipynb) | Which ad channel drives sales; linear regression on different feature sets | pandas, scikit-learn |
| [Red Wine Quality](Wine_Quality_Prediction.ipynb) | Chemical drivers of quality; Decision Tree vs. Random Forest | pandas, scikit-learn |

## Highlights

- **Wine quality:** a Random Forest reaches 66% accuracy on the 6-class quality score, against 56% for a single Decision Tree. Alcohol content has the strongest positive correlation with quality (r = 0.48), and volatile acidity the strongest negative one (r = −0.39).
- **Advertising:** TV spend correlates at r = 0.90 with sales. A linear model on all three channels fits sales with R² = 0.90, while radio and newspaper alone reach only R² = 0.12.
- **Facebook posts:** videos draw about 40× more comments than photos on average (642 vs. 16), and posts uploaded around 7–8 pm get the most reactions.

## Running locally

```bash
pip install -r requirements.txt
jupyter notebook
```

The notebooks read their datasets from [`data/`](data/), so start Jupyter from the repository root.

## Datasets

| File | Source |
|---|---|
| `data/Facebook_Marketplace_data.csv` | *Facebook Live Sellers in Thailand*, UCI Machine Learning Repository |
| `data/advertising_sales_data.xlsx` | The *Advertising* dataset: TV, radio and newspaper spend vs. sales for 200 markets |
| `data/wine_data.csv` | *Wine Quality* (red wine subset), UCI Machine Learning Repository; Cortez et al., 2009 |
