# Fast-Food Marketing Campaign A/B Test

## Project Overview
This project analyzes the effectiveness of three marketing campaigns for a fast-food chain introducing a new menu item.  
Using A/B testing methodology, we evaluate sales performance across different promotions, weeks, store ages, and market sizes.  
The goal is to determine which promotion strategy works best and to provide actionable business recommendations.

## Dataset
- Source: [Kaggle – Fast Food Marketing Campaign A/B Test](https://www.kaggle.com/datasets/chebotinaa/fast-food-marketing-campaign-ab-test/data)  
- Key variables:
  - `Promotion`: one of three promotion strategies tested  
  - `MarketSize`: small / medium / large  
  - `AgeOfStore`: store age in years  
  - `Week`: one of four weeks during the campaign  
  - `SalesInThousands`: weekly sales for the new menu item (in thousands)  

## Methodology
1. **Data Exploration**
   - Distribution of sales
   - Sales distribution by promotion
   - Sales trend across weeks
   - Sales vs. store age  
2. **Statistical Testing**
   - One-way ANOVA across promotions  
   - Post-hoc Tukey HSD to compare pairwise differences  
3. **Regression Analysis**
   - Sales explained by promotion, market size, and store age  
   - Interaction terms for heterogeneity (Promotion × MarketSize, Promotion × AgeOfStore)  
4. **Heterogeneity Analysis**
   - Effectiveness of promotions by market size  
   - Effectiveness of promotions across different store ages  

## Key Findings
- **Promotion 1 consistently outperforms Promotion 2** and is comparable to Promotion 3.  
- **Promotion 2 significantly underperforms** across all subgroups.  
- **Market size strongly drives sales**: large markets generate much higher sales than medium and small markets.  
- **Store age does not have a significant effect overall**, though older stores respond slightly better to Promotion 2.  

## Business Insights
- Adopt **Promotion 1 as the default campaign strategy**, with Promotion 3 as an alternative.  
- Avoid Promotion 2 in general, but consider targeting **older stores** where it performs better.  
- Prioritize campaign spending in **large markets**, where the return on investment is highest.  

## How to Run
- Open `Project.ipynb` in Jupyter Notebook or JupyterLab.  
- All analysis, visualizations, and results are contained in the notebook.  

## License
This project is for educational purposes. Dataset provided by [Kaggle](https://www.kaggle.com/datasets/chebotinaa/fast-food-marketing-campaign-ab-test/data).  
