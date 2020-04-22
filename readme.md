# Introduction
This case study is based upon the Bank Marketing Data Set in the UCal Irvine repository (http://archive.ics.uci.edu/ml/datasets/bank+marketing). Unlike the Irvine data set, which is relatively clean, this set was confounded with a number of issues which required resolution prior to performing any predictive analysis. Among the issues requiring further cleaning/wrangling are:
1. Missing data for `custAge`, `schooling`, and `day_of_week`
2. Response variable, `responded`, is highly imbalanced
3. Several numeric variables required binning to provide useful data
4. Some numeric columns included specific _flag values_ that that functioned as categorical indicators. As an example, the variable `pdays` refers to the number of days since the previous contact; however, a value of '999' was used to indicate that the customer had never been previously contacted.
# Analysis
Details of data cleansing and further analysis are documented [here](https://github.com/rainwaterone/sg-marketing-case-study/blob/master/rainwater-sparkCognitionDSCase.pdf). An initial logistic regression was performed and evaluated via integrated area under the Receiver Operating Characteristic curve. It must be emphasized that this analysis is incomplete at this point, but provides insight into the degree of data wrangling that may be necessary to render a usable dataset.
