# Variable Coding and Assumptions

## 1. Group Definition (Explanatory Variable)
* **Original Variable:** `q23` (During the past 12 months, did you ever feel so sad or hopeless...)
* **Recoded Variable:** `SadOrHopeless`
* **Logic:** 
  * Code 1 (Yes) -> Recoded as 1 (Success / Exposed group)
  * Code 2 (No) -> Recoded as 0 (Failure / Comparison group)
  * Missing or invalid responses were dropped.

## 2. Response Variable Definition
* **Original Variable:** `q28` (During the past 30 days, on how many days did you smoke cigarettes?)
* **Recoded Variable:** `CurrentCigaretteUse`
* **Logic:**
  * Codes 2-7 (Smoked on 1 or more days) -> Recoded as 1 (Success / Yes)
  * Code 1 (0 days) -> Recoded as 0 (Failure / No)
  * Missing or invalid responses were dropped.

## 3. Method Choice
We chose the **Two-proportion z-test** because both our group variable and response variable are binary categorical variables. We are comparing the proportion of successes (current cigarette use) between two independent groups.

### Assumption Check Evaluation
To use the Two-Proportion Z-test, the Success/Failure Condition must be met for both groups. This requires that the number of successes and failures in each group is at least 10:
- Group 0 (No Sad/Hopeless Feeling): Successes (Smoke) = 1,508, Failures (No Smoke) = 7,812
- Group 1 (Sad/Hopeless Feeling): Successes (Smoke) = 1,064, Failures (No Smoke) = 2,790

Since all four cell counts from our contingency table are strictly greater than 10 ($n\hat{p} \ge 10$ and $n(1-\hat{p}) \ge 10$), the Success/Failure Condition is fully satisfied. The sampling distribution of the difference between the two proportions can be safely approximated by a normal distribution, making the Two-Proportion Z-test valid for this analysis.
