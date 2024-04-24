# Analysis of Query Length and Response Time in GPT-4

This repository contains the data analysis project that explores the impact of query length on the response time of the GPT-4 model. The analysis aims to determine if there's a significant correlation between the number of tokens in a query and the time taken for GPT-4 to respond.

## Objective

The primary goal is to understand whether the length of the query, measured in tokens, significantly affects the response time of the GPT-4 model.

## Methodology

The analysis was conducted using the following steps:
- Data loading and preprocessing with Python libraries: Pandas, Seaborn, Matplotlib, and DuckDB.
- Data visualization through scatter plots and regression analysis to observe trends and variabilities.
- Statistical analysis to calculate the correlation coefficient and perform quartile analysis.

### Tools and Libraries Used
- **Pandas**: For data manipulation and analysis.
- **Seaborn and Matplotlib**: For data visualization.
- **DuckDB**: For SQL queries within a Python environment.

## Dataset

The dataset used in this analysis is named `total_tokens_vs_invoke_chain_time.csv`, which includes the following columns:
- `total_tokens`: The number of tokens in each query.
- `invoke_chain_time_in_seconds`: The response time for each query in seconds.

## Analysis Results

### Visualizations
1. **Scatter Plot**: Showcases the relationship between token count and response time.
   ![Scater_Plot](https://github.com/VladylenaHalchuk/Response-Time-in-GPT-4/assets/112247563/f677eff7-1635-4941-b24d-6a8e558e1b16)

   Concentration of points suggests shorter response times for queries with fewer tokens.
   As token count increases, response times show greater variability.
3. **Regression Plot**: Demonstrates the trend and variability in response time with increasing tokens.
   ![Regression_Plot](https://github.com/VladylenaHalchuk/Response-Time-in-GPT-4/assets/112247563/c8c4a8a7-0e21-4cf8-bc78-7503af0ae722)

   A positive trend line indicates response times tend to increase with more tokens.
   The wide confidence interval at higher token counts suggests more variability.
5. **Bar Plot**: Average response times segmented into quartiles based on token count.
   ![Bar_Plot](https://github.com/VladylenaHalchuk/Response-Time-in-GPT-4/assets/112247563/128afb4c-dca1-488f-b4c7-c7e784a9dc87)

   Quartile analysis does not show a consistent increase in response time with token count.


### Key Findings
- The correlation coefficient calculated was 0.245, indicating a weak positive linear relationship.
- While there is a trend of increasing response time with more tokens, the relationship is not strongly consistent.

## Conclusion

The findings suggest that the number of tokens does impact response time but not significantly enough to consider it the sole factor for optimization in GPT-4's response efficiency. Other factors may also play a significant role and should be considered in further studies.

## Recommendations

Further research is recommended to explore other variables that might affect the response time of GPT-4. Reducing the number of tokens alone may not significantly enhance response efficiency.

## How to Run This Project
[https://github.com/VladylenaHalchuk/Response-Time-in-GPT-4](https://github.com/VladylenaHalchuk/Response-Time-in-GPT-4/blob/main/Halchuk_GPT_time.ipynb)
### Requirements
Ensure you have Python installed, along with the necessary libraries:
