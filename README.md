# MPLSCrime

### OVERVIEW AND PURPOSE
Basically just to explore local crime data and keep my technical skills from disappearing completely. Maybe get some good visuals to show around.

### GENERAL SUMMARY OF ACTIONS TAKEN TO DATE
I got a dataset from https://opendata.minneapolismn.gov/datasets/cityoflakes::crime-data/about and I've been cleaning it with pandas. I was able to create dataframes for crimes against persons, crimes against property and crimes against society in the city of Minneapolis between like 2000(?) and Nov. 1 2022. I wrote code to identify datatypes, determine how best to approach null values in the dataframe, determine which data points to retain and which to discard due to irrelevance or redundancy, split data from one column into two columns, determine and list unique values, and used loc and groupby to isolate interesting data points. I added matplotlib and created a crude and useless graph.

I decided the dataset is of limited use, and its best purpose is probably for mapping, so today I built a super basic map using leaflet and mapbox. I wrote code in JavaScript, html, and css, and created a config file to store the mapbox api key. I should probably look into the dataset api because that's likely a superior way to approach the mapping project. 

Api wouldn't work. It's arcgis, so I installed that. Not sure why or if it's an improvement on leaflet and mapbox. Basically just manipulating the dfs in jupyter notebook in order to create graphs and save them as pdf and png files (which keep cutting off at the bottom?).

![most_popular_crimes](https://user-images.githubusercontent.com/4724180/203871725-de468326-b13d-4334-a696-b717ddad37ab.png)

![Standish_category](https://user-images.githubusercontent.com/4724180/203871780-3ea1e673-7b4f-47bd-b8b6-7b9549b4eb45.png)

These are kind of minimum viable product-type graphs for a project like this. I might just skip to tableau with this dataset....

Finally got the exploding pie aka bar of pie graph to work, although it's hard to read. I kinda don't care enough to make it beautiful right now.

![standish_crime](https://user-images.githubusercontent.com/4724180/204411403-df1a0cc7-2ce5-45a2-9190-ba7193dff77d.png)

....I did dump this data into tableau and even though I didn't get any graphs out of it immediately (more rust to shake off with tableau too) i would say that's a probably a little more user friendly.
