# Free Shipping A/B Test Analysis

## Overview
This repository contains the analysis and evaluation of an A/B testing experiment designed to assess the impact of a minimum order threshold for free shipping. The project investigates whether introducing a $35 minimum order requirement for free shipping can effectively increase the Average Order Value (AOV) without significantly increasing cart abandonment. By analyzing the treatment and control groups, we aim to provide actionable insights for decision-makers regarding this policy change.

## Why Does This Issue Matter?
Rising supply chain and shipping costs are a concern for businesses, impacting profitability and customer satisfaction. Implementing a minimum order threshold for free shipping can encourage customers to spend more, helping offset shipping expenses. However, setting a threshold may also discourage purchases if customers are unwilling to meet it, leading to increased cart abandonment. This analysis provides valuable insights to help balance increased order value with customer retention.

## Dataset
The dataset consists of simulated transaction data for a skincare brand, covering orders made in January and February 2024. Key features include:
- **Customer ID**: Unique identifier for each customer.
- **Order Amount**: Total purchase amount for each order.
- **Cart Abandonment**: Indicates if the customer abandoned their cart before completing the purchase.
- **Session Duration**: Duration of the customer’s session on the site.
- **Free Shipping Eligibility**: Status of free shipping eligibility based on the $35 threshold (treatment group only).

The primary objective of this dataset is to compare the Average Order Value, cart abandonment rates, and session durations between the control and treatment groups.

## Methods
Our analysis involves statistical testing and exploratory data analysis to evaluate the impact of the free shipping threshold:
- **T-Test**: Used to compare the Average Order Value between the control and treatment groups and assess statistical significance.
- **Confidence Intervals**: Used to provide a range within which we can be confident that the true mean AOV lies for each group.
- **Data Visualization**: Histograms and bar plots to visualize the distribution of order amounts, cart abandonment rates, and session durations across groups.

## Key Files
- **notebooks/free_shipping_ab_test_analysis.ipynb**: Jupyter Notebook containing the full analysis, including data preprocessing, EDA, statistical testing, and visualization.
- **data/ab_test_skincare_final.csv**: CSV file containing the dataset with control and treatment group data.
- **reports/AB_Test_Report.pdf**: PDF report summarizing the findings, conclusions, and recommendations.

## Tools and Libraries
- **Python**: Main programming language used for data analysis and statistical testing.
- **pandas and numpy**: For data manipulation and numerical computations.
- **matplotlib and seaborn**: For data visualization and plotting.
- **scipy and statsmodels**: For statistical testing (t-test and Chi-square test).

## Results
- **Average Order Value**: The treatment group showed a significant increase in AOV, suggesting that the minimum order threshold encouraged customers to spend more.
- **Cart Abandonment Rate**: Cart abandonment increased in the treatment group, indicating that some customers were deterred by the threshold.
- **Session Duration**: There was no significant difference in session duration between groups, suggesting that the threshold did not impact browsing behavior.

## Business Impact
- **Increased Revenue**: The increase in AOV in the treatment group indicates potential for higher revenue if the threshold is applied.
- **Customer Retention Considerations**: The higher cart abandonment rate in the treatment group suggests a need for careful messaging or alternative strategies to mitigate potential drop-offs.
- **Cost Savings on Shipping**: By incentivizing higher order amounts, this policy can help reduce the cost impact of free shipping.
- **Long-Term Strategy**: These findings can inform future strategies for free shipping thresholds, with adjustments to minimize cart abandonment while maximizing revenue.

## Conclusion and Recommendations
Based on the analysis, the $35 free shipping threshold effectively increases AOV but also raises cart abandonment. We recommend implementing this threshold with targeted messaging to mitigate abandonment and exploring further A/B testing with different thresholds (e.g., $25) to find an optimal balance.
