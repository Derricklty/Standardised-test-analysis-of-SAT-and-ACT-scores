# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis


### Problem Statement

From 2012 to 2018, the ACT's popularity exceeeded that of the SAT and it was only until 2019 that SAT managed to turn the tide with 55% of the market share. As an employee of the College board (the organisation that administers the SAT), this projects seeks to: (i) identify trends between SAT and ACT (based on data from 2017 to 2019) and (ii) examine if income affects the participation rates of SAT and ACT. With the relevant findings, we can then suggest possible actions to help non-technical executives of the Board maintain SAT's competitve edge over ACT (i.e. higher participation rate).

### Executive Summary

This project seeks to : (i) identify trends between SAT and ACT; and (ii) examine if income affects the participation rates of SAT and ACT. For this, we are using data on participation rates and scores for students taking the SAT and ACT tests from 2017 to 2019. More specifically, the data fields used are: 

**SAT 2017, 2018 and 2019 data**   
Comprising of the following data from all 50 US States and the District of Columbia:
1. SAT participation rates for 2017-2019 
2. Average SAT score for Evidence-Based Reading and Writing for 2017-2019 
3. Average SAT score for Math for 2017-2019 
4. Average total SAT score for 2017-2019 

**ACT 2017, 2018 and 2019 data**   
Comprising of the following data from all 50 US States and the District of Columbia:
1. ACT participation rates for 2017-2019 
2. Average ACT score for English for 2017
3. Average ACT score for Math for 2017
4. Average ACT score for Reading for 2017
5. Average ACT score for Science for 2017
6. Average composite score for 2017-2019 (i.e. mean score of all abovementioned categories)

Apart from allowing comparisons of participation rates and scores at the state-level, we are also interested in the effects of income on the participation rates of SAT and ACT. We therefore included income data from all 50 US States and the District of Columbia as follows:

**2015-2019 Income data**   
1. Median household income data from the 2015-2019 American Community Survey (5-Year estimates) 
2. Per Capita income data from the 2015-2019 American Community Survey (5-Year estimates) 
([*source*](https://data.census.gov/cedsci/table?g=0100000US.04000.001&d=ACS%205-Year%20Estimates%20Data%20Profiles&tid=ACSDP5Y2019.DP03))

**Summarised findings**  
1. Negative correlation between scores and participation rates. For instance, the correlation between SAT participation and average total score was -0.87, -0.79 and -0.86 for 2017 to 2019 respectively. Similarly, for ACT, the correlation between participation and average composite score was -0.86, -0.86 and -0.87 for 2017 to 2019 respectively. This means that higher participation rate actually leads to lower scores. Conversely, low participation rates suggests better scores due to potential selection bias in which only the most motivated students would take the tests and do well in them.
2. Correlation between participation rates for SAT and ACT are highly negative (-0.84 for 2017 and -0.87 for 2018 and 2019). This suggests that states with higher SAT participation rates tend to have a lower ACT participation rate, vice versa.
3. Correlation between incomes (either median household income or per capita income) and scores is positive for SAT but negative for ACT. For instance, correlation between median household income with: (i) sat_2018_part is 0.52; and (ii) act_2018_part is -0.53. This suggests that as a state gets richer, it tends to participate more in SAT and less in ACT.  

### Conclusions and Recommendations

**Identified trends between SAT and ACT** 
1. Studying of SAT/ACT data from 2017-2019 and income data reviews a negative correlation between test scores and participation rates. As more students participate in a test, the lower its average scores become. This could be due to the selection bias problem, in which only the most motivated and well-prepared students did well for their tests (and hence low participation rates). As such, if the College Board decides to solely increase participation rates, it would mean that a majority of juniors would not be performing very well for their tests.
2. Negative correlation between participation rates for SAT and ACT. This could mean that students see both tests as close substitutes, suggesting that states with higher SAT participation rates tend to have a lower ACT participation rate, vice versa.

**Identified trends between SAT/ACT and income**  
1. Positive correlation between SAT participation rates and income, negative correlation for ACT. This suggests that as a state gets richer, it tends to participate more in SAT and less in ACT.

**Recommendations**   
To maintian SAT's competitive edge over ACT and to increase its participation rate, we propose that:

1. The College Board focuses its attention on wooing high-income states to take part in SAT; and
2. Once these high-income states come onboard, to place more emphasis on creating and providing better preparatory materials so as to minimise the chances of observing lower average scores down the road.

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|final|Names of all US states and the District of Columbia
|sat_2017_part|float|final| Participation rate for SAT 2017 (by state)
|sat_2017_ebrw|int|final|Average SAT score for Evidence-Based Reading and Writing score in 2017 (by state)
|sat_2017_math|int|final|Average SAT score for Math in 2017 (by state)
|sat_2017_total|int|final|Average total SAT score in 2017 (by state)
|act_2017_part|float|final|Participation rate for ACT 2017 (by state)
|act_2017_eng|float|final|Average ACT score for English in 2017 (by state)
|act_2017_math|float|final|Average ACT score for Math in 2017 (by state)
|act_2017_reading|float|final|Average ACT score for Reading in 2017 (by state)
|act_2017_science|float|final|Average ACT score for Science in 2017 (by state)
|act_2017_composite|float|final|Average ACT composite score in 2017 (by state)
|sat_2018_part|float|final| Participation rate for SAT 2018 (by state)
|sat_2018_ebrw|int|final|Average SAT score for Evidence-Based Reading and Writing score in 2018 (by state)
|sat_2018_math|int|final|Average SAT score for Math in 2018 (by state)
|sat_2018_total|int|final|Average total SAT score in 2018 (by state)
|act_2018_part|float|final|Participation rate for ACT 2018 (by state)
|act_2018_composite|float|final|Average ACT composite score in 2018 (by state)
|sat_2019_part|float|final| Participation rate for SAT 2019 (by state)
|sat_2019_ebrw|int|final|Average SAT score for Evidence-Based Reading and Writing score in 2019 (by state)
|sat_2019_math|int|final|Average SAT score for Math in 2019 (by state)
|sat_2019_total|int|final|Average total SAT score in 2019 (by state)
|act_2019_part|float|final|Participation rate for ACT 2019 (by state)
|act_2019_composite|float|final|Average ACT composite score in 2019 (by state)
|sat_2017_2018_part_change|float|final| Change in participation rate between SAT 2017 and SAT 2018 (by state)
|sat_2018_2019_part_change|float|final| Change in participation rate between SAT 2018 and SAT 2019 (by state)
|act_2017_2018_part_change|float|final| Change in participation rate between ACT 2017 and ACT 2018 (by state)
|act_2018_2019_part_change|float|final| Change in participation rate between ACT 2018 and ACT 2019 (by state)
|median_household_income|float|final|Median household income 2015 - 2019 (by state)
|per_capita_income|float|final|Per capita income 2015 - 2019 (by state)
