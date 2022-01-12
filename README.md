# 1. Dashboard Methodology using Python and Power BI

[Back to Portfolio](https://michaeljmerritt.github.io/Portfolio/)

For this analysis I've pulled mortality data in the USA from 3 different sources in the Center for Disease Control (CDC) database. First, a large set of historical data from 2014 - 2018 that is stable. Second, a dataset from the end of 2020 that had provisional, semi-stable mortality data for 2019. Finally the most recent dataset from 2021 that has provisional mortality data for 2020 and 2021 year to date.

These datasets overlap, so I used Python and Pandas to concatenate them into a single data table and then remove all duplicate data before bringing the cleaned data set into PowerBI.

From this point I can plot the mortality for each year on the same chart. When I do this I can see that the number of deaths in the US in 2020 and 2021 were considerably higher than those in prior years and that the excess follows a pattern not unlike the different waves of Covid-19 that were reported in that time.  

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mort00.jpg)

Individually choosing the year 2019 gives me baseline mortality for an average year in the US.

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mort01.jpg)

Choosing 2020 shows a significant increase in mortality.

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mort02.jpg)

Choosing 2021 shows that mortality in the second year of the pandemic is on track to exceed 2020.

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mort03.jpg)

This is a great look at the data at a high level, but now lets look at the details.  The combined dataset I created using Python can now be loaded onto PowerBI and interrogated with a simple report.  The report will allow the data to be sliced by year and US state, and I also include the breakout chart of causes of death for any slice.  Since any death can be from multiple causes these values do not sum to the actual mortality numbers.

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/Cases00.jpg)

Now that the overall report is created I can interrogate it for more information.  Since the mortality curves for each year are very similar before 2020 I can take a snapshot of 2019 as a baseline:

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/Cases01.jpg)

Once I've noted the death count and causes of death I can switch to 2020 and see how the overall count changes as well as the ratio of the causes.  

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/Cases02.jpg)

In this case we can see the many deaths that are Covid-19 related spring up in 2020, and calculate that in 2020 there were over 485,000 more deaths than in 2019, a 16.8% increase.

Finally we can interrogate any US state's data.  In this case we can see that Kentucky avoided the intial wave of deaths due to Covid-19 but by the third wave the mortality numbers follow the shape of the national curve.

[Back to Portfolio](https://michaeljmerritt.github.io/Portfolio/)
