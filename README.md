
# WORLD HAPPINESS REPORT

 ![image](images/image2.jpg)


This project aims to provide an in-depth analysis of the happiness rates of countries around the world between 2020 and 2024 and  analyze the key factors influencing happiness levels across different countries and provide insights for policymakers, economists, and social scientists.


## Dataset Content
* Datasets are taken from Kaggle. The data is prepared by Gallup World Poll and Global Survey Research.

There are 5 csv files for the years 2020-2024.  They Have  eleven columns . Combined all csv files and added year column.



| Column Name                 | Description                                                           |
|-----------------------------|-----------------------------------------------------------------------|
| Country name                | Name of the Country                                                   |
| Happiness Rank              | The ranking of thecountry based on the happiness score                |
| HAppiness score             | The happiness scpre of the country (likely between 1 and 10)          |
| Upperwhisker                | Upper bound of the confidence interval                                |
| Lowerwhisker                | Lower bound of the confidence interval.                               |
| Economy(GDP per Capita)     | GDP per capita (a measure of economic prosperty)                      |
| Social Support              | Level of social support (e.g. relationships with family and friends.) |
| Health life expectancy      | Expectednumber of healthy life years.                                 |
| Freedom to make life choices| Freedom to make personal life choices.                                |
| Generosity                  | Generosity level(based on donations and willingness to help others)   |
| PErceptions of corruption   | Perceived level of corruption in the country                          |
| Year                        | The year to which the data belongs.                                   |




## Business Requirements
The business requirements should focus on understanding the factors that influence happiness scores and analyzing differences between countries. 

 ✅ Identify Key Factors Affecting Happiness

Determine which economic and social factors have the most significant impact on happiness levels.
Analyze the influence of GDP, social support, health, freedom, generosity, and corruption perceptions.
Compare countries with the highest and lowest happiness scores to understand the differences.

✅ Analyze Happiness Trends Over Time

Examine how happiness scores have changed between 2020 and 2024.
Assess the impact of global events, such as the COVID-19 pandemic, on happiness levels.

✅ Visualize Country Comparisons

Identify the happiest and least happy countries and evaluate geographic and economic influences.
Segment countries by continent or income level to detect patterns.

✅ Provide Data-Driven Policy Recommendations

Suggest policies that could improve happiness levels based on data insights.
Measure the impact of economic growth on happiness and propose strategies to enhance well-being.

## Hypothesis and how to validate?
Focus on 4 hypotheses 

1️⃣ Regional Happiness Score Differences
I assume that Europe's happiness score is higher than Asia's in terms of world economy, lifestyle and population density.

t-test will be used

2️⃣ Per Capita Income and Happiness Relationship
I think that in today's conditions, the economy is directly related to happiness and I wanted to show this connection.

Pearson Correlation Test will be used

3️⃣ Social Support and Happiness Relationship

Correlation Analysis will be used

4️⃣ Comparison of Happiness Scores Between 2020 and 2024
I wanted to observe if there was a difference between the years. Technology is developing day by day. Since the economy and other things were affected by the pandemic in 2020, I wanted to examine if there would be a difference in 4 years.

Independent Two-Sample t-Test will be used

## Project Plan

1-Data Cleaning 

Data Import & Inspection: Loaded 2020.csv,2021.csv, 2022.csv, 2023.csv, 2024.csv  files . checked structure.

Handling Missing Values: Applied imputation, removal, or "unknown" categorisation.

Standardisation & Formatting: Reformatted dates, verified categorical consistency.

Filtering & Structuring: Removed redundant records and prepared data for analysis.

Output: cleaned and combined file saved  as Combined_Cleaned.csv

2-Exploratory Data Analysis

3-Statistical Analysis

4-Hypotheses examination

Four hypotheses tested and used matplotlib and seaborn used and visualised.

## The rationale to map the business requirements to the Data Visualisations
* Identify Key Factors Affecting Happiness

Business Requirement: Determine which economic and social factors have the most significant impact on happiness levels.

Rationale: We want to understand how different factors (e.g., GDP, social support, health, freedom, generosity, and corruption) influence happiness scores. To do this:

Histogram: To visualize the distribution of numerical columns like "Happiness score", "Economy (GDP per Capita)", etc.

Box Plot: To check for outliers in numerical data.

Correlation Heatmap: To identify relationships between numerical columns.

pair plot : see relationships between multiple features at once

* Analyze Happiness Trends Over Time

Business Requirement: Examine how happiness scores have changed between 2020 and 2024, and assess the impact of global events like COVID-19 on happiness levels.

Rationale: This business requirement is focused on the temporal changes in happiness.

Line Graph: Use a line chart to plot happiness scores over time (for each year) to identify any upward or downward trends.

*  Visualize Country Comparisons
Business Requirement: Identify the happiest and least happy countries, and evaluate geographic and economic influences. Segment countries by continent or income level to detect patterns.

Rationale: To understand global disparities and analyze patterns across countries.

Line Graph: Use a line chart to plot happiness scores over time (for each year) to identify any upward or downward trends.

*  Provide Data-Driven Policy Recommendations

Business Requirement: Suggest policies that could improve happiness levels based on data insights, and measure the impact of economic growth on happiness.

Rationale: This is about deriving actionable insights from data to improve policy and increase happiness.

Regression Line: Overlay a linear regression line on the scatter plot to highlight the relationship between GDP and happiness.

## Analysis techniques used
Data Analysis Methods Used and Limitations

Methods: Descriptive statistics (mean, median, standard deviation), exploratory data analysis (EDA), statistical tests (T-test), visualizations (bar chart, line chart, scatter plot, regression analysis).

Limitations: Happiness score could be understood much more clearly if more detailed data was available.

Step 1: Data cleaning and preprocessing (missing data, date formats).

Step 2: Exploration of data distribution and relationships through EDA.

Step 3: Hypothesis testing through statistical tests (T-test).

Step 4: Presentation of findings through data visualizations (bar chart, line chart, regression line).

Data Limitations and Alternative Approaches

Missing Data: Missing data posed challenges, but analyses were carried out by either removing or imputing missing values.
Data Granularity: Since the data was country-level, deeper analyses were not possible; however, regional analysis was conducted to address this limitation.
Use of Generative AI Tools

Ideation: Ideas for analysis and visualizations were developed.
Design Thinking: The data analysis process was structured accordingly.
Code Optimization: Code optimization was performed for data cleaning, analysis, and visualization processes.
Primary Challenge: The "Year" column had mixed formats (date and integer). This issue was addressed by converting the "Year" column to integers.


## Ethical considerations

Data Privacy, Bias, or Fairness Issues:

Data Privacy: The dataset primarily contains public information, such as happiness scores and various indicators (GDP, social support, etc.) for countries, which do not include personal or sensitive data. Therefore, there were no direct data privacy issues.

Bias: The data reflects happiness and economic/social indicators across countries, which could potentially be influenced by biases in how data is collected or the measurements of happiness themselves. For example, the way happiness is measured might not be consistent across cultures, leading to potential cultural bias in the results.

Fairness: Since the analysis involves global happiness scores, ensuring fairness is crucial. Some countries might have limited or skewed data, affecting the overall conclusions about their happiness levels. This was addressed by considering the reliability and completeness of data from different regions.
How Legal or Societal Issues Were Overcome:

Legal Issues: Since the data is publicly available and does not involve any personal identifiers, there were no legal issues related to data privacy or security. However, ensuring that the data is used responsibly and with transparency in analysis was important.

Societal Issues: To address societal concerns, the analysis took into account that the measurement of happiness can be subjective and influenced by many cultural and societal factors. Efforts were made to acknowledge these differences and avoid drawing overgeneralized conclusions about happiness in various countries. Additionally, the limitations of the data and the potential for misinterpretation were clearly communicated to avoid societal misunderstandings.

## Dashboard Design
* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.
* Later, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but subsequently you used another plot type).
* How were data insights communicated to technical and non-technical audiences?
* Explain how the dashboard was designed to communicate complex data insights to different audiences. 


## Development Roadmap
*While preparing the data, I had edited the column names and types. In particular, I had changed the Year column to Date. However, when doing the next EDA section, I had to convert it back to integer.

*I wanted to work on regions, but I only had country names. My first hypothesis was to compare only Asia and Europe, so I ignored the other countries. As the project progressed, I realized that I had not included the other regions when I wanted to see different regions. I went back and adjusted it to include all regions.

## Future Plan

In the future, by adding additional data, detailed results such as the following can be obtained.

✅ Public Policy & Governance:

Governments can use happiness data to evaluate the impact of policies on well-being.
Example: Tracking how GDP growth or social programs influence happiness scores.

✅ Business & Workplace Well-being:

Companies can analyze happiness trends to improve employee satisfaction and productivity.
Example: Identifying how work-life balance initiatives affect happiness in different countries.

✅ Healthcare & Mental Well-being:

Researchers can assess the impact of healthcare access and mental health support on national happiness.
Example: Analyzing Healthy Life Expectancy vs. Happiness Scores across nations.

✅ Economic Development & Sustainability:

Happiness data can help track the effectiveness of economic policies beyond GDP metrics.
Example: Countries with strong social support systems often rank higher in happiness.

## Main Data Analysis Libraries

* Pandas:

Purpose: Data manipulation and analysis, especially for handling tabular data (CSV files, dataframes) and performing operations like filtering, grouping, and aggregation.

* NumPy:

Purpose:  Used for numerical operations, particularly for working with arrays and mathematical operations statistical analysis on large datasets.

* Matplotlib:

Purpose: Used for creating static visualizations like bar charts, line plots, histograms, etc.

* Seaborn:

Purpose: Built on top of Matplotlib, used for statistical data visualization, such as box plots, heatmaps, and pair plots.

* SciPy:

Purpose: Used for statistical analysis and hypothesis testing, including t-tests, correlation tests, etc.

* Streamlit:

Purpose: Used for creating interactive web-based dashboards that allow users to interact with data visualizations and control the analysis.
## Credits 

### Content 
* Data source

 The World Happiness Report dataset was sourced from Kaggle.
https://www.kaggle.com/datasets/samithsachidanandan/world-happiness-report-2020-2024/code 

This dataset provides insights into global happiness levels, along with various contributing factors such as GDP, social support, life expectancy, and corruption.

* Code & Tutorials:

The code for statistical analysis and data visualization was adapted from various online resources, including:

GeeksforGeeks - Pandas Documentation

Stack Overflow - For resolving specific coding issues and troubleshooting errors related to Pandas, Matplotlib, and other libraries.

Kaggle Notebooks - For insights on performing data analysis using Python and tutorials on common data science tasks.

ChatGBT

### Media

* Images & Visualizations:

Some of the charts and maps used in this project were inspired by the following tutorials:

Matplotlib Documentation - For creating various types of visualizations such as histograms, bar charts, and scatter plots.

Seaborn Gallery - For designing visually appealing statistical plots such as boxplots and pair plots.

Plotly Express Documentation - For generating interactive charts.

The photos and images  used on the home and sign-up page are from This Open-Source site- google images 

## Acknowledgements

I sincerely thank my mentors, peers, and dataset providers for their guidance and support. Special thanks to my family and friends for their encouragement throughout this project.

I would also like to thank the computer that is very slow, my daughter who is constantly asking for something, and my husband who distracts me by asking where things are at the beginning of every hour. 

[def]: C:\Users\balla\OneDrive\Documents\CapStoneProject_2025\images\image1.jpeg
