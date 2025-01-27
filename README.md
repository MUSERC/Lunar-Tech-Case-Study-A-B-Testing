# Lunar-Tech-Case-Study-A-B-Testing
That is the A/B test for Lunar Tech Case Study from FreeCodeCamp 


A/B Testing Analysis with Click Data

This project demonstrates how to conduct A/B testing analysis using a dataset of user clicks. The analysis involves calculating statistical metrics such as standard error, Minimum Detectable Effect (MDE), Z-scores, and power, with the goal of determining whether a significant difference exists between control and experimental groups.

Dataset Link: https://www.kaggle.com/datasets/andrsulloa/lunar-tech-case-study-ab-testing/data

Dataset Information

The dataset contains the following columns:

user_id: Unique identifier for each user.

click: Binary value indicating whether the user clicked (1) or not (0).

group: Specifies whether the user belongs to the control ("con") or experimental ("exp") group.

timestamp: The timestamp when the user action was recorded (optional).

Dataset Summary:

Total entries: 20,000

Groups: Control and Experimental

Clicks: Recorded as binary values (0 or 1).

Analysis Steps

1. Data Preprocessing

Filtered the dataset to extract relevant columns: click and group.

Summarized the total clicks for both the control and experimental groups.

Calculated the total number of users in each group.

2. Probability Calculations

Calculated the probability of a click for each group:

Experimental Probability (prob_exp): Number of clicks in the experimental group divided by the total number of users in the experimental group.

Control Probability (prob_con): Number of clicks in the control group divided by the total number of users in the control group.

3. Statistical Metrics

Standard Error (SE):

Minimum Detectable Effect (MDE):

Z-Effect:

Z-Beta:

Power (1 - \beta):

4. Hypothesis Testing

Null Hypothesis (H0): There is no significant difference between the control and experimental groups.

Alternative Hypothesis (H1): There is a significant difference between the control and experimental groups.

Rejected H0 if the Z-Effect exceeded the critical Z-value (Z-Alpha).

Results

Standard Error (SE): 0.0063

Minimum Detectable Effect (MDE): 0.4127

Z-Effect: 65.51

Z-Alpha: 2.5758

Z-Beta: -62.93

Power: 1.0

Conclusion

The analysis shows that the Z-Effect (65.51) is much larger than the critical Z-value (2.5758). Therefore, we reject the null hypothesis and conclude that there is a significant difference between the control and experimental groups.



