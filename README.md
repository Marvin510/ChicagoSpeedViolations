# Marvin Miranda Olmedo - Chicago Speed Violations 

# The making process of visualization# 1

## There are more cameras in impoverish areas. Specifically, if Hardship Index is above 70.


While doing the data exploration assignment, I questioned the skewness of some cameras.

For example, Camera ID 149 had by far the most violations. I found it interesting and thought it deserved a deeper analysis and understanding. 

![Pic1](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic1.png "Skewdata")


At first, I couldn’t visualize it but the more I thought about the amount of violations and how some cameras had a higher amount, made me wonder whether or not cameras were placed as the website claims around 1/8 of a mile from schools and parks. ("Children's Safety Zone Program & Automated Speed Enforcement")

I investigated zip codes and realized that the original dataset presented the following limitations:
-	Zip codes were wrong
- Community areas and wards didn’t have a meaning

At first, I tried to solve the zip code issue by exploring other data sets and I came across the Socio Economics Issue Data set from the City of Chicago. ("Census Data - Selected socioeconomic indicators in Chicago, 2008 – 2012 | City of Chicago | Data Portal")

This data set provided a column called Hardship Index, which collects socioeconomic indicators of the residents of Chicago.

This Index assigns areas with more poverty a higher ranking.

I then realize that I could start exploring any differences between impoverish and rich areas.

Visualization number one would attempt to find if there are more cameras in lower income zip codes across Chicago and thus skewed the results of violations.

I plotted a count of cameras to hardship index. The first graph did not show obvious bias.

![Pic2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic2.png "Countofcameras")

I also tried to graph a linear graph to see if there was an increment of cameras as Hardship increased. In this image, there was improvement yet there was alot of missing values.

![Pic2.2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic2.2.png "Lines")

I then created a calculated field that assigned any Hardship index above 50 to Poor else Rich, with the intention to find a correlation.

This image did show that there are more cameras in poorer areas, but I didn't think it was convincing enough.

![Pic3](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic3.png "Calculatedfield")

Finally, I decided to bin the Hardship Index in size bins of 10 and this is where I found a straight answer to my question.


There are more cameras in poorer areas than in rich areas. Specifically if Hardship Index is above 70.


![FinalPic#1](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPic%231.png "Visualization#1")

### Future enhancements

- A future enhancement to this visualization would be to optain school locations to prove or disprove that cameras have been installed 1/8 of mile from schools as the City of Chicago Claims.
- Consider other socio economic factors that may be affecting the location of cameras
- Explore population differences among indexes.


### The making process of visualization #2

## The city of Chicago is divided into 50 wards, each with 1 representative. Out of the 50 there is one not controlled by democrats or Republicans and it is the one with the highest violations. The Ward with the only Independent Representative has the highest amount of Violations.

While researching the zip code issue from the original data set I came to realize that I did not understand the meaning of the Wards. 

I turned to Wikipedia and found data on wards and how each has a political representative. ("Chicago City Council", 2019)

Quickly realize that the City of Chicago has a democratic majority and it would be interesting to see if Wards ran by other parties differed from democrats.

At first, I plotted zip codes which required me to download another Data set called Ward Offices. ("Ward Offices | City of Chicago | Data Portal")

I had to split column location to create Longitude and Latitudes.

I then created a map of violations by zip code and party.

From this image, I couldn’t  make any clear statements about violations and parties.


![Pic4](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic4.png "zip code")


I then proceeded to think of Wards rather than zip codes and created a visualization that showed violations by Wards.

Here is where I found my interesting  finding; there are only 2 Wards not controlled by Democrats, one of them is an Independent and the other is a Republican. The Ward with the highest amount of violations  is represented by an Independent.

I thought this was a very intersting finding that does not imply or claim anything but is something I was not expecting.

![FinalPic2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPic%232.png "Visualization#2")

### Future enhancements
 - I would like to explore demographics of this Ward
 - I would like to see if this Ward differs from others on socio economic factors
 


### The making process of visualization #3




### The making process summary


- I had to retrieve information from multiple sources, combined all into a spreadsheet and then I had a hard time mapping and joining the tables. 

- I had to physically draw the attributes I needed to analyze if joining the different data sets was feasible.

![joins](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Joins.png "joins")

- Created bins for Harship Index

- I also had to create calculated fields such as bins 

- Created IF statements to categorize rich or poor in the column called Harship Index.

###


#References

- Children's Safety Zone Program & Automated Speed Enforcement. (n.d.). Retrieved April 27, 2019, from https://www.chicago.gov/city/en/depts/cdot/supp_info/children_s_safetyzoneporgramautomaticspeedenforcement.html

- Census Data - Selected socioeconomic indicators in Chicago, 2008 – 2012 | City of Chicago | Data Portal. (n.d.). Retrieved April 27, 2019, from https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2

- Chicago City Council. (2019, April 26). Retrieved April 27, 2019, from https://en.wikipedia.org/wiki/Chicago_City_Council

- Ward Offices | City of Chicago | Data Portal. (n.d.). Retrieved April 27, 2019, from https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Ward-Offices/htai-wnw4

