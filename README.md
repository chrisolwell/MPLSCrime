# MPLSCrime

###OVERVIEW AND PURPOSE
Basically just to explore local crime data and keep my technical skills from disappearing completely. Maybe get some good visuals to show around.

###GENERAL SUMMARY OF ACTIONS TAKEN TO DATE
I got a dataset from https://opendata.minneapolismn.gov/datasets/cityoflakes::crime-data/about and I've been cleaning it with pandas. I was able to create dataframes for crimes against persons, crimes against property and crimes against society in the city of Minneapolis between like 2000(?) and Nov. 1 2022. I wrote code to identify datatypes, determine how best to approach null values in the dataframe, determine which data points to retain and which to discard due to irrelevance or redundancy, split data from one column into two columns, determine and list unique values, and used loc and groupby to isolate interesting data points. I added matplotlib and created a crude and useless graph.

I decided the dataset is of limited use, and its best purpose is probably for mapping, so today I built a super basic map using leaflet and mapbox. I wrote code in JavaScript, html, and css, and created a config file to store the mapbox api key. I should probably look into the dataset api because that's likely a superior way to approach the mapping project. 
