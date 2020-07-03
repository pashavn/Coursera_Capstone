# Coursera_Capstone

Where to Go When You Want to Eat Vietnamese Restaurant ?
Data Science Capstone - IBM Data Science Professional Certificate on Coursera

Introduction
Let’s say you have never been to the US and you want to have only Vietnamese food while you are there. So you want to go to a place with a high density of Vietnamese Restaurant places around you. The problem we aim to solve is to analyze the Vietnamese Restaurant locations in the New York and Chicago cities and compare where is the crowded Vietnamese Restaurant places 

Data section
I will use the FourSquare API to collect data about locations of Vietnamese Restaurant in 2 major US cities which are: New York and Chicago

Methodology
My main target here is to asses which city would have the highest Vietnamese Restaurant density. I used the Four Square API through the venues channel. I used the near query to get venues in the cities. Also, I use the CategoryID to set it to show only Vietnamese Restaurant. An Example of my requests:
https://api.foursquare.com/v2/venues/search?ll=40.7484,-73.9857&client_id=H3EDOOGKQWA0FHZSMUH5H3JUVSJKFZEJFXHJ3EXZQYCWVDWF&client_secret=DYTYCCP1010KEX2RRT2OJDZPISGJGI31AUG0M3WZHB35ER0C&v=20180605&New York, NY&radius=250&limit=100&categoryId=4bf58dd8d48988d14a941735

That 4bf58dd8d48988d14a941735 is the Id of the Vietnamese Restaurant Category. Also, Foursquare limits us to maximum of 100 venues per query.

Moreover, I repeated this request for the 2 studied cities and got their top 100 venues. I saved the name and coordinate data only from the result and plotted them on the map for visual inspection.

Results
We now see that New York is the best option for us to enjoy any Vietnamese Restaurant Food !!!


