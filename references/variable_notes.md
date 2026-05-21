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

### Assumption Evaluation & Interpretation

To safely conduct the Two-Proportion Z-test, the **Success/Failure Condition** must be met. This statistical rule requires that both independent groups have at least 10 observed successes and 10 observed failures ($n\hat{p} \ge 10$ and $n(1-\hat{p}) \ge 10$).

Based on our contingency table output above:
* **Group 0 (Students who did NOT feel sad/hopeless):**
  * Failures (Non-smokers): **7,812** ($\ge 10$) $\rightarrow$ *Passed!*
  * Successes (Current smokers): **1,508** ($\ge 10$) $\rightarrow$ *Passed!*
* **Group 1 (Students who FELT sad/hopeless):**
  * Failures (Non-smokers): **2,790** ($\ge 10$) $\rightarrow$ *Passed!*
  * Successes (Current smokers): **1,064** ($\ge 10$) $\rightarrow$ *Passed!*

**Conclusion for Assumption Check:**
Since all four core cell counts are significantly greater than the minimum threshold of 10, the Success/Failure condition is fully and robustly satisfied. Therefore, the sampling distribution of the difference between the two proportions ($\hat{p}_1 - \hat{p}_2$) can be safely approximated by a normal distribution, confirming that the **Two-Proportion Z-test is a valid and appropriate statistical method** for our dataset.
