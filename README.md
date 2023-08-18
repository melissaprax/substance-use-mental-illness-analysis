# Machine Learning Model Project: Substance Use and Mental Health

For our final project, we are interested in people's health outcomes after substance use. The question or "problem" we are trying to answer through our model is if substance usage predicts a set of negative mental health indicators/outcomes for people or not.

## The Data

Our main data source is from the Substance Abuse and Mental Health Services Administration [survey published](https://www.datafiles.samhsa.gov/sites/default/files/field-uploads-protected/studies/NSDUH-2021/NSDUH-2021-datasets/NSDUH-2021-DS0001/NSDUH-2021-DS0001-info/NSDUH-2021-DS0001-info-codebook.pdf) in March 2023 (data from a 2019 survey).

With 58,034 rows and 2,988 variables to pull from, we thought this would be ample data to model.

## Technologies

- Random forest
- Numpy
- Pycaret
- Python
- Gradient Boosting Classifier
- imblearn packages
- Jupyter notebook
- Pandas
- Matplotlib
- Seaborn

## Preliminary Data Analysis

Exploratory data analysis (EDA) was the first step in our project. Our interest was particularly in marijuana-related variables, given the recent discourse around [cannabis use disorder](https://www.washingtonpost.com/health/2023/07/31/marijuana-addiction-legal-recreational-sales/).

So first, we pulled a handful of indicators relating to marijuana and mental health indicators that were focused on respondent's experiences in the past year. We focused binary indicators during our initial EDA, preprocessing the data for an initial model.

## Initial Model

Using random forest (fresh_look.ipynb)

MJEVER, which is the indicator for if respondents have used marijuana previously, was showed as the most important feature.

What we don't know is if this model predicted better or worse mental health outcomes for users of marijuana.

## Expanding the Data Variables

After looking through the code book more thoroughly and having a better understanding the of methodology, we created a data frame (shown in MainV2_copy.ipynb.) that would answer our initial question better, ultimately landing on 15 variables. These variables considered more substances and predictors of health, including demographic and economic factors.

- CATAG3 = Recoded field - 5 levels of age groups
- HEALTH2 = Recoded field - Overall health
- ANYHLTI2 = Recoded field - Any health insurance
- INCOME = Recoded field - Total family income
- POVERTY3 = Recoded field - Poverty level
- TOBFLAG  =  Used tobacco at least once in lifetime
- MRJFLAG = Used marijuana at least once in lifetime
- PYUD5MRJ = Recoded field - Marijuana disorder
- MJYRTOT  = Use of marijuana - days of past year
- ALCFLAG = Used alcohol at least once in lifetime
- COCFLAG = Used cocaine at least once in lifetime
- CRKFLAG = Used crack at least once in lifetime
- HERFLAG = Used heroine at least once in lifetime
- LSDFLAG = Used LSD at least once in lifetime
- METHAMFLAG =Used metamphetamines at least once in lifetime

- Target (y) : Depression - Combination of ADSMMDEA & YODSMMDE - show at least 5 symptoms of depression

## Pycaret

We used the Pycaret library to see which would be the best model for our use which showed a Gradient Boosting Classifier. (pycaret_addprev_starter.ipynb)

## Modeling workflow

After initial exploratory data analysis, we built a pilot model with only binary substance use variables using scikit-learn’s Random Forest Classifier. Our first model’s target was built from the variable ADDPREV (several days or longer when felt sad/empty/depressed). After thorough review of the Survey Codebook, wee xpanded predictors to include demographic information and selected a more reliable/representative target for Major Depression.

## Advancing the model

![map](/Threshold_Optimization.png)

![map](/mainV2_copy_TUNED_GBC_CM.png)

Feature importance: * insert image *

## What we can infer

Based on using depression as a target, we found in our features that marijuana use did have an effect on mental health

Marijuana use was between the most important features to all models compared to other binary substance use variables (outside of alcohol in youth)

We can use the variable smoker model  to “catch more” people with depression


## Link to our presentation slides

[Google slides](https://docs.google.com/presentation/d/1Pg1Eq0wTxrVo2yH9IqTPCoKMTMywzswbn93F7supOa8/edit#slide=id.g23bf9061268_2_95)
