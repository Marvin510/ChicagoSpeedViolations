# Marvin Miranda Olmedo - Chicago Speed Violations 

## The making process of visualization# 1

- There are more cameras in poorer areas than in rich areas. Specifically if Hardship Index is above 70.

While doing the data exploration assignment, I questioned the skewness of some cameras. For example, Camera ID 149 had by far the most violations. I found it interesting and thought it deserved a deeper analysis and understanding. 

![Pic1](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic1.png "Skewdata")


I ambition an image that would be eye opening to what I thought could be a mysterious issue.

At first, I couldn’t visualize it but the more I thought about the amount of violations and how some cameras had a higher amount made me wonder whether or not cameras were placed as the website claims around 1/8 of a mile from schools and parks. ("Children's Safety Zone Program & Automated Speed Enforcement")

The original dataset presented the following limitations:
-	Zip codes were wrong
- Community areas and wards didn’t have a meaning

At first I tried to solve the zip code issue by exploring other data sets and I came across the socio economics issue Data set from the city of Chicago. ("Census Data - Selected socioeconomic indicators in Chicago, 2008 – 2012 | City of Chicago | Data Portal")

This data set provided a column called Hardship Index, which collects socioeconomic indicators of the residents of Chicago.

I then realize that I could start by discarding the over policing of poor communities.

I plotted count of cameras to hardship index and the first graph did not show obvious bias.

![Pic2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic2.png "Countofcameras")

I also tried to graph a linear graph to see if there was an increment of cameras as Harship increased. In this image, there was improvement yet there was alot of missing values that I couldn't present.

![Pic2.2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic2.2.png "Lines")

I then created a calculated field that assigned any Hardship index above 50 to Poor else Rich, with the intention to find a correlation. This immage did showed that there are more cameras in poorer areas but I didn't think it was convincing enough.

![Pic3](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic3.png "Calculatedfield")

Finally, I decided to bin the Hardship Index in size bins of 10 and this is where I found a straight answer to my question.

There are more cameras in poorer areas than in rich areas. Specifically if Hardship Index is above 70.


![FinalPic#1](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPic%231.png "Visualization#1")


A future enhancement to this visualization would be to optain school locations to prove or disprove that cameras have been installed 1/8 of mile from schools as the City of Chicago Claims.




### The making process of visualization #2

While researching the zip code issue from the original data set I came to realize that I did not understant the meaning of the wards. 

I turned to Wikipedia and found data on wards and how each has a political representative.("Chicago City Council", 2019)

Quickly realize that the City of Chicago has a democratic majority and thought it would be interesting to see if Wards ran by other parties differed from democrats.

At first, I plotted zip codes which  required me to download another Data set called Ward Offices. ("Ward Offices | City of Chicago | Data Portal")

I had to split location to create Longitude and Latitudes. I then created a map of violations by zip code and party. From this image, I could't make any statements about violations and parties.


![Pic4](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic4.png "zip code")


I then proceeded to think of Wards rather than zip codes and created a visualization that showed violations by Wards. Here is where, I found my intersting finding. There is only 2 Wards not controlled by Democrats, one of them is an Independent and the other is a Republican. The Ward with the highest amount of vioalations is represented an Independent.

I thought this was a very intersting finding that does not imply or claim anything but is something I was not expecting.

![FinalPic2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPic%232.png "Visualization#2")





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



#References

- Children's Safety Zone Program & Automated Speed Enforcement. (n.d.). Retrieved April 27, 2019, from https://www.chicago.gov/city/en/depts/cdot/supp_info/children_s_safetyzoneporgramautomaticspeedenforcement.html

- Census Data - Selected socioeconomic indicators in Chicago, 2008 – 2012 | City of Chicago | Data Portal. (n.d.). Retrieved April 27, 2019, from https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2

- Chicago City Council. (2019, April 26). Retrieved April 27, 2019, from https://en.wikipedia.org/wiki/Chicago_City_Council

- Ward Offices | City of Chicago | Data Portal. (n.d.). Retrieved April 27, 2019, from https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Ward-Offices/htai-wnw4

