# MPLSCrime

### OVERVIEW AND PURPOSE
Basically just to explore local crime data and keep my technical skills from disappearing completely. Maybe get some good visuals to show around.

### GENERAL SUMMARY OF ACTIONS TAKEN TO DATE
I got a dataset from https://opendata.minneapolismn.gov/datasets/cityoflakes::crime-data/about and I've been cleaning it with pandas. I was able to create dataframes for crimes against persons, crimes against property and crimes against society in the city of Minneapolis between like 2000(?) and Nov. 1 2022. I wrote code to identify datatypes, determine how best to approach null values in the dataframe, determine which data points to retain and which to discard due to irrelevance or redundancy, split data from one column into two columns, determine and list unique values, and used loc and groupby to isolate interesting data points. I added matplotlib and created a crude and useless graph.

I decided the dataset is of limited use, and its best purpose is probably for mapping, so today I built a super basic map using leaflet and mapbox. I wrote code in JavaScript, html, and css, and created a config file to store the mapbox api key. I should probably look into the dataset api because that's likely a superior way to approach the mapping project. 

Api wouldn't work. It's arcgis, so I installed that. Not sure why or if it's an improvement on leaflet and mapbox. Basically just manipulating the dfs in jupyter notebook in order to create graphs and save them as pdf and png files (which keep cutting off at the bottom?).

![most_popular_crimes](https://user-images.githubusercontent.com/4724180/203871725-de468326-b13d-4334-a696-b717ddad37ab.png)

This time in Cyberpunk:

![most_popular_crimes_cyberpunk](https://user-images.githubusercontent.com/4724180/204928827-00bae510-a41b-4081-bcfa-b287d07908eb.png)

![Standish_category](https://user-images.githubusercontent.com/4724180/203871780-3ea1e673-7b4f-47bd-b8b6-7b9549b4eb45.png)

And cyberpunk: 

![Standish_category_cyberpunk](https://user-images.githubusercontent.com/4724180/204928942-2322d314-84d8-414d-bc83-73fe1d0706db.png)

These are kind of minimum viable product-type graphs for a project like this. I might just skip to tableau with this dataset....

Finally got the exploding pie aka bar of pie graph to work, although it's hard to read. I kinda don't care enough to make it beautiful right now.

![standish_crime](https://user-images.githubusercontent.com/4724180/204411403-df1a0cc7-2ce5-45a2-9190-ba7193dff77d.png)

In Cyberpunk style:
![standish_crime_cyberpunk](https://user-images.githubusercontent.com/4724180/204928751-2a4fa232-c8e2-48e8-b421-179717afa61d.png)

....I did dump this data into tableau and even though I didn't get any graphs out of it immediately (more rust to shake off with tableau too) i would say that's a probably a little more user friendly.

So I had to do a bunch of stuff to create a line graph showing crimes by month in Standish. I did that in Cyberpunk. Here's that graph:

![cpm_cyberpunk](https://user-images.githubusercontent.com/4724180/206877086-a547d59f-61f4-443c-907a-b6eecd007cc7.png)

I dumped the standish data into a new csv and ran that in a new notebook called standish_time.ipynb. I had to convert the date columns to dt, and sort them to inlcude crimes only crimes that occurred on or after Jan. 1, 2019, so that's the scope I guess is the word I'm thinking of. I aslo dropped a bunch of columns to eliminate the nerdiest stuff. For some reason the savefig thing I tried to write into the code didn't work? I got this file using the download icon in vs code.

*** 12/12/2022
Here is an updated chart with legend and three lines in cyberpunk:

![three_lines_WMD_cyberpunk](https://user-images.githubusercontent.com/4724180/207115811-adc4403c-2758-4ea2-97d6-6ce9cd9e44da.png)
