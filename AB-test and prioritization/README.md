# A/B-test and prioritization 

The data of a large online store is provided. It is necessary to prioritize the hypotheses provided by the marketing department to increase revenue, run an A/B test and analyze its results.

Data description:

- hypothesis.csv is a dataset that stores data about hypotheses. Contains a brief description of the hypothesis, the reach of users on a 10-point scale, the impact on users on a 10-point scale, and the cost of resources to test the hypothesis on a 10-point scale.
- orders.csv - stores data about orders of online store users. Contains the order ID, the user who made the order, the order date, the revenue from the order, and the test group that the order fell into.
- visitors - stores data about the visitors of the online store. Contains the date of the visit, the A/B test group, and the number of users on the specified date in the specified A/B test group.

Research Steps:

1. Data preprocessing
2. Prioritization of hypotheses using ICE and ICE frameworks, study of results and explanation of changes in prioritization
3. Analysis of A/B test results: plotting, calculation of percentiles and statistical significance. 

Conclusions: 

When prioritizing hypotheses, it was found that according to the ICE method, hypothesis 8 has the highest priority, offering to launch a promotion giving a discount on goods on the user's birthday, and according to the Rice method, hypothesis 7 has the highest priority - to add a subscription form to all the main pages in order to collect a customer base for email newsletters.

This difference in results is probably due to the fact that the ICE method does not take into account how many users will be affected by the change being made. The promotion, which gives a discount on the product on the user's birthday, will affect only a part of users - those who have indicated their date of birth, and will not affect all users at the same time. The subscription form on all the main pages will affect most of the users of the online store.

A/B test results.

During the calculations, it was found that:

according to raw data, there is no statistically significant difference in the average number of orders, after the removal of anomalies, no significant difference was also revealed;
there is a statistically significant difference in the average check between the groups both according to raw data and after filtering anomalies;
the graph of the difference in the average check varies greatly, probably due to anomalies. It does not allow us to draw significant conclusions, but it allowed us to identify the presence of anomalies.

The test can be stopped and recognized as successful. The conversion graph has come to stability, group B is statistically significantly better than group A.
