java c
BUSANA 7003 – Business Analytics Project – Semester 2, 2024
Final Project
Background.You are starting a new job as a Business Analyst at AQR Asset Management, a global investment management  firm focused on quantitative  investment  strategies. Your  first task is to  analyse the performance of US-listed securities to help the firm manage their portfolio. You have several datasets on US securities (stocks and ETFs), and you should help your employer with the following tasks:
(1) Exploratory data analysis, visualisations, descriptive statisticsExamine the dataset Stock_data_part1.xlsx. Characterise the performance of US securities between February 14, 2020,and March 20, 2020, and compare their performance to a similar period not affected by the COVID-19 pandemic. Justify how you choose the non-COVID period to make a fair comparison.
Based on your analysis, comment on the effect of the COVID-19 pandemic on securities’ performance. In your analysis, you should consider the following:
•    Which variables to analyse? Consider the following: returns, volatility, Sharpe ratio, bid-ask spread, dollar volume, number of trades. You should do your own research and also use the course content to understand these variables, and potentially add others, which could be helpful for understanding the market dynamics during the COVID-19 pandemic and beyond it.
•    What is the data structure (unit of observation) that you need for this analysis? (Cross-sectional? Time series? Panel?) How to transform. your data into the units of observation that you need?
•    How can you add value with your analysis? Can you offer relevant comparisons of returns or other variables across different groups (e.g., COVID vs non-COVID period, by industry, by company size, ETFs vs stocks etc.)?
Use your own judgement to select the relevant descriptive statistics and visualisations. However, at a minimum, you should consider the following:
•    A  table with descriptive  statistics (mean, median, 25th  percentile, 75th  percentile, standard deviation, min, max) of the key variables you choose to analyse. (Add comparisons by group if relevant).
•    The time series of the key variables of interest (Add comparisons by group if relevant). Make sure you cover the entire time period of the sample. You can add analysis by sub-period (e.g., COVID vs non-COVID periods) as an additional point.
(2) Supervised Machine Learning – OLS regressionsTransform. your data into across-section: for each security, compute returns between February 14, 2020, and March 20, 2020, and run regression analysis to help explain returns. Then, do the same for returns between December 14, 2019, and January 20, 2020. You may use any variables in the existing dataset, or variables outside the provided datasets (from external sources). For example, you may consider the following external sources:
-     Robinhood  stock  popularity  history: https://www.kaggle.com/datasets/cprimozi/robinhood- stock-popularity-history?resource=download (historical data about the number of users that hold each stock available on the Robinhood stockbrokerage),
-     Stock exposure to the market, and to Fama-French factors. The time series data on Fama-French factors is available here:
-    https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.htmlNOTE: you need to first run OLS regressions of stock returns on 3 Factors (Mkt, HML, SMB), and compute betas (factor exposures) for each stock. Then, you can use those betas as explanatory variables in your SML analysis.
Please, make sure to split the dataset you use for analysis into training and testing samples, and comment on the model accuracy. Please, analyse the following:
-     Are you better able to predict returns between February 14, 2020,and March 20, 2020 or returns between December 14, 2019, and January 20, 2020?Why?
-     Are you better able to predict returns between February 14, 2020,and March 20, 2020 for stocks or for ETFs? Why?
In your analysis, you should consider the following:
•    Which explanatory variables to use?
•    Over which period of time to compute the explanatory variables? Imagine it is February  14, 2020, and you know nothing about the future returns, market caps, volumes, investor interest etc. You are tasked to develop a SML model to help predict returns between February 14, 2020, and March 20, 2020. How can you use the data from the past to predict the future?
•    Consider running separate models for stocks vsETFs. Think about which explanatory variables are more relevant for each group.
•    What is the data structure (unit of observation) that you need for this analysis? (Cross-sectional? Time series? Panel?) How to transform. your data into the units of observation that you need?
•    How  well  does your model perform? Can you offer relevant comparisons  of your model accuracy across different groups (e.g., COVID vs non-COVID period, by industry, by company size, ETFs vs stocks etc.)?
In your analysis, at a minimum, you should present the following output:
•    Regression coefficients from multiple models (at least five).
•    Model evaluation metrics: MSE, RMSE, MAE for each model.
•    Your  assessment of which factors are most important for explaining stock returns between February 14, 2020, and March 20, 2020, and between December 14, 2019, and January 20, 2020.
•    Your  assessment of which factors are most important for explaining ETF returns between February 14, 2020, and March 20, 2020, and between December 14, 2019, and January 20, 2020.
(3) Supervised Machine Learning – Logistic regressionsUse the same dataset as in part (2), and introduce a dummy variable for whether a given security increased in price between February  14, 2020, and March 20, 2020. Model the probability of a price increase using any continuous or categorical variables you find relevant. You may use any variables in the existing dataset, or variables outside the provided datasets (from external sources).
Please, make sure to split the dataset you use for analysis into training and testing samples, and comment on the model accuracy.
In your analysis, you should consider the following:
•    How  does the industry variable affect whether a given security increased in price between February 14, 2020, and March 20, 2020?
•    H代 写BUSANA 7003 – Business Analytics Project – Semester 2, 2024C/C++
代做程序编程语言ow does being a stock or an ETF affect whether a given security increased in price between February 14, 2020, and March 20, 2020?
•    Imagine we are facing areplay of the COVID-19 pandemic now, and you are asked to predict whether your testing sample securities will increase or decrease in price, based on what you learnt from your analysis over February 14, 2020, and March 20, 2020. Comment on which factors are affecting this.
In your analysis, at a minimum, you should present the following output:
•    Regression coefficients from multiple models (at least five).
•    Model evaluation metrics: accuracy, precision, recall for each model.
•    Your assessment of which factors are most important for explaining whether a given security increased in price between February 14, 2020, and March 20, 2020?
(4)  Unsupervised Machine Learning – K-means clusteringExamine the dataset Stock_data_part2.xlsx to perform. the k-means clustering. You may combine Stock_data_part2.xlsx dataset with any other data (e.g., returns) from the previous exercise. The key part of this analysis is finding clusters if stocks with similar characteristics (financial ratios), and showing  whether their returns during between February 14, 2020, and  March  20,  2020  were significantly different. How about their returns during December 14, 2019 - January 20, 2020?
In your analysis, you should consider the following:
•    Variable Selection: Which two financial ratios did you select as the most important variables for clustering, and why?
•    Cluster Characteristics: What are the average values of the selected financial ratios for each cluster? Present a table showing the average values of the selected financial ratios for each identified cluster.
-     Cluster  Visualization:  How  can  we  visualize  the  distribution  of  the  clusters  in  a  two- dimensional space using the selected financial ratios?
-     Provide a scatter plot where each point represents a stock, coloured by cluster, using the two selected financial ratios on the axes.
In your analysis, at a minimum, you should present the following output:
•    Elbow plot and cluster visualisation in two-dimensional space.
•    How returns differ across cluster, with comparison of two periods: February 14, 2020 -  March 20, 2020, vs December 14, 2019 - January 20, 2020.
•    Your assessment of investment implications. Which stocks should AQR invest in, if market conditions are similar to those on February 14, 2020, vs those on December 14, 2019?
(5)  Unsupervised Machine Learning – Principal Component AnalysisThe lead asset manager asks you to  distil  a variety of market-wide  factors to the  core Principal Components. The Principal components will be used to explain average monthly returns on SP500 index. You may combine Stock_data_part3.xlsx dataset with any other data (e.g., valuation ratios, market returns, Fama-French factors (external), interest rates (external) etc.), and analyse the principal components to understand the factors driving market returns.
In your analysis, you should present the following output:
•    A detailed summary of the principal components extracted from the PCA, including the amount of variance  explained  by  each  component.  This  should  include  a  scree  plot  or  a  table summarizing the eigenvalues and the percentage of variance explained by each principal component, helping to identify the most significant factors affecting monthly returns.
•    Factor Loadings: For each principal  component identified as significant, provide the factor loadings of the original variables (e.g., valuation ratios, market returns, Fama-French factors, interest  rates).  This  will  show  how  each  original  variable  contributes  to  the  principal components, indicating which factors are most influential in driving returns.
•    Factor Interpretation: An interpretation of what each significant principal component represents in the context of market-wide and company-specific factors. For example, the first principal component might be interpreted as overall market risk, while the next components could represent size and value factors, sector exposures, or interest rate sensitivity. This section should bridge the mathematical output of PCA with intuitive financial concepts.
•    Implications for Monthly Returns: Discuss how each principal component influences monthly returns on  SP500 index. This could involve  analyzing how movements in the principal components  are  associated  with  changes  in  market  returns,  providing  insights  into  the underlying risk factors or market conditions that impact asset prices.
(6) Analysing experimental evidence using Difference-in-Difference regressionsAQR wants to analyse the effects of the SEC Tick Size Pilot program, and find out how the securities in test groups were affected in terms of relative bid-ask spread. Use monthly data from Stock_data_part3.xlsx and the list of treatment and control securities  (https://www.finra.org/rules- guidance/key-topics/tick-size-pilot-program) to investigate this question.
In your analysis, you should present the following output:
•    A  regression specification with detailed explanation of the null hypothesis and alternative hypothesis.
•    Regression output and interpretation of coefficients.
•    Implications for AQR trading strategy. How should AQR adjust their trading in treated and control stocks to minimise their transaction costs?
(7) Summary
Based on your earlier analysis, draw conclusions  for AQR that tackle the  following overarching questions:
-     What are your recommendations to AQR about their stock and ETF selection strategy, if they found themselves in market conditions similar to pre-COVID (e.g., February 14, 2020)?
-     How accurate are your ML models in predicting the price changes, and how confident are you in providing recommendations based on those models?
-     What does your analysis reveal about the market dynamics around the COVID-19 period, and how it differs across different groups of securities?
-     Which variables from the dataset are most important in their contribution to the variation in SP500 returns?
-     What did you learn about the way the effect on liquidity, as a result of the Tick Size Pilot?

         
加QQ：99515681  WX：codinghelp
