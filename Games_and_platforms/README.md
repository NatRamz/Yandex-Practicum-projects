# Games and platforms
Historical data on game sales, user and expert ratings, genres and platforms (for example, Xbox or PlayStation) were presented from open sources. I have identified patterns that determine the success of the game. This will allow you to bet on a potentially popular product and plan advertising campaigns.
Data up to 2016 are presented.
The data set contains the abbreviation ESRB (Entertainment Software Rating Board), an association that determines the age rating of computer games. ESRB evaluates game content and assigns it a suitable age category, for example, "For adults", "For younger children" or "For teenagers".

Research Steps:

1. Data preprocessing
2. Calculation of total sales by region
3. Study of the number of games released in different years
4. Studying sales changes across platforms
5. Creating a slice of current data
6. Study the leading sales platforms and search for potentially profitable platforms 
7. Construction of box lots for global sales of games by platform
8. Evaluation of the impact on sales of user reviews and critics, calculation of the correlation between reviews and sales
9. Study of the general distribution of games by genre.
10. Drawing up a portrait of the user of each region: the most popular platforms, genres.
11. Study of the impact of the ESRB rating on sales in certain regions
12. Testing hypotheses about the average user ratings of platforms and genres. 

Conclusions:

In this project, I researched historical data on game sales, user and critic ratings, genres and gaming platforms. The purpose of the study is to identify patterns that determine the success of the game in order to bet on a potentially popular product in 2017 and plan advertising campaigns.

In the first and second steps, I opened the dataframe and prepared the data for the study: reduced the column names to lowercase, converted the data into the necessary types, processed the omissions. In some columns - user_score, critic_score and rating, it was impossible to assume a logical replacement, besides, in the future, statistical analysis should be carried out on the basis of these data, and filling with synthetic data would distort statistics. The nature of the omissions in the columns with ratings from critics and players may be explained by the low popularity of some games: they simply did not receive enough ratings to assign a rating. In the case of the ESRB rating, it can be assumed that not all games were submitted for assignment of this rating.

In the third step, during the research data analysis, data for the entire period, for the period from 2010 to 2016, were analyzed separately for the platforms. The number of games released has increased significantly over the years. Most of the games were released from 2006 to 2011. PS2(1233), PS3(931), X360(961), DS(802) and Wii(891) have the largest total sales for the entire period. The average "lifetime" of the platform is 7-10 years. For further analysis, a separate dataframe with data from 2010 to 2016 was allocated to create a forecast for 2017. In the relevant sample, the most popular gaming platform was PS3(587), X360(550) was in second place, PS4 (314) was third, 3DS (257) was fourth, and Wii (222) was fifth. The most promising and growing platforms, as can be seen on the charts, are PS4 and 3DS. For all platforms on boxplots, average sales are no more than 5 million copies of the game. The relationship between reviews from players and critics and the overall sales of the game was also studied. The most promising platforms were selected for study: PS4 and 3DS. According to the scatter plot and the Pearson correlation coefficient, ratings from players do not have a big impact on game sales, but in general, the relationship between higher game sales and higher ratings from players is visible. While the ratings from critics have a significant impact on sales: the better the critics' ratings, the higher the sales of the game. According to median values, the most profitable genre of games is shooter, platform is in second place, sports is in third. Strategy, puzzle and adventure have the lowest sales.

At the fourth step, a portrait of the user of each region was compiled. The study examined the most popular platforms and genres of games in certain regions. The average user from North America likes to play action games on their X360. The average user from Japan prefers role-playing games on the DS platform. The average user from Europe plays action games on PS2. The relationship between the age rating of the game and its sales was confirmed: for example, in all regions, except Japanese, the most popular rating is E - for everyone, for all ages. Most of the games actively sold in Japan do not have an ESRB rating, because the Japanese market is isolated and games created for the Japanese market were not submitted for assignment of the European age rating.

At the fifth step , two hypotheses were tested: "The average user ratings of the Xbox one and PC platforms are the same" and "The average user ratings of the Action and Sports genres are different. Calculations have shown that the first null hypothesis is correct, the average user ratings for the Xbox One and PC platforms do not differ. The second hypothesis was rejected: the average user ratings of games of the Action and Sports genres do not differ.
