# IBM Data Science Capstone Project
To view the project notebook, please click [here](https://nbviewer.jupyter.org/github/tanyadyne/Coursera_Capstone/blob/master/Main%20Project/The%20Battle%20of%20the%20Neighborhoods%20-%20Notebook.ipynb).

To view the Coursera certificate, please click [here](https://www.coursera.org/account/accomplishments/professional-cert/7U2GEC5ZNJKJ?utm_source=link&utm_medium=certificate&utm_content=cert_image&utm_campaign=sharing_cta&utm_product=prof).

## Situation
New homeowners often take into consideration a wide range of factors when choosing where they would like to permanently reside. And families (especially those with children) often prioritise safety above all things. Beyond that, different households will also vary in terms of what they do in their free time or how they commute to work. As such, some demographics will appreciate neighborhoods with well-connected public transport, some will appreciate having many grocery shops in the vicinity, and others will prefer having plenty of clubs and restaurants to choose from.

## Task
This project is my "Applied Data Science Specialisation" Capstone completed as part of the IBM Data Science course on Coursera. Given the situation outlined above, it aims to:
a) identify the 'safest' borough in London based on crime rate
b) explore/characterise the neighborhoods within that borough (i.e. determine the most common venues in each neighborhood)
c) cluster/group those neighborhoods using k-means clustering.

## Action
I first used pandas to import a dataset containing crime statistics for the different London boroughs and preprocessed it into a readable dataframe. I then used beautiful soup to scrape additional data from Wikipedia and incoporated it into the dataframe. I then used matplotlib to visualise the crime rates in the london boroughs (looking at both the safest and least safest boroughs) and the most common *types* of crime committed. Having found the safest london borough, I create my own dataframe containing data on the *neighborhoods* within that borough. Using geocoder and geopy, I'm able to retrieve the latitude and longitude values for each neighborhood. Using the Foursquare API, I retrieved data on all venues within a 500 meter radius of each Neighborhood. I then run k-means clustering on the resulting dataframe to group the neighborhoods based on their most common venues. Finally, I use folium to visualise these clusters on a map.

## Result
I ultimately identified the safest borough to be Richmond upon Thames (RuT), a medium-sized borough with a crime rate of just 71 registered crimes per 1,000 residents. This is impressive when compared to boroughs such as Westminster and Camden that have crime rates of 364 and 179 per 1,000 residents. Note however, that although RuT has the lowest crime rate, the other five boroughs with the lowest crime rates also fall below 80 recorded crimes per 1,000 residents. Those that do not find any of the neighborhoods within RuT to suit them may therefore look into the next safest boroughs without there being too much of a difference. Nonetheless, the neighborhoods within RuT offer a good variety (as demonstrated by the five clusters). For example, a family might look into the neighborhood of Hampton as there is a very good mix of venues that will suit the needs of both the children and the parents. Single, working adults that are sociable might opt for one of the neighborhoods within cluster 0 as it offers many opportunities to eat out and meet with friends for a drink. 
