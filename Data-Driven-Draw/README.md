# Colorado Big Game Hunting Data Driven Draw

# Project Understanding
## Background:
Mike had been applying for points every year for over half his lifetime in order to hunt elk in a specific unit. April rolled around again as it had every other year he'd been applying, but this year was different. A friend told him he had enough points to draw the legendary tag this year, so he optimistically submitted the application and started planning the hunt; only to get an e-mail a short month later stating that he had once again failed to recieve the license because he didn't look through over 6,000 pages of past draw recap statistics to verify what his chances of drawing were.

This situation happens every year in some capacity to most Colorado big game hunters because of the time required and difficulty to digest the hunting statistics provided by Colorado Parks and Wildlife.

For big game hunting, Colorado uses a preference point system to increase the chances of getting the opportunity to hunt specific units over time. The hunters with the higher preference points have a higher probability of obtaining tags that require a draw than hunters with the fewer preference points. The preference points are specific to species and hunters are able to accumulate a single point per species after unsuccuessfully drawing a tag. In addition, the majority of "trophy" units have a limited number of tags available per hunt code, which is specific to species, region in colorado, time of year, and hunting method.

## Objective:
1. Determine which Hunt Codes receive the highest number of applicants.
2. Determine which Hunt Codes allocate the highest number of tags.
3. Determine Which Hunt Codes are the most difficult to draw.
4. Explore the "Point Creep" phenominon, which occurs when the number of tags available doesn't meet the demand of applicants and each year the quantity of points it takes to draw the tag increases.
5. Build a Model to predict the likelyhood of drawing a specific Hunt Code in the 2023 application based on the number of preference points the applicant has.
6. Deploy and Monitor the Model as a free resource for Colorado big game hunters to quickly evaluated which Hunt Codes they could obtain a tag for, so they are better prepared when making applications decisions for the 2023 application period. 

# Data Understanding
* Determine the number of data sources:
    - [Colorado Parks & Wildlife - Elk Hunting Statistics](https://cpw.state.co.us/thingstodo/Pages/Statistics-Elk.aspx)
* Collecting inital Data
    - [Data Collection Code](https://github.com/AscendingToApex/Data-Science-Projects/blob/Production/Data-Driven-Draw/Data-Collection/Elk/Data-Collection-CO-Elk.ipynb)
* Describe Data

# Data Preparation
* [Data Preparation Code](https://github.com/AscendingToApex/Data-Science-Projects/blob/Production/Data-Driven-Draw/Data-Preparation/Elk/Data-Preparation-CO-Elk.ipynb)

# Exploratory Data Analysis
## Top 20 Most Difficult Elk Hunt Codes to Obtain a License for based on 2015-2022 CPW Draw Recap Data

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

## Top 10 Most Applied for Elk Hunt Codes from 2015-2022
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

## Top 10 Most Tags Allocated for Elk Hunt Codes from 2015-2022
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

## Evaluate Hunt Codes for Point Creep
The "Point Creep" phenominon, which occurs when the number of tags available doesn't meet the demand of applicants and each year the quantity of points it takes to draw the tag increases.

## Modeling
* Select Modeling Techniques
* Generate Test Design
* Build Model
* Assess Model

## Project Evaluation
* Evaluate Results
* Review PRocess
* Determine Next Steps

## Deployment
* Plan Deployment
* Plan Monitoring and Maintenance
* Produce Final Report
* Review Project

## Monitoring
* Continual modeling process evaluation and improvement
