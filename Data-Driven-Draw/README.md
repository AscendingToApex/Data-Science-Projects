# Colorado Big Game Hunting Data Driven Draw

# Project Understanding
### Plan for Project Understanding Phase
Establish the background and need for project and determine the objectives of the project; progressively through a describe, explore, explain, predict, and prescrive analytics maturity path.

### Tools Used in Phase:
- CRISP-DM Methodology

## Background:
Mike had been applying for points every year for over half his lifetime in order to hunt elk in a specific unit. April rolled around again, as it had every other year he'd been applying, but this year was different. A friend told him he had enough points to draw the legendary tag this year, so he optimistically submitted the application and started planning the hunt; only to get an e-mail a short month later stating that he had once again failed to recieve the tag because he didn't look through over 6,000 pages of past draw recap statistics to verify what his chances of drawing were.

This situation happens every year in some capacity to most Colorado big game hunters because of the time required and difficulty to digest the hunting statistics provided by Colorado Parks and Wildlife.

For big game hunting, Colorado uses a preference point system to increase the chances of getting the opportunity to hunt specific units over time. The hunters with the higher preference points have a higher probability of obtaining tags that require a draw than hunters with the fewer preference points. The preference points are specific to species and hunters are able to accumulate a single point per species after unsuccuessfully drawing a tag. In addition, the majority of "trophy" units have a limited number of tags available per hunt code, which is specific to species, region in colorado, time of year, and hunting method.

One of the issues with the current preference point methodology is "Point Creep". The "Point Creep" phenominon occurs when the number of tags available doesn't meet the demand of applicants and each year the quantity of points required to draw the tag increases. The Colorado Division of Wildlife has combated this phenoinom by executing a hybrid draw of up to 20% of select tags. These tags are a random draw for hunts that require at least 10 preference points to draw, which allow an opportunity for hunters to at least have a shot at drawing some of the more desireable hunt codes. Unfortunately, the hunt code available for a hybrid draw has not been evaluated since a 2009.

This project is geared towards analyzing "Point Creep" in order to present the results to the Colorado Division of Wildlife with hopes of expanding the available list of hybrid draw hunt codes.

## Objective:
### Describe
- How many hunt codes is point creep occuring on?
### Explore
- Which hunt codes is point creep occuring?
- What does the problem space look like for the top three hunt codes with the most point creep?
- What patterns or groupings can be found in my data?
### Explain
- What is related to point creep?
- What can a sample tell me about the population?
- What conclusion can I draw about cause?
### Predict
- How likely is point creep to keep occuring in the most prominent hunt codes?
- What is the current point creep trend in the most prominent hunt codes?
- Will point creep continue to occur in the most prominent hunt codes?
### Prescriptive
- Which hunt codes prompt action to be added to the hybrid draw list?

### Assessment of Current Situation
The Colorado Division of Wildlife current has the following Hunt Codes on the Hybrid Draw list for Elk.

|Hybrid Draw Hunt Codes|
|---|
|E-E-001-E1-R|
|E-E-002-E1-R|
|E-E-002-O1-A|
|E-E-005-W1-R|
|E-E-010-E1-R|
|E-E-010-O1-A|
|E-E-010-W1-R|
|E-E-084-W1-R|
|E-E-084-W2-R|
|E-E-085-W1-R|
|E-E-104-W1-R|
|E-E-201-E1-R|
|E-E-851-W1-R|
|E-M-001-O1-M|
|E-M-002-O1-M|
|E-M-010-O1-M|
|E-M-061-O1-M|
|E-M-201-O1-M|
|E-M-851-O1-R|
|E-M-851-O3-R|
|E-E-010-O1-A|

# Data Understanding
### Plan for Data Understanding Phase
### Tools Used
- Python Packages: pandas, requests, BeautifulSoup,pdfplumber, re, os, shutil, StringIO

### Number of data sources:
- [Colorado Parks & Wildlife - Elk Hunting Statistics](https://cpw.state.co.us/thingstodo/Pages/Statistics-Elk.aspx)

### Collecting inital Data:
- [Data Collection Code](https://github.com/AscendingToApex/Data-Science-Projects/blob/Production/Data-Driven-Draw/Data-Collection/Elk/Data-Collection-CO-Elk.ipynb)

### Describe Data

### Explore Data
#### Top 20 Most Difficult Elk Hunt Codes to Obtain a License for based on 2015-2022 CPW Draw Recap Data

Hunt Code|Total Tags|Total Applications|Supply-Demand Ratio
---|---|---|---
EE085W1R|8|1531|0.005225
EF391O1M|1|173|0.005780
EE010W1R|8|894|0.008949
EE002O1A|79|8409|0.009395
EF171P3R|4|341|0.011730
EF161P4R|4|335|0.011940
EF016P3R|8|628|0.012739
EF060O1M|5|339|0.014749
EE001O1A|16|1004|0.015936
EF009L1R|31|1815|0.017080
EE033P4R|36|2088|0.017241
EF104O1M|4|206|0.019417
EF133O1M|2|82|0.024390
EE851W4R|8|327|0.024465
EE011W1R|16|647|0.024730
EF004P1M|46|1833|0.025095
EE010E1R|256|10014|0.025564
EE010O1A|120|4692|0.025575
EE201O1A|76|2913|0.026090
EE851W2R|15|571|0.026270

#### Top 10 Most Applied for Elk Hunt Codes from 2015-2022
Hunt Code|Total Applications
--|--
EE010E1R|10014
EE002O1A|8409
EM011O1R|6888
EM061O2R|6708
EE006O1R|5996
EF011O3R|5614
EE012O1M|5353
EM043O1M|5352
EE033O1A|5287
EE201E1R|5236

#### Top 10 Most Tags Allocated for Elk Hunt Codes from 2015-2022
Hunt Code|Total Tags Awarded
--|--
EM011O1R|16278
EF011O1R|14533
EF012O2R|8867
EE007O1A|8570
EE033O1A|8100
EF004O2R|6403
EE006O1R|6080
EM041O1R|6000
EM003O1R|5527
EE012O1A|5050

#### Top 10 Hunt Codes that take the most preference points to draw for adult residents in 2022
Hunt Code| Minimum Preference Points
--|--
EE010W1R|30
EE084W1R|28
EE040W1R|27
EE851W1R|27
EE085W1R|26
EE851W2R|26
EE023W1R|23
EE104W1R|23
EM002O1M|23
EE084W2R|22

### Verify Data Quality

# Data Preparation
### Plan for Project Phase:
- [Data Preparation Code](https://github.com/AscendingToApex/Data-Science-Projects/blob/Production/Data-Driven-Draw/Data-Preparation/Elk/Data-Preparation-CO-Elk.ipynb)
### Tools Used
- Python Packages: pandas and os

# Exploratory Data Analysis
### Plan for Exploratory Data Analysis Phase
### Tools Used:
- Python packages:

### Is point creep occuring on hunt codes that are not currently on the hybrid draw list?
Point creep is currently occuring on X amount of units based on an increase in the minimum points required to draw in three out of the last seven years

### Which hunt codes is point creep occuring?
The following hunt codes have increased the minimum points required to draw in five out of the last seven years.

Hunt Code|Qty of Years Min Points Required  to Draw Increased
--|--
EE040W1R|6
EE011W2R|5
EM010O1M|5
EE003W1R|5
EE023W1R|5
EM076E1R|5
EE084W1R|5

### What does the problem space look like for the top three hunt codes with the most point creep?

### What patterns or groupings can be found in my data?


# Modeling
## Plan for Modeling Phase:

## Tools Used:

## Selecting Modeling Techniques:
### What is related to point creep?

### What can a sample tell me about the population?

### What conclusion can I draw about cause?

## Generating Test Design

## Building Model
### How likely is point creep to keep occuring in the most prominent hunt codes?

### What is the current point creep trend in the most prominent hunt codes?

### Will point creep continue to occur in the most prominent hunt codes?

## Assessing Model:


# Project Evaluation
## Plan for Project Evaluation Phase:

## Tools Used:

## Evaluating Results:

## Reviewing Next Steps:

# Deployment
## Plan for Deployment Phase

## Tools Used

## Plan Deployment

## Plan Monitoring and Maintenace

## Final Report
### Which hunt codes prompt action to be added to the hybrid draw list?

## Review Project

# Monitoring
## Plan for Project Phase

## Tools Used

## Continual modeling process evaluation and improvement
