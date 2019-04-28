# Marvin Miranda Olmedo - Chicago Speed Violations 

https://public.tableau.com/profile/marvin.olmedo#!/vizhome/4_28_19/Dashboard1

# The making process of visualization# 1

## There are more cameras in impoverish areas. Specifically, if Hardship Index is above 70.


While doing the data exploration assignment, I questioned the skewness of some cameras.

For example, Camera ID 149 had by far the most violations. I found it interesting and thought it deserved a deeper analysis and understanding. 

![Pic1](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic1.png "Skewdata")


At first, I couldn’t make any assertions about why some areas and cameras had disproportionately higer amount of violations. However, I felt the City of Chicago website did not provide enough information to justify their claim that cameras were installed around 1/8 of a mile from schools and parks. ("Children's Safety Zone Program & Automated Speed Enforcement")

Because of this, I suspected the skewness was due to the location of the cameras. This would I believed lead me to an interesting finding.

I started by investigating zip codes and realized that the original dataset presented the following limitations:
-	Zip codes were wrong
- Community areas and wards did not provide obvious insights

I tackled the the zip code issue by exploring other data sets and I came across the Socio Economics Issue Data set from the City of Chicago. ("Census Data - Selected socioeconomic indicators in Chicago, 2008 – 2012 | City of Chicago | Data Portal")

This data set provided a column called Hardship Index, which collects socioeconomic indicators of the residents of Chicago.

This Index assigns areas with more poverty a higher ranking and vice versa.

I suspected at this point that location of cameras could be driven by economic issues and thus decided to explore differences betweent impoverish and rich areas.

Visualization number one would attempt to find if there are more cameras in lower income zip codes across Chicago and thus skewed the results of violations.

I plotted a count of cameras to hardship index. The first graph did not show obvious bias.

![Pic2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic2.png "Countofcameras")

I also tried to graph a linear graph to see if there was an increment of cameras as Hardship increased. In this image, there was improvement yet there was alot of missing values.

![Pic2.2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic2.2.png "Lines")

I then created a calculated field that assigned any Hardship index above 50 to Poor else Rich, with the intention to find a correlation.

This image did show that there are more cameras in poorer areas, but I didn't think it was convincing enough.
I also took a detour in my thinking. Up to this point, I wanted to proof with my visualization to the Mayor of Chicago that I had found evidence that empoverish areas are more police. I decided that that is not the message I would try to convey.

![Pic3](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic3.png "Calculatedfield")

Finally, I decided to bin the Hardship Index in size bins of 10 and this is where I found a straight answer to my question.


There are more cameras in poorer areas than in rich areas. Specifically if Hardship Index is above 70 and this is the message that I would covey.


![FinalPic#1](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPic%231.png "Visualization#1")

### Future enhancements

- A future enhancement to this visualization would be to optain school locations to prove or disprove that cameras have been installed 1/8 of mile from schools as the City of Chicago Claims.
- Consider other socio economic factors that may be affecting the location of cameras
- Explore population differences among indexes.


# The making process of visualization #2

## The city of Chicago is divided into 50 wards, each with 1 representative. Out of the 50 there is one not controlled by democrats or Republicans and it is the one with the highest violations. 
## The Ward with the only Independent Representative has the highest amount of Violations.

While researching the zip code issue from the original data set I came to realize that I did not understand the meaning of the Wards. 

I turned to Wikipedia and found data on wards and how each has a political representative. ("Chicago City Council", 2019)

Quickly realized that the City of Chicago has a democratic majority and it would be interesting to see if Wards ran by other parties differed from democrats.

At first, I plotted zip codes which required me to download another Data set called Ward Offices. ("Ward Offices | City of Chicago | Data Portal")

I had to split column location to create Longitude and Latitudes.

I then created a map of violations by zip code and party.

From this image, I couldn’t  make any clear statements about violations and parties.


![Pic4](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic4.png "zip code")


I then proceeded to think of Wards rather than zip codes and created a visualization that showed violations by Wards.

Here is where I found my interesting finding; there are only 2 Wards not controlled by Democrats, one of them is an Independent and the other is a Republican. 

The Ward with the highest amount of violations is represented by an Independent.

I thought this was a very intersting finding that does not imply or claim anything but is something I was not expecting.

![FinalPic2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPic%232.png "Visualization#2")

### Future enhancements
 - I would like to explore demographics of this Ward
 - I would like to see if this Ward differs from others on socio economic factors
 


# The making process of visualization #3

In the data exploration process, I designed a visualization that showed Friday as the day with more violations. I received criticism and thus decided to build on that mistake. Perhaps, explore if this visualization could lead to an interesting finding.

Picture
![Friday](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic5.png "Friday")

From feedback received, I wanted to explore different ways to properly show this information.  I decided to explore changes through out the years instead of day. 

Picture
![Pic6](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic6.png "Years")

After analyzing weekdays and years, I decided to add weekends and realized that on average Friday is not the day with more violations.

Thi is an intersting finding considering the fact that I had originally in the data exploration process claimed Friday had the highest amount.

![FinalPic3](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPic%233.png "Visualization#3")


### Future enhancements
- Would like to create a forecast
- Would like to breakdown by wards
- Would like to compare by zip code and Socio economic Factors


# Data Wrangling


- I had to retrieve information from multiple sources.

- Combined all Data Sets into a spreadsheet.

- Mapped and joined the tables. 

![joinss](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Jointss.png "joinss")


- I had to physically draw the attributes I needed to analyze if joining the different data sets was feasible.

![joins](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Joins.png "joins")

- Created bins for Harship Index

![bins](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/bins.png "bins")

- Created IF statements to categorize rich or poor in the column called Harship Index.

![if](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Calculated%20field.png "ifstatements")

- Split columns to find Longitude and Latitude of Wards.


# References

- Children's Safety Zone Program & Automated Speed Enforcement. (n.d.). Retrieved April 27, 2019, from https://www.chicago.gov/city/en/depts/cdot/supp_info/children_s_safetyzoneporgramautomaticspeedenforcement.html

- Census Data - Selected socioeconomic indicators in Chicago, 2008 – 2012 | City of Chicago | Data Portal. (n.d.). Retrieved April 27, 2019, from https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2

- Chicago City Council. (2019, April 26). Retrieved April 27, 2019, from https://en.wikipedia.org/wiki/Chicago_City_Council

- Ward Offices | City of Chicago | Data Portal. (n.d.). Retrieved April 27, 2019, from https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Ward-Offices/htai-wnw4

