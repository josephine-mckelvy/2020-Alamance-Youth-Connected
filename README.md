# AYC
code for analyzing data for the Alamance Youth Connected (AYC) initiative

# Purpose:
to store datasets and R code to analyze assessment data for AYC

# Inputs:
  + Markdown files to document what the R code is and does (*.rmd), knit into a Word document (*.docx)
  + datasets (with numerical values) from SurveyMonkey (*.csv)

# Outputs:
  + Diverging bar charts to visualize Likert scale items (i.e., 5-point scales ranging from strongly disagree (1) to strongly agree (5) for progress reports (*.png)
  + Donut charts to visualize counts/percents of categorical data for progress reports (*.png)

# Getting Started--Data Collection

1. Create/Edit the survey on SurveyMonkey
2. TEST this survey for typos, exhaustive/mutually exclusive response categories, and page/skip logic
  + Go to "Preview & Score"
  + "View comments" on the top right sends you to "Preview & Test"
  + Copy and paste the "Invite" link on the top right
3. Export this survey as a PDF (not recommended, especially for dropdown menu Qs) or administer/distribute it via SurveyMonkey response collectors.
  + Turn on multiple responses
4. For your codebook, print the survey (bottom right under "Design Survey") and add recode values for each response category. 
(Take the survey and export as numerical values for recode values. The recode values will be your "key" or "legend" as to what the numbers mean.)
  + Include Survey Title
  + Include Page Numbers
  + Print without Page Breaks

# Getting Started--Survey Monkey

1. Sign in to Survey Monkey and select your survey
2. Export the responses ("Exports" under "Analyze Results")
  + Export all responses data (individual = what each respondent entered; summary = SurveyMonkey charts and data tables)
  + .csv
  + Original View (without any SurveyMonkey filters)
  + Condensed
  + Numerical Value (easier to clean this format; "actual text" is not analyzable)
3. Upload this *.csv file to the Repository

# Getting Started--R Studio

Download the PPGWLI-master zipped folder
Open the 2018-2019 PPGWLI.Rproj (a directory where you'll find the inputs, code, and outputs)
Open the 2018-2019.R (the R code with documentation to explain what the code does)
