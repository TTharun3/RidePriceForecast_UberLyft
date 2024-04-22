Introduction

The dynamic pricing model of ride-sharing companies like Uber and Lyft has transformed urban transportation. Unlike traditional public transport with fixed rates, ride-sharing prices fluctuate based on real-time demand and supply, leading to varying costs for the same trip at different times. Understanding the factors influencing these price changes can help consumers make cost-effective choices and enable these companies to refine their pricing algorithms. This report analyzes a dataset reflecting Uber and Lyft ride prices in Boston and investigates the factors affecting these prices, including time of day, weather conditions, and location.

Executive Summary

This report presents an in-depth analysis of ride-sharing prices from Uber and Lyft, using a dataset that captures the intricacies of dynamic pricing. The analysis reveals that time of day, weather conditions, and specific dates have significant impacts on pricing and ride demand. A Random Forest model was employed to predict ride prices, achieving an explanation of 90% of the variability in the data. Key findings indicate that Uber is preferred for longer distances and that weather conditions can notably influence the decision to book a ride.

Dataset Description

The dataset comprises real-time queries from the Uber and Lyft APIs, encompassing various types of rides, their prices, surge multipliers, and corresponding weather conditions. Data was collected in Boston for approximately one week in November 2018, using a custom Scala application. Although the primary focus was not on time-series analysis, the data provides a rich source for understanding the price dynamics in ride-sharing.

Data Preparation

Data cleaning and preparation steps were thorough, addressing missing values, anomalies, and appropriate transformations. Initial explorations included statistical summaries and data visualizations to understand data distributions and outliers. This groundwork ensured the reliability of subsequent analyses.

Data Analysis Methodology

The data analysis employed statistical techniques to identify trends and relationships within the dataset. The Exploratory Data Analysis (EDA) utilized a variety of visualization methods, such as bar charts and line plots, to uncover patterns related to ride prices across different cab types, destinations, sources, and weather conditions.

Exploratory Data Analysis (EDA)

EDA focused heavily on visualization, with bar plots comparing the average price of rides across different cab types, and line graphs assessing the impact of environmental factors like temperature, pressure, and wind speed on pricing. Notably, certain cab types showed a higher average price, and there was an observable trend of price variation with changes in weather conditions.

Model Selection

A Random Forest model was chosen for its ability to handle non-linear relationships and interactions between variables without extensive hyperparameter tuning. The model was assessed using cross-validation to ensure robustness and evaluated using standard metrics to confirm its predictive power.

Results and Recommendations

The model demonstrated a strong ability to predict ride prices, with weather conditions, time of day, and day of the week emerging as significant predictors. Recommendations include preferring Uber for longer distances and checking weather forecasts to anticipate price surges. Additionally, the analysis suggests avoiding rides during peak times on Mondays and Tuesdays due to higher costs.
