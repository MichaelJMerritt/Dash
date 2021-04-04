# 1. Dashboard Methodology using Python and Power BI

Large amounts of data needs to be collected before many analyses can be made.  This can be public data downloaded or scraped from websites or it can be queried from private databases.  Often this data is not immediately in a useable form and must be processed in order to make sure that any missing data is accounted for and the data types are consistent.  

For this analysis I've pulled mortality data in the USA from 3 different sources in the Center for Disease Control (CDC) database.  First, a large set of historical data from 2014 - 2018 that is stable.  Second, a dataset from the end of 2020 that had provisional, semi-stable mortality data for 2019.  Finally the most recent dataset from 2021 that has provisional mortality data for 2020 and 2021 year to date.

These datasets overlap, so I used Python to concatenate them and then remove all duplicate lines of data.

From this point I simply plot the mortality for each year and then calculate the difference in mortality between 2019 and 2020.  When we do this we can see that the number of deaths in the US in 2020 was considerably higher than those in prior years and that the excess follows a pattern not unlike the different waves of Covid-19 that were reported throughout the year.  It is also interesting to note that the number of excess deaths as of mid-December is considerably higher than any of the reported Covid-19 tallies from that timeframe. 

![Image of Chart](https://michaeljmerritt.github.io/Portfolio/Images/mortalityhistoryi.jpg)

Since the data for 202 and 20221 is not yet stable I calculate how each reporting date's mortality numbers change from week to week.  These convergence indicators are shown on the next chart and looking at them we can understand how long it takes for the that week's tally to stabilize.  

An interesting artifact that this chart shows is that during the holidays at the end of December and early January there was a week in which it would appear reporting was put on hold.  The week of very few death reports followed by a significant spike in reported deaths can be seen rippling back throught the data for most of January.  

But that few week time period seems to be an anomoly, otherwise we can see that it usually takes between five and six weeks before the mortality count for that week stops changing.

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/convergeh.jpg)

This is a great look at the data at a high level, but now lets look at the details.  The combined dataset I created can be opened with PowerBI and interrogated with a simple report that allows the data to be sliced by year and US state.  The data also includes causes of death for any slice.  Since any death can be from multiple causes these values do not sum to the actual mortality numbers.

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/PBIRprtTot.jpg)

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/PBIRprt2019.jpg)

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/PBIRprt2020.jpg)

![Image of Convegence](https://michaeljmerritt.github.io/Portfolio/Images/PBIRprt2020KY.jpg)
