## Hello, I'm Keynes. Welcome to my GitHub! 

*Data Analytics Fellow @COOP Careers. Building a career in entertainment analytics. DJ under the name DJ Key.*

## Table of Contents

* [About Me](#about-me)
* [Skills](#skills)
* [Projects](#projects)
  * [NBA Salary Determinants](#nba-salary-determinants)
  * [Email Spam Classification System](#email-spam-classification-system)
  * [Cook County Housing Price Prediction](#cook-county-housing-price-prediction)
  * [Minimum Wage Policy & Foreign Investment](#minimum-wage-policy--foreign-investment)
  * [Climate Change & Civil Conflict](#climate-change--civil-conflict)
  * [Economic Impact Analysis: Mariel Boatlift](#economic-impact-analysis-mariel-boatlift)
  * [Regional GDP Analysis](#regional-gdp-analysis)
  * [Econometric Analysis of MLB Salary Disparities](#econometric-analysis-of-mlb-salary-disparities)
  * [Classifying Movies (K-Nearest Neighbors)](#classifying-movies-k-nearest-neighbors)
  * [Climate Change: Temperature & Precipitation Analysis](#climate-change-temperature--precipitation-analysis)
  * [Predicting Baseball Wins](#predicting-baseball-wins)
  * [World Population & Poverty Analysis](#world-population--poverty-analysis)
* [Education](#education)
* [Contact & Links](#contact--links)

## About Me
I'm Keynes (pronounced Key-eans), a UC Berkeley graduate in Economics with minors in Data Science and Journalism, currently a Data Analytics Fellow at COOP Careers. My work spans machine learning, econometric analysis, and data-driven projects, with an emphasis on turning analysis into actionable insight rather than just prediction.

Alongside my fellowship, I've gained experience in live and culture-driven environments, including supporting production for the Super Bowl LX Halftime Show, DJing, and active participation in GRAMMY U's LA Chapter. These experiences have shaped how I approach analytics, viewing it not just as numbers but as part of larger systems where timing, coordination, and audience behavior matter. I'm particularly interested in applying data analysis within the entertainment industry, exploring how audience insights and behavior can inform strategy and creative direction.
 
This repository highlights my work across Python and R projects in econometrics, machine learning, and audience research, with a growing focus on entertainment analytics.
 
For a broader view of my work across culture, live production, and creative projects, visit my [personal website](https://keynesle.com).

## Skills 
* **Languages**: SQL, Tableau, Python (pandas, scikit-learn, NumPy, matplotlib, geopandas, statsmodels), R (tidyverse)
* **Tools**: Excel (Pivot Tables, VLOOKUP)
* **Methods**: Econometric modeling, regression analysis, hypothesis testing, machine learning, feature engineering, fairness analysis

## Projects
 
### NBA Salary Determinants
 
September 2025 - December 2025

[Read the full paper (PDF)](Labor%20Economics%20NBA%20Salary%20Determinants%20Project.pdf)
 
**Description:** Applied econometric regression techniques to analyze salary determinants for 269 NBA players from the 1994-95 season. Used log-transformed salary data to address skewness and incorporated performance metrics, experience, position, and race as explanatory variables. Evaluated how on-court productivity translated into wages using both simple and multivariate OLS models.
 
**Skills:** Econometric modeling, OLS regression, data transformation, statistical analysis, hypothesis testing
 
**Technology:** R, tidyverse, regression modeling, data visualization
 
**Results:** Scoring and experience were the strongest predictors of salary, while race and position lost statistical significance once performance was controlled for. Observable productivity explains much of wage variation, though unobserved factors may still influence compensation.
 
**Impact:** Shows how econometric controls separate real drivers of talent compensation from surface-level correlations, an approach directly applicable to evaluating pay structures in sports and entertainment.
 
### Email Spam Classification System
 
November 2025 - December 2025
 
**Description:** Built a supervised machine learning pipeline for email classification using a dataset of over 5,000 messages. The workflow included text preprocessing, feature engineering, model training, and evaluation. Key features were derived using regex-based pattern extraction, word frequency metrics, and text statistics including email length, punctuation counts, and capitalization patterns.
 
**Skills:** Feature engineering, text preprocessing, classification modeling, cross-validation, model evaluation (precision-recall, ROC analysis)
 
**Technology:** Python, pandas, scikit-learn, NumPy, regex
 
**Results:** The model achieved over 90% accuracy with an AUC of 0.943, optimized through multiple iterations of hyperparameter tuning. Precision-recall analysis was used to balance spam detection against the risk of blocking legitimate mail.
 
![ROC curve for the logistic regression spam classifier, AUC 0.943](assets/Email_Spam_ROC_Curve.png)
 
*The curve maps the tradeoff between catching spam and wrongly flagging real mail. The steep climb near the left edge means roughly 80% of spam can be caught while while wrongly flagging under 10% of legitimate messages*
 
**Impact:** Illustrates why headline accuracy is an insufficient success metric when the two error types carry unequal real-world cost.
 
### Cook County Housing Price Prediction
 
October 2025
 
**Description:** Built a machine learning model to predict housing prices using 500k+ property records, applying feature engineering techniques including text mining, log transformations, and one-hot encoding. Developed a full pipeline covering preprocessing, training, and evaluation in scikit-learn, then incorporated fairness analysis to assess model bias across socioeconomic groups.
 
**Skills:** Machine learning, feature engineering, model evaluation, data cleaning, fairness analysis
 
**Technology:** Python, pandas, scikit-learn, NumPy, matplotlib
 
**Results:** Achieved strong predictive performance through K-fold cross-validation and metric comparison (RMSE vs. MAPE). Identified a 15-20% overestimation bias in lower-priced neighborhoods that aggregate accuracy alone concealed.
 
![RMSE and percentage of homes overestimated, both plotted across log sale price intervals](assets/Cook_County_Fairness_Graph.png)
 
*RMSE is lowest at the bottom of the price range, which makes the model look accurate there. The right panel shows the opposite: nearly 100% of the cheapest homes are overvalued, while under 10% of the most expensive ones are.*
 
**Impact:** Demonstrates that a model can perform well overall while failing systematically for a specific group, and that comparing metrics is what surfaces the difference.
 
### Minimum Wage Policy & Foreign Investment
 
January 2025 - May 2025
 
[Read the full paper (PDF)](assets/Minimum%20Wage%20Policy%20%26%20Foreign%20Investment.pdf)
 
**Description:** Conducted panel econometric analysis examining how minimum wage policies and labor availability influence FDI inflows in Southeast Asia. Integrated datasets from ILOSTAT and the World Bank, controlling for macroeconomic variables, and applied fixed effects models to isolate labor policy impacts.
 
**Skills:** Econometrics, panel data analysis, data cleaning, policy analysis, regression modeling
 
**Technology:** R, tidyverse, regression modeling
 
**Results:** Labor availability proved a stronger driver of FDI than low wages. Rising minimum wages did not significantly deter investment when supported by strong labor participation.
 
**Impact:** Challenges the assumption that low wages are the primary competitive lever for emerging economies attracting foreign investment.
 
### Climate Change & Civil Conflict
 
April 2025 - May 2025
 
[Read the full paper (PDF)](assets/Econ%20148%20Climate%20Change%20%26%20Civil%20Conflict.pdf)
 
**Description:** Constructed a panel dataset integrating climate, agricultural, and conflict data to analyze how environmental shocks influence civil conflict risk. Applied fixed effects regression to isolate temperature and precipitation effects while controlling for country and time factors, replicating a foundational climate-conflict economics study.
 
**Skills:** Panel data analysis, fixed effects modeling, data merging, econometrics, statistical interpretation
 
**Technology:** Python, R, pandas, statsmodels
 
**Results:** Found significant relationships between climate anomalies and increased conflict risk in specific contexts, aligning with established academic findings.
 
**Impact:** Building the dataset independently makes the replication a real test of whether the published result holds, not a restatement of it.
 
### Economic Impact Analysis: Mariel Boatlift
 
February 2025 - March 2025
 
**Description:** Replicated a Nobel Prize-winning natural experiment analyzing the labor market impact of immigration using 26,000+ survey records. Conducted comparative trend analysis across metropolitan areas and applied OLS regression with engineered variables, focused on identifying causal effects from labor supply shocks.
 
**Skills:** Causal inference, OLS regression, data analysis, feature engineering, data visualization
 
**Technology:** Python, pandas, NumPy, matplotlib
 
**Results:** Found no statistically significant negative impact on wages despite a 7% labor force increase, supporting the conclusions of the original study.
 
![Log wages in Miami versus comparison cities from 1979 to 1985, split by demographic group](assets/Mariel_Boatlift_Trends.png)

*Miami and the comparison cities rise together both before and after the 1980 boatlift, marked by the dashed line. That continued parallel movement is what makes the absence of a wage effect credible rather than coincidental.*
 
**Impact:** A worked example of using a natural experiment to establish causation where correlation would mislead.
 
### Regional GDP Analysis
 
February 2025
 
**Description:** Analyzed U.S. county-level GDP data from 2001 to 2021 to evaluate regional economic trends and recovery patterns. Processed and reshaped large datasets, expanding 47k+ records into 718k rows for analysis, and developed geospatial visualizations to identify growth disparities across regions.
 
**Skills:** Data cleaning, time-series analysis, data transformation, geospatial analysis, data visualization
 
**Technology:** Python, pandas, matplotlib, geopandas
 
**Results:** Identified stronger post-2008 recovery in coastal regions than in the Midwest, with growth concentrated in urban and tech-driven areas.
 
![County-level percentage change in real GDP across the United States in 2002, 2008, and 2020](assets/regional-gdp-maps-2002-2008-2020.png)
 
*Three snapshots on a shared color scale. Mapping every county turns a national average into a geography and shows how unevenly each period was distributed across the country.*
 
**Impact:** Shows how restructuring a dataset into the right shape is often the step that makes a pattern visible at all.
 
### Econometric Analysis of MLB Salary Disparities
 
November 2024 - December 2024
 
[Read the full paper (PDF)](assets/Econometrics%20Analysis%20of%20MLB%20Salary%20Disparities.pdf)
 
**Description:** Analyzed MLB salary determinants using regression models to evaluate the impact of race, city demographics, and performance metrics. Applied econometric techniques to control for confounding variables and explored potential bias and omitted variable effects.
 
**Skills:** Econometrics, regression analysis, bias analysis, statistical modeling, data interpretation
 
**Technology:** R, regression modeling
 
**Results:** Performance metrics were the strongest predictors of salary, with limited influence from demographic variables. Identified potential omitted variable bias in the specification.
 
**Impact:** Naming what the model cannot observe matters as much as reporting what it found.
 
### Classifying Movies (K-Nearest Neighbors)
 
April 2024
 
**Description:** Built a k-nearest neighbors classifier to predict movie genres from keyword frequency in scripts. Engineered custom features and applied Euclidean distance for classification, evaluating performance across different feature sets.
 
**Skills:** Machine learning, feature engineering, classification, data analysis, model evaluation
 
**Technology:** Python, scikit-learn, pandas
 
**Results:** Improved classification accuracy through feature selection and distance tuning, identifying the word associations driving genre prediction.
 
![Movies plotted by the frequency of the words water and feel, colored by genre](assets/Classifying_Movies_Graph.png)
 
*Each film becomes a point in keyword space. Adding The Silence of the Lambs to the training set moves the nearest neighbor of the unlabeled film, flipping its predicted genre from comedy to thriller.*
 
**Impact:** An early look at classifying entertainment content by its text, the same problem shape as tagging or categorizing music by lyrical and metadata features.
 
### Climate Change: Temperature & Precipitation Analysis
 
March 2024 - April 2024
 
**Description:** Analyzed temperature and precipitation trends across 210 U.S. cities, applying hypothesis testing and confidence intervals to evaluate change over time, with A/B testing on drought conditions.
 
**Skills:** Statistical analysis, hypothesis testing, data visualization, inference
 
**Technology:** Python, pandas, matplotlib
 
**Results:** Identified statistically significant warming trends across cities and measurable differences in precipitation during drought periods.
 
![Average maximum and minimum temperatures across U.S. cities from 1896 to 2020](assets/Temperature_Trends_1900-2020.png)
 
*Both daily highs and daily lows trend upward across 120 years, but nighttime lows climb far more sharply after 1960, rising roughly 10 degrees while daytime highs rise about 5.*
 
**Impact:** An applied exercise in separating a real trend from year-to-year noise using confidence intervals, rather than reading a direction off a chart.
 
### Predicting Baseball Wins
 
March 2024 - April 2024
 
**Description:** Developed least squares regression models to predict MLB team wins from performance metrics, building from a single-variable model through multivariate specifications and log transformations across every team season since 2000.
 
**Skills:** Regression analysis, statistical modeling, model evaluation, sports analytics
 
**Technology:** R, tidyverse, ggplot2
 
**Results:** Runs alone explained 61% of variation in wins. Adding runs allowed raised this to 79%, and log transformations across runs, runs allowed, doubles, and saves reached 94%.
 
![Team runs scored plotted against season wins, with fitted regression line](assets/Runs_vs_Wins_Graph.png)
 
*The small cluster in the lower left is the shortened 2020 COVID season, a reminder that structural breaks in the data can distort a fitted line if left unexamined.*
 
**Impact:** A model improves by adding the variables that carry independent information, not by adding variables indiscriminately, and knowing which is which is the analyst's job.
 
### World Population & Poverty Analysis
 
February 2024
 
**Description:** Analyzed global population and poverty trends across 145 countries using statistical visualization techniques, exploring relationships between life expectancy, fertility, and economic conditions.
 
**Skills:** Data visualization, statistical analysis, exploratory data analysis
 
**Technology:** Python, pandas, matplotlib
 
**Results:** Identified strong relationships between development indicators and population dynamics, with clear patterns in global poverty reduction.
 
![Distribution of children per woman across countries in 1962 compared with 2010](assets/Fertility_1962_vs_2010.png)
 
*In 1962 the distribution peaked near six or seven children per woman. By 2010 it had collapsed toward two, one of the largest demographic shifts ever recorded.*
 
**Impact:** Early practice in using visualization to find which relationships across 145 countries were worth modeling formally, before committing to a specification.
 
## Education
**COOP Careers** — Data Analytics Fellowship<br>
July 2026 - Expected December 2026

**University of California, Berkeley** — College of Letters and Science<br>
Bachelor of Arts, Economics | Minors in Data Science and Journalism<br>
January 2024 - December 2025

**Pasadena City College** — Associate of Arts, Business, Economics UC Transfer Pathway<br>
August 2021 - May 2023
 
## Contact & Links
 
* **Email:** [lekeynes1@gmail.com](mailto:lekeynes1@gmail.com)
* **LinkedIn:** [linkedin.com/in/keynesle](https://www.linkedin.com/in/keynesle/)
* **Website:** [keynesle.com](https://keynesle.com/)
