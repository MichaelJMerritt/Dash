# 1. Dashboard Methodology using Python and Power BI

[Back to Portfolio](https://michaeljmerritt.github.io/Portfolio/)

For this analysis I've pulled mortality data in the USA from 3 different sources in the Center for Disease Control (CDC) database. First, a large set of historical data from 2014 - 2018 that is stable. Second, a dataset from the end of 2020 that had provisional, semi-stable mortality data for 2019. Finally the most recent dataset from 2021 that has provisional mortality data for 2020 and 2021 year to date.

These datasets overlap, so I used Python and Pandas to concatenate them into a single data table and then remove all duplicate data before bringing the cleaned data set into PowerBI.  From this point I can plot the mortality for each year on the same chart. The report will allow the data to be sliced by year and US state, and I also include the breakout chart of causes of death for any slice.  Since any death can be from multiple causes these values do not sum to the actual mortality numbers.  

When I do this I can see that the number of deaths in the US in 2020 and 2021 were considerably higher than those in prior years and that the excess follows a pattern not unlike the different waves of Covid-19 that were reported in that time.  

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mort00.jpg)

Individually choosing the year 2019 provides baseline mortality for an average year in the time before the Covid pandemic.

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mort01.jpg)

Choosing 2020 shows a significant increase in mortality in the first year of the Covid pandemic.

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mort02.jpg)

Choosing 2021 shows that mortality in the second year of the pandemic is on track to exceed 2020.  It is als interesting to notefrom the cause of death section that the percentage of deaths of natural causes remains more or less constant despite the increase due to Covid.  This suggests that the 

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mort03.jpg)

For this next analysis I use only a single dataset from the CDC that has detailed information on Covid cases in the US categorized by age, race and sex.  Each case also has information regarding the severity of the case including hospitalization and death. 

In the charts I've shown the Covid identified cases in the left pane, the deaths in the top-center pane and the death rate by age group in the bottom-center pane.  I added a number of slicers to the right to further study different sections of the population.

Its interesting to note that while looking at the total population the death rate increases non-linearly with age.  In fact the death rate for people under 40 years old is extremely small.

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/Cases00.jpg)

Clicking the 80+ age group show that while the total number of Covid cases is relatively small the death rate from these cases in very large.

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/Cases01.jpg)

Clicking the 30-39 age group shows that while folks in this age group contracted five times as many Covid cases as 80+ year old people there were only one twentieth as many deaths.

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/Cases02.jpg)

[Back to Portfolio](https://michaeljmerritt.github.io/Portfolio/)
