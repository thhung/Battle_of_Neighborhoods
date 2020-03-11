# Location recommendation for business

## 1. Introduction
### 1.1. Background

Office location is always a important factor for any business owner. Not only, with a good location, companies, restaurants can rise the awareness of customers but also could reduce the cost for transportation. However, a good location requires a large rental cost. A good tradeoff between the goodness and price could be a boost for any business. However, the movement of customer usually changing from years to years, seasons by seasons. For example, in the summer, people have tendency to go to the sea. On the other hand, they usually look for a cozy place in downtowns. It is also important to aware about the competitors in the same region. Usually, people with the same business are attracted to the same place. Therefore, it is advantageous to know these information beforehand. This kind of problem could be applied for any city in the world. In this particular project, Toronto was chosen.     

### 1.2. Problem

Data that could help to determine this place include: trending venues in a given street or neighborhood, attractiveness of similar business, rental prices on these neighborhoods (if available). We could also introduce some metrics to measure an attractiveness of given street for this specific business. This project aims for giving a recommendation base on these informations.       

### 1.3. Interest

As the name of this report, this project is interested by any business owner, specially a small business such as coffee shops, restaurants which location is critical for their business.

## 2. Data
### 2.1. Data Sources
Most of information about the venues at Toronto could be gathered by Foursquare's data. For example, Foursquare API not only provides the trending venues at a specific location but also gives the similar venues. These kinds of data could be used to determine similar neigborhoods and venues. These factors could be indicators for location selection.      
### 2.2. Data wrangling
Most of the time, Foursquare API could provide very good data given good location information. However, sometime, these information might be missing either by network (in my case) or lacking of information from the database of Foursquare. I will need to remove this kind of missing from my recommendations. It is also good to recommend a place when we have good informations rather than some places that we doesn't has any information. 

Format of data provides from Foursquare API is json. I will need to transform it into a dataframe and quantify these information into numerical format that I could use to compare between the neigborhoods and adding this factor for my location metrics. 

Each neighborhood will have different venues. The atractiveness of a given place will not only depends purely on the number of venues. Therefore, this data need to be normalized to be compared fairly. 

The details of this process will be described after data collection. 


