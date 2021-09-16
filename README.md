# IBM Data Science Capstone Project
To view the project notebook, please click [here](https://nbviewer.jupyter.org/github/tanyadyne/Coursera_Capstone/blob/master/Main%20Project/The%20Battle%20of%20the%20Neighborhoods%20-%20Notebook.ipynb).

## Situation
New homeowners often take into consideration a wide range of factors when choosing where they would like to permanently reside. And families (especially those with children) often prioritise safety above all things. Beyond that, different households will also vary in terms of what they do in their free time or how they commute to work. As such, some demographics will appreciate neighborhoods with well-connected public transport, some will appreciate having many grocery shops in the vicinity, and others will prefer having plenty of clubs and restaurants to choose from.

## Task
This project is my "Applied Data Science Specialisation" Capstone completed as part of the IBM Data Science course on Coursera. Given the situation outlined above, it aims to:
a) identify the 'safest' borough in London based on crime rate
b) explore/characterise the neighborhoods within that borough (i.e. determine the most common venues in each neighborhood)
c) cluster/group those neighborhoods using k-means clustering.

## Action
I first used pandas to import a dataset containing crime statistics for the different London boroughs and preprocessed it into a readable dataframe. I then used beautiful soup to scrape additional data from Wikipedia and incoporated it into the dataframe. I then used matplotlib to visualise the crime rates in the london boroughs (looking at both the safest and least safest boroughs) and the most common *types* of crime committed. Having found the 

## Result
The safest London borough (in terms of crime-rate) was Richmond upon Thames (RuT), and the least safest borough was Westminster. The top 3 most committed crimes within RuT were Violence against the person, theft, and vehicle offenses. The least common type of crime was weapon possession. 
