## Machine Learning in Business: Oil Well Profitability Analysis

In this project, I worked as a data scientist for the OilyGiant mining company to determine the most profitable region for developing new oil wells. Using geological exploration data from three regions, I built and evaluated a machine learning model to predict oil reserve volumes and support a data-driven business decision.

A linear regression model was trained separately for each region to predict the volume of reserves in new wells. Model performance was evaluated using RMSE and the average predicted reserve volume. Based on model predictions, the top 200 wells were selected from a sample of 500 wells in each region to estimate potential profit.

To assess financial viability and risk, a profit calculation function was implemented using business constraints, including a fixed development budget and revenue per barrel. The bootstrapping technique (1,000 iterations) was applied to estimate the distribution of profit, calculate the average expected profit, construct a 95% confidence interval, and measure the probability of losses.

The final recommendation was made by selecting the region with a loss risk below 2.5% and the highest average profit. This approach ensures both profitability and controlled financial risk, aligning the model results with real-world business requirements.

