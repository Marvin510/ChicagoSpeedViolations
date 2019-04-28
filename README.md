# Marvin Miranda Olmedo
# Chicago Speed Violations - Individual Project
### 3 Aspect:  interesting, non-trivial, and somewhat unexpected 

### Picture 1


### The making process



While doing the data exploration assignment, I questioned the skewness of some cameras. For example, Camera ID 149 (1) had by far the most violations. I found it interesting and thought it deserved a deeper analysis and understanding. 

I ambition an image that would be eye opening to what I thought could be a mysterious issue.

At first, I couldn’t visualize it but the more I thought about the amount of violations (2) and how some cameras had a higher amount made me wonder whether or not cameras were placed as the website claims around 1/8 of a mile from schools and parks. (citation1)

The original dataset presented the following limitations:
•	Zip codes were wrong
•	Community areas and wards didn’t have a meaning

At first I tried to solve the zip code issue by exploring other data sets and I came across the socio economics issue Data set from the city of Chicago(citation2). This data set provided a column called Hardship Index, which collects socioeconomic indicators of the residents of Chicago.

I then realize that I could start by discarding the over policing of poor communities.

I plotted count of cameras to hardship index and first graph was not very obvious ( pic3)

I then created a calculated field that assign any Hardship index above 50 to Poor else Rich. (Pic4)

Finally decided to bin the Hardship Index in size bins of 10 and this is where I found a straight answer to my question. There are more cameras in poorer areas than in rich areas. Specifically if Hardship Index is above 70.

A future enhancement to this visualization would be to graph hardship index by zip code and wards area to better understand where are the areas targeted and why.





Had to retrieve information from multiple sources, combined all into a spreadsheet and then I had a hard time mapping and joining the tables. I had to physically draw the attributes I needed.

I tried to optain data to prove my point but ended up finding an interesting fact. that the city ward with the only independent representative has the highest violations.

I am exploring the city of Chicago data and I am realizing that perhaps I should have researched what data was available to make a decision on what to dive into.

1- In Visualization number one, I will attempt to find if there are more cameras in lower income zip codes across chicago.
 
### T
 

2- For visualization number two, I will try to find a correlation of income to violations. I will search for zip codes that differ in income and find how they differ in violations

3- Visualization number three, I will try to prove that cameras were located in poverty areas and therefore skewed the results of violations

4- Found that the city of Chicago is divided into 50 wards, each with 1 representative. Out of the 50 there is one not controlled by democrats or Republicans and it is the one with the highest vioaoations.

5 - Found that empoverish areas are more overpoliced. as expected






### Visualizations

1- Overpolicing of Poor Areas
![Viz1](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Overpolicing.png)


2-


3- Ward control by an Idenpendent has the highest Violations

![Viz3](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Independent.png)




### Future enhancements


### Conclusion



#Citations

https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Ward-Offices/htai-wnw4
https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2
https://en.wikipedia.org/wiki/Chicago_City_Council
