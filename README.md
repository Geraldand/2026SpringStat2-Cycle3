# Project Cycle 3: Two-Sample Inference

## Group Number (組別): 10

## Member Names (組員姓名)
* **112370234 張智源** (Geraldand)
* **113370201 簡愷毅** (kaibao8171)
* **113370218 彭鈺芳** (Vickyfang77)

## Research Details
* **Selected Research Question (選定的研究問題):** Is the proportion of current cigarette use different between students who felt sad or hopeless and those who did not? (Question 8)
* **Group Variable (群組變數):** `SadOrHopeless_Recoded` (1 = Felt sad or hopeless, 0 = Did not feel sad or hopeless)
* **Response Variable (反應變數):** `CurrentCigaretteUse_Recoded` (1 = Current user, 0 = Non-user)

## Methodology & Current Progress
* **Method Used (使用的統計方法):** Two-proportion z-test

### 📌 Current Status (目前進度)
* **Assumption Check (假設檢定):** ✅ **Passed!** We have verified the *Success/Failure Condition* via a contingency table. All 4 core cell counts are strictly greater than 10 (Minimum count is 1,064), confirming that the normal approximation is valid for our sample.
* **Preliminary Summary (初步數據摘要):**
  * Group 0 (Not Sad): $n_1 = 9,320$, Smokers = $1,508$ ($\hat{p}_1 \approx 16.18\%$)
  * Group 1 (Sad/Hopeless): $n_2 = 3,854$, Smokers = $1,064$ ($\hat{p}_2 \approx 27.61\%$)

## Short Final Conclusion (最終大結論)
本研究針對 2007 年 YRBS 數據（有效樣本共 13,174 筆）進行雙樣本比例 Z 檢定，得到以下最終結論：

1. **統計結果極度顯著**：檢定統計量 $Z = 15.0536$，$P$ 值趨近於 0（$3.27 \times 10^{-51} \ll 0.05$），我們**強烈拒絕虛無假設（Reject $H_0$）**。證實在美國青少年中，過去一年曾感到悲傷或絕望者的目前吸菸比例，**顯著高於**未感到悲傷或絕望者。
2. **實質差距巨大**：感到悲傷絕望青少年的吸菸率（27.61%）比對照組（16.18%）高出了 **11.43%**。我們有 95% 的信心母體真實比例差異落在 **9.83% 至 13.02%** 之間。由馬賽克圖與雙常態分佈圖可見，兩群體的行為模式存在實質性的巨大鴻溝（Practical Significance）。

*⚠️ 核心統計把關宣告：由於本研究採用的是觀察性研究資料（Observational Data），此處結果僅能證實青少年的「心理健康狀況（悲傷絕望）」與「吸菸行為」之間存在強烈的統計相關性（Association），絕不宣稱或推論其具備因果關係（Causality）。*

# Project Cycle 3: Two-Sample Inference (Group 10)

## Team Members
* **112370234 Geraldand** (張智源) - Project Management & Assumptions
* **113370201 kaibao8171** (簡愷毅) - Statistical Computing & Data
* **113370218 Vickyfang77** (彭鈺芳) - Data Visualization & Plotting

---

## 1. Research Framework & Variables
* **Research Question:** Is the proportion of current cigarette use different between students who felt sad or hopeless and those who did not? (YRBS 2007, Q8)
* **Group Variable (Explanatory):** `SadOrHopeless_Recoded` 
  * `1` = Felt sad or hopeless (Exposed Group)
  * `0` = Did not feel sad or hopeless (Comparison Group)
* **Response Variable:** `CurrentCigaretteUse_Recoded`
  * `1` = Current smoker (Smoked on 1 or more days in the past 30 days)
  * `0` = Non-smoker
* **Statistical Methodology:** Two-proportion Z-test

---

## 2. Statistical Assumption Verification (Passed ✅)
To validate the use of the Two-Proportion Z-test, the **Success/Failure Condition** was evaluated. The sampling distribution can be safely approximated by a normal distribution because the counts of successes and failures in both independent groups are strictly greater than 10:
* **Group 0 (Not Sad):** Failures = 7,812 ($\ge 10$), Successes = 1,508 ($\ge 10$)
* **Group 1 (Sad):** Failures = 2,790 ($\ge 10$), Successes = 1,064 ($\ge 10$)

---

## 3. Inferential Statistics Results
Based on our statistical execution on $N = 13,174$ valid observations:
* **Group 1 (Sad) Smoking Rate ($\hat{p}_1$):** 27.61% ($1,064 / 3,854$)
* **Group 2 (Not Sad) Smoking Rate ($\hat{p}_2$):** 16.18% ($1,508 / 9,320$)
* **Observed Sample Difference ($\hat{p}_1 - \hat{p}_2$):** 11.43%
* **Z-test Statistic:** 15.0536
* **P-value:** $3.27 \times 10^{-51}$ (Extremely significant, $P < 0.05$)
* **95% Confidence Interval (CI) for Difference:** [9.83%, 13.02%]

---

## 4. Final Substantive Conclusion
1. **Strong Statistical Evidence:** Since the P-value is effectively 0, we **strongly reject the null hypothesis ($H_0$)**. There is overwhelming evidence that American adolescents who experienced persistent sadness or hopelessness in 2007 had a significantly higher proportion of cigarette use than those who did not.
2. **Practical Significance:** The 11.43% gap represents a massive real-world disparity. We are 95% confident that in the true population, the smoking rate for distressed students is between 9.83% and 13.02% higher.
3. **Observational Study Disclaimer:** Because this analysis is based on survey data, this study establishes a robust **statistical association** between psychological distress and tobacco use, but **does not imply cross-sectional causality**.
