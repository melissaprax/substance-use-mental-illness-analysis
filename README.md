# Machine Learning Model Project: Substance Use and Mental Health

For our final project, we are interested in people's health outcomes after substance use. The question or "problem" we are trying to answer through our model is if substance usage predicts a set of negative mental health indicators/outcomes for people or not.

## The Data

Our main data source is from the Substance Abuse and Mental Health Services Administration [survey published](https://www.datafiles.samhsa.gov/sites/default/files/field-uploads-protected/studies/NSDUH-2021/NSDUH-2021-datasets/NSDUH-2021-DS0001/NSDUH-2021-DS0001-info/NSDUH-2021-DS0001-info-codebook.pdf) in March 2023 (data from a 2019 survey).

With 58,034 rows and 2,988 variables to pull from, we thought this would be ample of enough data to model.

## Preliminary Data Analysis

Exploratory data analysis (EDA) was the first step in our project. Our interest was particularly in marijuana-related variables, given the recent discourse around [cannabis use disorder](https://www.washingtonpost.com/health/2023/07/31/marijuana-addiction-legal-recreational-sales/).

So first, we pulled a handful of indicators relating to marijuana and mental health indicators that were focused on respondent's experiences in the past year. We focused binary indicators during our initial EDA, preprocessing the data for an initial model.

## Initial Model



Using random forest (fresh_look.ipynb)

MJEVER, which is the indicator for if respondents have used marijuana previously, was showed as the most important feature.

Our target?

We were able to get a 64???% accuracy in running the model.

What we don't know is if our model predicts better or worse mental health outcomes for users of marijuana.

## Pycaret

## Expanding the Data Variables

After looking through the code book more thoroughly and having a better understanding the of methodology, we created a data frame that fully encompassed

## Advancing the model

Adding a handful of more variables to expand our model to consider more substances and predictors of health.

## Indicators

Indicators we are interested include general marijuana usage questions in the survey, including:

- 'MMBTPYR' — Bought cannabis in past 12 months
- 'MMBT30DY' — Days bought cannabis in Past Month
- 'MMBTDISP' — Bought from store or dispoensary
- 'MMBJOINT' — Last cannabis bought in joints
- 'MMBLOOSE' — Last cannabis bought in Loose form
- 'MMBOTHER' — Last cannabis bought in other form
- 'MMLSUNIT1' — AMT cannabis bought in last time: grams/oz/lbs
- 'MMLSPCTB1' — Amount paid for cannabis last time in bins
- 'MMLSPCAT1' — Price category of last loose marijuana bought
- 'MMBSELL' — Sell any marijuana bought last time

Because of how large the survey is and how many substances covered in the questions, we narrowed down our focus to include adults with a range of mental health indicators, including:

-'IRIMPREMEM' — DIFFICULTY REMEMBERING ONE MO IN PAST 12 MOS
- 'ADDPREV' — SEVERAL DAYS OR LONGER WHEN FELT SAD/EMPTY/ DPRSD
- 'IRSUIPLANYR' — ADULT MADE PLANS TO KILL SELF IN PAST YEAR - IMP REV
- 'ASDSREL2' — ADULT: DEEP FEELINGS ROLE IMPAIRMENT - CLOSE RELATIONSHIPS
- 'IRAMDEYR' — ADULT: PAST YEAR MAJOR DEPRESSIVE EPISODE
- 'IRDSTCHR12' — HOW OFTEN FELT COULDN'T BE CHEERED UP IN WORST MONTH

## ML Technolgies

We will start with logisitic regression, random forests (for purpose of featured engineering) and deep learning/neural networks. Potentially use PyCaret for larger overview.

## Final Product

We are looking to populate a report via a Jupyter notebook and also data visualizations based on data exploratory analysis for annual and other trends from the indicators listed in the section above.
