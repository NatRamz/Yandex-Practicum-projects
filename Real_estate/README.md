# Real_estate project
At my disposal were provided the data of the Yandex Real Estate service — an archive of ads for several years about the sale of apartments in St. Petersburg and neighboring settlements.
I preprocessed the data and studied them to find interesting features and dependencies that exist in the real estate market.
The database contains two types of data about each apartment: user-added and cartographic. For example, the first type includes the area of the apartment, its floor and the number of balconies, the second — the distance to the city center, the airport and the nearest park.

## Research Steps:

1. Data preprocessing
2. Research data analysis: determination of normal parameters of apartments.
3. Study of the average sale rate of an apartment.
4. Study of the factors that most strongly affect the value of the property.
5. Calculation of the average price per square meter in 10 localities with the largest number of ads
6. Calculation of the average price of one kilometer from the city center in St. Petersburg

## Conclusions:

In this project, I researched and analyzed a dataframe with real estate data in various localities. During the study, a number of important dependencies were identified.

At the first stage, during preprocessing, gaps were filled in where it was possible to assume a replacement, abnormal values that distort the accuracy of the data were removed, and implicit duplicates were eliminated. When collecting data in the future, for greater accuracy, it is desirable to pay attention to data on the distance to the nearest parks, city centers and reservoirs. There are gaps in many columns here, and it is impossible to assume a logical replacement.

At the second stage, new columns were added that are important for further calculations: the price of one square meter of real estate, the date and day of the week of publication of the announcement, the type of floor of the apartment and the distance to the city center in kilometers.

At the third stage, all the parameters of the objects were studied. Histograms confirm the correctness of the preprocessing, showing normal scattering where it is logical. Most of the apartments have an area of up to 100 square meters, a living area of less than 50 and a kitchen area of less than 20 square meters. In the histogram of the kitchen area, there is a peak of about 0: this is due to the fact that there is no dedicated kitchen in studio apartments, so its area is indicated as 0. In most apartments there are 1 or 2 rooms. Most of the apartments are located from the 1st to the 5th floor, there is also an extensive group of apartments from 5 to 9. There are few apartments located higher than on the 9th floor. Most often, the apartments are not located on the first or last floors. Most of the apartments are located within 20 kilometers from the city center, 40 kilometers from the airport and a kilometer from parks. Most often, ads are published on weekdays, in spring and autumn.

At the fourth stage, the speed of the sale of the apartment was studied. The arithmetic mean and median values differ almost twice. Sales in 40 days or less can be considered unusually fast, and sales longer than 200 days can be considered unusually long. It is also noted that the speed of sales has increased significantly since 2014.

At the fifth stage, the factors that most strongly affect the cost of the object were studied. In general, we can say that the larger the property, the higher its price. The larger the total area, living area and kitchen, the number of rooms, the more expensive the property is sold. The day of the week and the month do not affect the final cost, but it depends on the year of publication: prices showed a decrease by 2016, followed by a rise to the previous level. The number of ads increased by 2017 and then began to decline again.

At the sixth stage, prices per square meter of real estate in 10 settlements with the most published ads were studied. It was found that among the 10 cities with the largest number of ads, St. Petersburg has the highest cost per square meter - 107,528 rubles, and Vyborg has the lowest, 58,583 rubles.

At the seventh stage, the cost of one kilometer in distance to the city center in St. Petersburg was investigated. It amounted to 5,350,000 rubles: this has a very big impact on the final cost. The strange behavior of the graph at 27 kilometers from the city center was also studied: it was due to the fact that there were only 2 ads for the sale of apartments in this place.
