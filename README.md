# AYC
code for analyzing data to assess the Alamance Youth Connected (AYC) initiative:
+ member knowledge, skills, and attitudes (KSAs) within the Community Advisory Board (CAB)
+ technical assistance (TA) hours, tracked over time
+ organizational readiness, using indices from the Sex Education Collaborative's (SEC) Racial Justice and Equity Task Team (RJETT)
+ Implementation Partner Needs Assessment (IPNA) to support TA
+ self-assessment of facilitators' comfort with trauma-informed approaches (TIA)
+ reach, fidelity, and dosage via pre/post tests (PPTs) and observations of evidence-based programming by implementing organizations (IOs) for quarterly progress reports (QPRs) and semi-annual progress reports (SAPRs) to the Office of Populations Affairs (OPA)/Office of Adolescent Health Performance Measures (OAHPM) database

# Purpose:
to store datasets and R code to analyze assessment data for AYC
(when in doubt go here: https://happygitwithr.com/rstudio-git-github.html)

# Inputs:
  + Markdown files to document what the R code is and does (.rmd), knit into a Word document (.docx)
  + datasets (with numerical values) from SurveyMonkey (.csv)

# Outputs:
  + Diverging bar charts to visualize Likert scale items (i.e., 5-point scales ranging from strongly disagree (1) to strongly agree (5) for progress reports (.png)
  + Donut charts to visualize counts/percents of categorical data for progress reports (.png)

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

# Getting Started--Exporting Data

1. Sign in to Survey Monkey and select your survey
2. Export the responses ("Exports" under "Analyze Results")
  + Export all responses data (individual = what each respondent entered; summary = SurveyMonkey charts and data tables)
  + .csv
  + Original View (without any SurveyMonkey filters)
  + Condensed
  + Numerical Value (easier to clean this format; "actual text" is not analyzable)
3. Upload this *.csv file to the Repository

# Getting Started--R Studio

First time: 
1. Download & install Git (http://git-scm.com/downloads), R (e.g., http://archive.linux.duke.edu/cran/), and RStudio (https://rstudio.com/products/rstudio/download/#download). 
2. Open RStudio. Create a new project (top right) > version control > GIT > https://github.com/ [owner name]/[repository name].git. This will create a local directory (i.e., a folder with the repository name in your Documents folder).
3. Upload datasets and save Markdown files there. The code that you will run is an .rmd file. Markdown is a plain text format that incorporates R code and outputs into a .docx, .pdf, or .html files. Knitting the Markdown file will generate the visualizations, also saved in that local directory folder.
4. Commit your changes: Git tab (top right) > select all those additions (A), add a commit message that summarizes what you're doing in this version, session, or draft > commit those changes > push those committed changes to GitHub (enter your GitHub username and password).

Every time:
1. Open RStudio. Set your project (top right in RStudio).
2. Pull any changes made in GitHub to your local directory FIRST.
3. File > New Files > R Script or R Markdown to clean, analyze, visualize data
 + import or read in your dataset
 + remove informational headers
 + define/recode missingness (e.g., -99 = NA)
 + factor categorical (dichotomous, nominal, ordinal) variables
 + select or subset the data you want to analyze
 + run any analyses
 + plot any visualizations
4. Commit any changes you  make (i.e., saving changes frequently) with a description.
5. Push those committed changes to GitHub before you close out of RStudio.
