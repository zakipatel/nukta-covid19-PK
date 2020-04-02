## Covide Case Counts - Punjab 

NOTE: This is a WORK IN PROCESS and repo will be updated frequently. Pls do your own due dilligence before using. 

### Quick Links 
- Tableau Public dashboard # 1 https://public.tableau.com/profile/zaki5466#!/vizhome/Covid19-PK-Punjab/Story1?publish=yes
- Tableau Public dashboard # 2 https://public.tableau.com/profile/zaki5466#!/vizhome/Covid19-PK-Punjab-INTERACTIVE/Story2
- Data file https://docs.google.com/spreadsheets/d/1fPyN7FPTqOTYYABwywNC_zvo3s5ruL0hmOHXRtbvcJo/ 
- Map Viz https://kepler.gl/demo/map/dropbox?path=/apps/kepler.gl%20(managed%20by%20uber%20technologies,%20inc.)/covid-19%20in%20punjab%20-%20confirmed%20cases.json

For more info, please read below. 

### About the data
Description: Aggregated data on confirmed case counts by day and district, for the province of Punjab  

Data Source: Twitter, @CMBuzdar

Data Collection: 
- Manual scrape of tweets
- Daily entry of cumulative cases by district and official quarantine centre
- Calculation of new cases by day and district, based on cumulative cases

Data Quality Issues: 
- A few inconsistencies likely as a result of collapsing/combining geographies. For eg: 
  -  Muzaffargarh has cases and then none 
  -  ..
- Data for Mar 16/17 is not 100% clear

Limitations 
- No data on age, gender, hospital, symptomatic/no, travel/no, etc. 
- Cases at each quarantine centre is not available for April 1, Mar 29. 

### Links: 

#### Google Sheet 

Here is the file (https://docs.google.com/spreadsheets/d/1fPyN7FPTqOTYYABwywNC_zvo3s5ruL0hmOHXRtbvcJo/) 

It has the following sheets:
  - Raw Data: 
      - Scraped from twitter - table 1 has cumulative cases by date and district, table 2 has new case counts by day
      - This is updated at the end of the day based on new info on case counts 
      - This data is in "wide format" and not great for use
      - This sheet has some basic charts to see trends
  - Dataset 
      - Based on the raw dataset, this is the dataset that i use for analysis
      - This data is structued in "long format" - each row is a date and a district.
      - Dictionary of Columns: 
          - Name of District 
          - Latitude
          - Longitude 
          - Number of new confirmed cases for the date 
          - Type = District or Quarantine Facility (not included in first version of data) 
  - Charts
  
  
#### Tableau Dashboard 

Here is the public dashboard - https://public.tableau.com/profile/zaki5466#!/vizhome/Covid19-PK-Punjab/Story1?publish=yes

Some basic exploratory data analysis to start understandng the case count data, and make it accessible to everyone 

The dashboard includes the following tabs: 
- Map:  showing locatins of cases and sum of cases at location 
- Cross Tab 
- Tree Map 1
- Tree Map 3

#### Map Visualiztion 

https://kepler.gl/demo/map/dropbox?path=/apps/kepler.gl%20(managed%20by%20uber%20technologies,%20inc.)/covid-19%20in%20punjab%20-%20confirmed%20cases.json
