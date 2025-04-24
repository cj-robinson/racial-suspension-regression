# Racial Discipline Disparity

This repo holds the code to examine 2021-22 Civil Rights education data for racial disparities in education, specifically the ratio of supension rates of Black students compared to white students. It utilizes linear regression to account for school-level characteristics and explain the range of this racial discipline gap. 

## Data

Only the final, filtered data is uploaded due to size constraints. Original CRDC data can be found here: https://civilrightsdata.ed.gov/data

I also utlize school-lunch data as a proxy for poverty/income in a school found here: https://nces.ed.gov/ccd/files.asp

## Analysis

1-data-extraction.ipynb
- takes all individual CRDC data excel sheets and collates them into a single CSV
  
2-merge-with-census.ipynb
- uses tidycensus to grab zip-code level informaiton and joins on the CSV above
  
3-data-cleaning.ipynb
- creates variables for analysis, filters for specific conditions necessary for regression and outputs final filtered data

4-linear-regression.ipynb
- regression and residual analysis for story
