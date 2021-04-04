# 1. Dashboard Methodology using Python and Power BI

For this analysis I've pulled mortality data in the USA from 3 different sources in the Center for Disease Control (CDC) database. First, a large set of historical data from 2014 - 2018 that is stable in that the data will not periodically. Second, a dataset from the end of 2020 that had provisional, semi-stable mortality data for 2019. Finally the most recent dataset from 2021 that has provisional mortality data for 2020 and 2021 year to date.

These datasets overlap, so I used Python to concatenate them into a single data table and then remove all duplicate lines of data.

From this point I can plot the mortality for each year on the same chart. When I do this I can see that the number of deaths in the US in 2020 was considerably higher than those in prior years and that the excess follows a pattern not unlike the different waves of Covid-19 that were reported throughout the year.  

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mortalityhistoryi.jpg)

As I stated, the data for 2020 and 2021 is not yet stable.  The causes for this are many but simply put there is a procedure required to assigning a death to a SSN and every instance has a different level of complexity. Given this lag time I will calculate how each reporting date's mortality numbers change from week to week. These convergence indicators will indicate how long it takes for the that week's tally to stabilize.  

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/convergeh.jpg)

An interesting artifact that this chart shows is that during the holidays at the end of December and early January there was a week in which it would appear reporting was put on hold.  The week of very few death reports followed by a significant spike in reported deaths can be seen rippling back throught the data for most of January, as seen in the lines highlighted green.  

That time period of 3 weeks seems to be an anomoly, otherwise we can see that it usually takes between five and six weeks before the mortality count for that week stops changing.

This is a great look at the data at a high level, but now lets look at the details.  The combined dataset I created using Python can now be loaded onto PowerBI and interrogated with a simple report.  The report will allow the data to be sliced by year and US state, and I also include the breakout chart of causes of death for any slice.  Since any death can be from multiple causes these values do not sum to the actual mortality numbers.

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/PBIRprtTot.jpg)

Now that the overall report is created I can interrogate it for more information.  Since the mortality curves for each year are very similar before 2020 I can take a snapshot of 2019 as a baseline:

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/PBIRprt2019.jpg)

Once I've noted the death count and causes of death I can switch to 2020 and see how the overall count changes as well as the ratio of the causes.  

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/PBIRprt2020.jpg)

In this case we can see the many deaths that are Covid-19 related spring up in 2020, and calculate that in 2020 there were over 485,000 more deaths than in 2019, a 16.8% increase.

Finally we can interrogate any US state's data.  In this case we can see that Kentucky avoided the intial wave of deaths due to Covid-19 but by the third wave the mortality numbers follow the shape of the national curve.

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/PBIRprt2020KY.jpg)
