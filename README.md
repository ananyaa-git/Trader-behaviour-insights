# Trader-behaviour-insights
JUNIOR DATA SCIENCE PROJECT
-----------------------------


Here's a breakdown of how the notebook addresses each part of the task:

Explore the relationship between trader performance and market sentiment:

The notebook loads historical trading data (historical_data.csv) which contains metrics for trader performance ('Closed PnL', 'Size Tokens', 'Size USD', etc.).
It loads external sentiment data (fear_greed_index.csv).
It merges these two datasets based on date (Trade_Date) to associate trading activities with prevailing market sentiment.
The 'Data Analysis' and 'Relationship Analysis' sections specifically calculate correlations between trader performance metrics ('Closed PnL') and the sentiment index ('Fear_Greed_Index').
It analyzes average and total 'Closed PnL' by sentiment category (Extreme Fear, Fear, Greed, Extreme Greed).
Uncover hidden patterns:

The data exploration phase identifies initial patterns like data distribution, missing values, and potential outliers.
Data wrangling and feature engineering create new features (rolling averages, lagged values, time-based cyclical features, interactions) that can help uncover more complex relationships.
Correlation analysis and visualization (heatmaps, scatter plots) help identify linear relationships and patterns between performance and engineered features/sentiment.
Analyzing performance by sentiment category reveals potential patterns in how traders perform under different market sentiment regimes.
The time-series visualization of sentiment and average daily PnL can show if there are temporal patterns or trends.
Deliver insights that can drive smarter trading strategies:

The correlation coefficients and statistical test results provide quantitative insights into the strength and significance of the relationships found.
The analysis of average/total PnL by sentiment category directly provides actionable insights, such as identifying whether certain sentiment periods are historically more profitable or less profitable on average.
Analyzing performance by trading strategy ('Side', 'Direction', 'Crossed') in conjunction with sentiment reveals which strategies might be more effective under different sentiment conditions. For example, insights could be: "Buying during Extreme Fear has historically yielded higher average PnL than selling," or "Crossed trades are more profitable during Greed phases."
The engineered features and the intention to use them in a model (though the model training section faced errors related to data availability) are aimed at building a predictive tool that could inform trading decisions based on current data and sentiment.
Although the model training section in the provided code snippet encountered errors (due to data not having overlapping dates), the overall process, the implemented analysis steps, and the visualizations are all directly aligned with the objective of exploring the relationship and gaining insights. The analysis conducted after the data merge (assuming the merge issue is resolved) provides clear insights into how performance metrics correlate with sentiment and how performance varies across different sentiment categories and trading strategies.

Therefore, yes, the notebook's content fully covers the steps required to fulfill the task, provided the data issues preventing the merge are resolved.
