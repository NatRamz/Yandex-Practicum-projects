# A/A/B-test and analysis

The data of a startup that sells food is provided. It is necessary to study the behavior of users of the mobile application, the sales funnel and the results of the A/A/B experiment.

## Data description:
- eventName - event name
- Device ID HAsh - unique user ID
- Event TimeStamp - time of the event
- ExpID - experiment number: 246 and 247 - control groups, 248 - experimental.

## Action plan:
- Explore the sales funnel
- To investigate the results of the A/A/B experiment.

## Conclusions 

During the verification and examination of the data, it was found that the data up to August 1, 2019 is incomplete and contains very few records. Therefore, it was decided to drop the records until 1.08.2019.

As a result, about 1% of the data was deleted, the losses were insignificant, while the distribution of the number of records by day was normalized.

The funnel of events looks like this:

- The user opens the application, gets to the main screen, the MainScreenAppear event is marked.
- After the user views the offers for purchase, the OffersScreenAppear event is marked.
- The user adds what he liked to the cart and opens it - this is the CartScreenAppear event.
- And finally, PaymentScreenSuccessful is flagged when the user has paid for the purchase.
98% of users get to the first stage. Perhaps this is due to the fact that the user has the opportunity to go directly to the catalog through the push notification of the application or a link in the email newsletter. Therefore, not all users start their journey from the first step.

The biggest loss of users occurs at the stage of transition from the first step to the second - only 61% of users go to the second step, then 81% of users go to the third step, and 94% go to the fourth. In total, 47.7% of the users who got to the first step reach the fourth step.

The A/A test showed that there are no statistically significant differences in the proportions between transitions from all steps: the division into groups works correctly.

The A/B test showed that in the end, in comparison with both control groups and with the combined control group, the test group showed no significant differences.

When checking conclusions with a reduced level of statistical significance of 0.003125, there is no statistically significant difference.

The A/A/B test can be stopped, and it is recognized that the test group did not show higher results.
