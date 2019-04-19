## The Battle of Neighbourhoods project

### Exploring the restaurants of Tokyo - Week 1 report

**Background:**

Just a year is left until 2020 Tokyo Olympic Games. Tokyo is my home city, and I decided to focus my research on Tokyo and its restaurants. Probably the resulting data would be helpful for enterpreneurs who is looking forward to start their restaurant in Tokyo. This research can be adapted to check on any possible cuisine or restaurant type.

Tokyo is quite diverse when it comes to dining options. Though the most popular cuisine is Japanese, every other possible cuisine can be found. There are plenty of Chinese, Korean, Thai, Italian and Indian restaurants. We also have theme restaurants like Ninja cafes, maid cafes, animal cafes, or prisoner cafe called Lock-up.

Mexican cuisine is very popular worldwide, but there's still lack of Mexican restaurants in Japan. That's a pity! Mexican food is tasty, nutritious and quick to make. Many visitors of 2020 Olympic Games would be disappointed if they won't find their favourite tacos or burritos to snack on while cheering for national Olympic team. Let's have a look at Mexican restaurants in Tokyo, their locations and possible business opportunities.



**1: Business Problem**

A friend of mine, who is currently living in Cancun, Mexico, and running his own Mexican restaurant, contacted me recently. Just a year is left until Tokyo 2020 Olympic Games start, so Tokyo is going to welcome a lot of guests from abroad. My friend was wondering is there any Mexican restaurants in Tokyo, and where are they located? If he decides to open his own Mexcian restaurant, which area should he choose? 



**2: Data**

Tokyo consists of 23 wards, or special areas, which bear some resemblance to New York's boroughs. I've prepared a list of 23 wards and their coordinates in csv format.

First, we will utilize Foursquare API to have a look at what Tokyo is like, and venues are most common for each ward. we will then use Foursquare API to find information on Mexican restaurants, their locations and ratings.



**3: Methodology**

K-means clustering was used to perform the Tokyo city segmentation. The wards of Tokyo city were grouped into five clusters and most common venues for each cluster were defined.

By utilizing the Foursquare API, we were able to select Mexican restaurants located in Tokyo and have a look at their locations and ratings.

This was achieved with following steps:

1 - Create a dataframe from csv file (a list of 23 Tokyo wards)
2 - Utilize Foursquare API to search for Mexican restaurants and create a new dataframe that contains the search results; sorting and filtering the results
3 - Cluster the Tokyo's 23 wards by their most popular venues using K-means
4 - Visualize and explore the clusters
5 - Explore the Mexican restaurants in Tokyo with the Foursquare API



**4: Results**

Clustering of Tokyo's 23 wards by most popular venue resulted in the following:
- Cluster 1: Cafe is the most popular venue type (central and historical areas Chiyoda, Meguro, Bunkyo)
- Cluster 2: Convenience store, discount store or fast food are the most popular venue types (suburbs like Adachi, Itabashi, Katsushika, Edogawa)
- Cluster 3: Japanese restaurant and Bar are the most popular venue types (business areas such as Minato, Chuo, Shibuya, Shinagawa, etc)
- Cluster 4: Convenience store or Ramen restaurant are the most popular venue types (suburbs with some percentage of small businesses: Koto, Ota, Setagaya etc)
- Cluster 5: contains only Shinjuku ward, the most popular venues in which are Korean restaurant, BBQ, Soba restaurant. Shinjuku is also the ward which will host the Olympic Games of 2020.

Exploring the Mexican restaurants resulted in the following:
- The wards that have 20-30 Mexican restaurants are: Adachi, Nakano, Taito, Sumida, Shinagawa, Shibuya. Excluding Adachi, these are all areas that we've labelled as "business" during clustering. Other business areas are Chuo, Minato, and Toshima, with corresponding number of Mexican restaurants 14, 11, and 8. Business areas in Japan have a large potential for dining venues, because office workers tend to go out for lunch or have a dinner with colleagues after work. So, we can recommend Chuo, Minato or Toshima wards to our client, because these are business areas with average or small number of competing Mexican venues.
- Wards that have small number of Mexican restaurants (6-7) are mostly suburbs such as Katsushika, Edogawa, Nerima, Itabashi etc. From our clustering, we've learned that most popular venues in these areas are convenience stores and grocery stores. Most likely, a new Mexican restaurant (a cuisine which is not so common for Japanese) won't be popular in these areas.
- There are only two newly opened or not so popular (considering absence of ratings) Mexican restaurants within the walking distance from New Olympic Stadium. Our client might consider opening a Mexican venue near the Stadium, which will welcome millions of guests during the 2020 Olympic Games.



**5: Discussion**

Business areas such as Chuo, Minato or Toshima, which accomodate lots of company offices, might sound like a good idea for starting a new dining venue. But at the same time, rent in these areas is also sky high. Opening a small restaurant might be a good option. Also, our client might consider other areas, which might not accomodate that many potential customers, but will be more cost-effective.
We've also figured out that it might be a good business opportunity to open a Mexican venue in walking distance from the Olympic Stadium. Because Olympic Games are quite a short-lived event, our client might consider not a fully established restaurant, but a Mexican food truck or a temporary cafe instead.



**6: Consclusion**

In conclusion, our client can consider the following options:
1 - A fully-established Mexican restaurant: business areas with small or average number of competitors: Chuo, Minato, Toshima
2 - Mexican food truck or temporary cafe: within the walking distance from 2020 Olympic Stadium, which will attract a lot of people during the Games. 
However, these results are not absolute and need further research. We might need to research the wards which our client is shoving interest in, or get more information on possible competitors.

