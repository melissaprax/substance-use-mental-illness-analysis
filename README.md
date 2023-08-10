# Machine Learning Project Proposal: Marijuana and Mental Health

For our final project, we are interested in exploring the marijuana users' health outcomes. The question or "problem" we are trying to answer through our model is if marijuana usage predicts a set of negative mental health indicators/outcomes or not.

We will do this by using data from the Substance Abuse and Mental Health Services Administration survey published in March 2023 (data from 2019 survey):
https://www.datafiles.samhsa.gov/sites/default/files/field-uploads-protected/studies/NSDUH-2021/NSDUH-2021-datasets/NSDUH-2021-DS0001/NSDUH-2021-DS0001-info/NSDUH-2021-DS0001-info-codebook.pdf

How many rows of data?
2,988 variables (columns)
58,034 rows

Size of data?
File 442 MB


What each person do?
Data analysis and examination of columns


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
