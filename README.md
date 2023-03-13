# Airbnb-Exploratory-Data-Analysis


## Project Summary
Airbnb stands for 'Air Bed and Breakfast', and it is an online service that lets property owners rent out their premises, houses, or places to travelers looking for a place to stay. The prices of Airbnb premises are comparatively cheaper than hotels. And it allows the owner to fix the price of premises for the traveler. These days' people are preferring Airbnb to stay instead of expensive and luxurious hotels. In this growing industry, there is a lot of competition among hosts, all hosts want to make their listings attractive, and it is difficult for some hosts to make their listings attractive. Using data science, we make this problem quite simple by collecting lots of data and analyzing it using python's libraries (i.e., pandas, numpy, seaborn, and matplotlib). This analysis helps us to attract customers and give them world-class service at their level, and so different types of factors like price, area, reviews, and services affect their choices. Here, we will analyze the data and try to make a correlation between different variables, and find the relation between top listings so that in the future a host can take business decisions using these insights gained after EDA.

## Problem Statement

With the given data, our first step is to identify all the variables and find out the relationship between them. Our first sub-problem is that first focus on its physical features and its facilities and find out the relationship between top listings with prices. We mainly focused on the listing's room type, the property type, price, host, location, and reviews.

id: all properties have a unique id by which we tried to find unique properties.

Host_id: all the hosts have a unique id by which we tried to find unique number of hosts, their maximum number of listings, most popular host and their charges.

Neighbourhood_group & neighborhood: by this, we tried to find out which neighborhood group has the maximum number of properties, which one is the most popular, which one is the most expensive place to live.

Room_type: In the given data, there are three types of rooms are available that is private, shared, and entire home and we tried to find out which types of rooms are the most popular and most expensive.

Number_of_reviews: by this, we tried to find out which property has the best service and which host provides the best service.

Availability_365: by this, we tried to find the availability of the property.



### Define Your Business Objective?
Exploratory data analysis of NYC Airbnb Bookings Analysis by analyzing all the variables, we have to find the factor that will help the host to grow their Airbnb business.

## Know Your Data

- Dataset Loading
- Dataset First View
- Dataset Rows & Columns count
- Dataset Information
- Duplicate Values
- Missing Values/Null Values

### What did you know about your dataset?
Since 2008, guests and hosts have used Airbnb to expand on traveling possibilities and present a more unique, personalized way of experiencing the world. Today, Airbnb has become one of a kind service that is used and recognized by the whole world. Data analysis on millions of listings provided through Airbnb is a crucial factor for the company. These millions of listings generate a lot of data that can be analyzed and used for security, business decisions, understanding of customers' and providers' (hosts') behavior and performance on the platform, guiding marketing initiatives, implementation of innovative additional services, and much more. This dataset has around 49,000 observations with 16 columns, and it is a mix of categorical and numeric values.

### Variable Description

- id: In our dataset, every premise has a unique id
- host_id: All the hosts have unique IDs by which they are working, and a host has multiple IDs.
- neighbourhood_group & neighborhood: Within our dataset, four neighborhood groups contain multiple numbers of the neighborhood in which Airbnb is working.
- room_type: in the given data, there are three types of rooms available that is private, shared, and the entire home.
- number_of_reviews: All the premises are reviewed and rated by users based on their living experiences.
- Availability_365: In this, it has been talked about the availability for how many days the premises remain available for booking throughout the year.
- latitude & longitude: The location of each premise has been given here.
- minimum_nights: It is given the minimum number of nights that people stay on this premises.
- calculated_host_listings_count: It denotes how many hosts are registered in this particular premises.





### Check Unique Values for each variable
## Data Wrangling


Our dataset has 7894 unique properties, and 16 variables (or features). Each of the rows has a property name that has a unique ID and their host, and where that property is located with some other features like room types, reviews, and price. Our first task is to focus on its physical features and its facilities and find out the relationship between top listings prices. We mainly focused on the listing's room type, property type, price, host, location, and reviews. In the given dataset, there are a lot of null values in two columns (last_review and reviews_per_month). So, we drop these columns from the datasets. When we checked about hosts, we came to know that we have 11452 unique hosts. And in our entire dataset, about 48895 hosts are registered which means that a particular host is registered in multiple properties. When we further investigated, we found that Sonder (NYC) is the most registered host followed by Blueground, kara, and Kazuya. And we checked the calculated host listing count corresponding to their neighborhood group, and we came to know that the maximum number of the hosts are registered in Manhattan followed by Brooklyn, Queens, Bronx, and Staten Island.

## Data Vizualization, Storytelling & Experimenting with charts : Understand the relationships between variables

#### Chart - 1 : Pie chart of Room types or Proportions of RoomType (Univariate)
#### Chart - 2 Distribution density plot of Price (Univariate)
#### Chart 3- Pi chart of unique host count by its name in each neighbourhood group (Univariate)
#### Chart - 4 Bar plot of Top 3 active host in each neighbourhood group.
#### Chart - 5 Finding the top 5 host based on calculated_host_listings_count (Bivariate)
#### Chart - 6 Numbers of Unique room type in each neighbourhood group.(Bivariate)
#### Chart - 7 Revenue generated from different neighbourhood group (Bivariate)
#### Chart - 8 Average money spend by people on each room types.(Bivariate)
#### Chart - 9 Scatter plot of number of reviews and price considering the room types (mutivariate)
#### Chart -10 Scatter Plot between the longitude and latitude considering the neighbourhood_group (Mutivariate)
#### Chart - 11 Scatter plot denoting the distribution of locations of rooms in each neighbourhood (multivariate)
#### Chart - 12 Bar plot of Availability of room types (Multivariate)
#### Chart - 13 On an average for how many nights people stayed in each room_types.(Multivariate)
#### Chart - 14 - Correlation Heatmap
#### Chart - 15 - Pair Plot

### Solutions to make the host listings attractive.

* Periodically look at the customer reviews so that based on the review host can upgrade the rooms.
* The host must follow the business pattern of top active hosts.
* The host must focus on the Private and Entire home/Apt because its demand is high.
* The Premises should be in the Average price range of each room type in the respected neighborhood group.
* By keeping eye on the nearest host premises whether they giving any offers or not to visitors to increase their bookings.
* By keeping an eye on the location of premises that in which location demand for which room types is high.
* The new host must open his premises in the Manhattan neighborhood group because in manhattan the bookings are and most of the revenue of Airbnb is generated from Manhattan as compared to other neighborhood groups.
* It can be the best opportunity for the host to add his premises to the Staten Island neighborhood group because here premises are low in number and there will be less competition between the hosts.
* They have to maintain their rating for this, along with the price they will also have to provide great service to the customer
* Stay competitive and updated

## Conclusion
- Busiest place is Manhattan followed by Brooklyn.
- Based on the host listing count the maximum number of hosts are registered in Manhattan.
- The Maximum number of unique hosts (that are currently booked in the given dataset) in Brooklyn.
- Visitors prefer to stay in private type rooms or Entire Home/Apt but among these visitors are liking the Entire Home/Ap the most.
- The room types whose price is low, and are getting comparatively more reviews. So, the rooms are getting booked whose price is low.
- The most expensive premises is Entire Home/Ap type, yet people prefer to stay in it, the cheapest is the shared room type, yet people do not like to live in it.
- Based on the reviews Premises in Manhattan got the most Positive Reviews followed by Brooklyn.
- Based on price, the most expensive place is Manhattan followed by Brooklyn and the cheapest is the Bronx yet people prefer to live in Manhattan and Brooklyn.
- The maximum Revenue generated from Manhattan followed by Brooklyn.
- On average spending of people on the Home/Apt type is 212 dollar followed by Private type room is 90 dollar and Shared room 70 dollar.
- From the above analysis we found that Manhattan and Brooklyn is the most attractive place for tourists and also are the best place from a business perspective for the Hosts.
