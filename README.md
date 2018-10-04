## Introduction
Kuala Lumpur and Johor Bahru are two major cities in Malaysia. Both cities become a center of attention for residential, job employment, tourism, education, shopping and sports activity. Both cities are well known in Malaysia, and become the top choice for local and foreign communities.

Brief information about both cities:  
**Kuala Lumpur**: is the national capital of Malaysia as well as its largest city. The only global city in Malaysia, it covers an area of 243 km2 (94 sq mi) and has an estimated population of 1.73 million as of 2016. Greater Kuala Lumpur, also known as the Klang Valley, is an urban agglomeration of 7.25 million people as of 2017.It is among the fastest growing metropolitan regions in South-East Asia, in both population and economic development.   
(source: https://en.wikipedia.org/wiki/Kuala_Lumpur)

**Johor Bahru**: formerly known as Tanjung Puteri or Iskandar Puteri, is the capital of the state of Johor, Malaysia. It is situated along the Straits of Johor at the southern end of Peninsular Malaysia. Johor Bahru has a population of 497,097, while its metropolitan area, with a population of 1,638,219, is the third largest in the country.  
(source: https://en.wikipedia.org/wiki/Johor_Bahru)


## Objective
In this project, we will study in details the area classification using Foursquare data and machine learning segmentation and clustering. The aim of this project is to segment areas of Kuala Lumpur and Johor Bahru based on the most common places captured from Foursquare.

Using segmentation and clustering, we hope we can determine:
- the similarity or dissimilarirty of both cities
- classification of area located inside the city whether it is residential, tourism places, or others

## Data
The data acquired from wikipedia pages and restructure to csv file for easier manipulation and reading. Both files uploaded to my github for references. Link to the files are:

- [JB District Data](https://github.com/zaephaer/CapstoneProject/blob/master/JB_disrict.csv)
- [KL District Data](https://github.com/zaephaer/CapstoneProject/blob/master/KL_disrict.csv)

Another aspect to consider for this project is the Foursquare data. I believe that the data as good as provided, meaning although we are using Foursquare data for segmentation and clustering, the amount and accuracy of data captured can't 100% determine correct classification in real world.

To start, let's get and look at the data. I've already downloaded it, so let's read it (from local drive) and load it to dataframe:
Using geocoder, we able to get Latitude and longitude for each area.

![Test Image 1](https://image.ibb.co/coJvKK/code01.png)
![Test Image 1](https://image.ibb.co/dsxNzK/code02.png)


## Methodology
In this project, I will use the basic methodology as taught in Week 3 lab.

Above, we have done convert addresses into their equivalent latitude and longitude values.
Then we will use the Foursquare API to explore neighborhoods in both cities, Kuala Lumpur and Johor Bahru
After that, explore function to get the most common venue categories in each neighborhood,
and then use this feature to group the neighborhoods into clusters
K-means clustering algorithm will be use to complete this task. And also, the Folium library to visualize the neighborhoods in Kuala Lumpur and Johor Bahru and their emerging clusters.

Based on dataframe analysis above, we found out that Bukit Bintang area in Kuala Lumpur and Johor Bahru area in Johor Bahru are both have the highest number of area within it those district.

![Test Image 1](https://image.ibb.co/kF2fKK/code03.png)
![Test Image 1](https://image.ibb.co/cPGqKK/code04.png)


## Analyze Kuala Lumpur
Analyzing Kuala Lumpur data to get most common venue for each area.
![Test Image 1](https://image.ibb.co/fdKMRz/code05.png)


## K-mean Cluster Kuala Lumpur
Using K-mean to clustering data area with most common venue
![Test Image 1](https://image.ibb.co/kXUMRz/code06.png)

![Image 1](https://image.ibb.co/foN86z/code07.png)

## Analyze Johor Bahru
Analyzing Johor Bahru data to get most common venue for each area.
![Test Image 1](https://image.ibb.co/gS84eK/code08.png)


## K-mean Cluster Johor Bahru
Using K-mean to clustering data area with most common venue
![Test Image 1](https://image.ibb.co/n7QjeK/code09.png)

![Test Image 1](https://image.ibb.co/jgcKDe/code10.png)






### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/zaephaer/CapstoneProject/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
