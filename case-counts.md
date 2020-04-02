# Case Counts

Case counts data is needed for surveillance and monitoring. Numnber of cases is a leading key indicator in measuring the outbreak. 

Typically, this data is shown on dashboards. And, it is incredibly useful for analysis : 

Types of analysis: 
- analyzed geo-spatially
- analyzed as a time series 
- modelled to generate an epi curve 

##  An Example - Punjab Case Counts at District Level 

- Insert link 

## Data Requirement 

Here I spec out the requirements: 

1) Confirmed Case Register 

For each confirmed case, we record a row of data, with dates, age, gender, symptoms/none, travel/history, hospital, status, location

This is the ideal case but probably not available. One way to build this up is using news media sources, but the exercise is manual, time consuming and reporting is incomplete 

2) Cases by Province/District/Tehsil - Disaggregated

This is a time series dataset, where for each district, there is a new row for each date. For each row, we have:
 - the number of new cases confirmed.
 - how many in each  hospitals
 - count by gender and age group 
 
This is not available and probably unrealistic 

3) Cases by Province/District/Tehsil - Aggregated 

This is a time series dataset, where for each district, there is a new row for each date. 
For each district, each date, we have:
 - the number of new cases confirmed
 
This data is available at Province level, but needs to be curated at District level. 


## Pakistan - Data Sources

Here are a list of data sources / publishers of case count data in Pakistan. 

### NIH 
- By Date, by Province
- Published on their website in a PDF format, aggregated at the Provincial level
- Key data points included are:
  - New case counts (i.e. positive test cases), 
  - Tests performed 
  - Travellers screened 
  - Risk interventions 

This dataset appears to be the official one,  except, the published data is aggregated at the province level. There is nothing about age, gender or hospital. 

The dataset is in PDF, which is a pain. Luckily, it looks like someone has done the job to scrape the PDF into a spreadsheet ! 

This data can and should be used for baseline modeling at provincial level. 

### News Media 

- Dawn/Geo/Express and other local news 
- Each provide a blog thread with well structured event info 
- In many cases, disaggregated infomration about gender, age, hospital and travel history is included, tho incomplete.

### Government officials

- Twitter feeds of Provincial CM's provide good source for district level data on a daily basis 

