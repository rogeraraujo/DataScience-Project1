Project goals
=============
The main goal of this project is to analyze crime data from Montgomery County, MD (USA).

Insights and conclusions
========================
The data file describes crimes reported during a period of six months, from July to December of 2013. It contains 23,369 crimes in total. Most of the columns in each data row are described in the following link:

https://www.opendatanetwork.com/dataset/data.montgomerycountymd.gov/icn6-v9z3

Many of the columns refer to crime locations, with an increasing level of granularity. A Police District is divided into Sectors; a Sector is divided into Beats; a Beat is divided into Police Response Areas (PRAs). While the Police District column has no null values, it is probably not granular enough for detailed analyses. The Sector column has 46 null values and, perhaps surprisingly, the Beat column has only 8 null values. Fortunately, the Beat can be used to derive the Sector, which alleviates the problem of null values in that column. Detailed maps are available in the following links:

https://www.montgomerycountymd.gov/pol/districts/map.html
http://mcgov-gis.maps.arcgis.com/apps/Viewer/index.html?appid=4317830a05654b8f907e65515970a5ba

132 crimes have no address number, and 161 numbers have no exact geographic coordinates. These rows amount to less than 1% of the total.

The city of GERMANTOWN has the lowest population (131,391). With 2,755 crimes, it has a rate of 0.020 crimes per capita. The city of WHEATON has the highest population (208,263). With 4,375 crimes, it has a rate of 0.021 crimes per capita. The city of SILVER SPRING, with a population of 152,991 and 5,533 crimes, has the highest rate of crimes per capita, at 0.036. The city of BETHESDA, with a population of 182,883 and 3,383 crimes, has the lowest rate of crimes per capita, at 0.018.

There are 285 different crime class IDs, with corresponding descriptions. They can be organized by range in 27 distinct groups. Crime IDs in the 111-199 range correspond to HOMICIDE, with the least number of crimes, at 4 occurrences. Crime IDs in the 611-699 range correspond to LARCENY, with the highest number of crimes, at 6,277 occurrences. When it comes to violent crimes, the most common ID range is 811-899, ASSAULT & BATTERY, at 1,380 occurrences. As for non-violent crimes, the most common ID range is 611-699, LARCENY, at 6,277 occurrences.

The city with the highest number of both violent and non-violent crimes is SILVER SPRING. The number of violent crimes is 1,574, and non-violent is 3,959.

The month with the highest number of violent crimes is September, with 1,305 crimes. There is a noticeable increase in the number of violent crimes from July (1,083) to August (1,299), which is probably because the school year starts in August/September in the northern hemisphere. The month with the highest number of non-violent crimes is October, with 2,818 crimes. There is also an increase in the number of non-violent crimes from July (2,437) to August (2,703), probably for the same reasons as discussed for violent crimes. The data file only spans six months of a single year; therefore, it should be difficult to make additional assumptions about seasonal phenomena.

The total number of violent crimes is highest on Monday, at 1,215 crimes, and it decreases steadily along the week, with the total count stabilizing at 905 for both Saturday and Sunday. The total number of non-violent crimes is highest on Tuesday, at 2,644 crimes. There is no noticeable trend during working days, but there is a sharp drop at weekends, with a total of 1,902 crimes at Saturday and 1,478 crimes at Sunday.

Necessary APIs
==============
Pandas (http://pandas.pydata.org/)
NumPy (http://www.numpy.org/)
Matplotlib (http://matplotlib.org/)

The team
========
Eduardo Santos
Hilário Castro
Roger Araújo

