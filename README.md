# Project Cycle 3: Two-Sample Inference

## 1. Group Number (組別)
* **Group 10**

## 2. Member Names (組員姓名)
* **112370234 張智源** (Geraldand)
* **113370201 簡愷毅** (kaibao8171)
* **113370218 彭鈺芳** (Vickyfang77)

## 3. Selected Research Question (選定的研究問題)
* Is the proportion of current cigarette use different between students who felt sad or hopeless and those who did not? (Question 8)

## 4. Group Variable and Response Variable (群組變數與反應變數)
* **Group Variable (Explanatory):** `SadOrHopeless_Recoded` (1 = Felt sad or hopeless, 0 = Did not feel sad or hopeless)
* **Response Variable:** `CurrentCigaretteUse_Recoded` (1 = Current cigarette user, 0 = Non-user)

## 5. Method Used (使用的統計方法)
* **Two-proportion z-test**

## 6. Short Final Conclusion (簡短大結論)
Based on our Two-Proportion Z-test on $N = 13,174$ students from the YRBS 2007 dataset, we found a highly statistically significant difference in cigarette use between the two groups ($Z = 15.0536$, $P = 3.27 \times 10^{-51} < 0.05$). 

We **strongly reject the null hypothesis ($H_0$)**. Students who felt sad or hopeless have a significantly higher smoking rate (**27.61%**) than those who did not (**16.18%**). **Visual evidence from our plots—specifically the completely non-overlapping 95% confidence intervals and the distinct separation of sampling distributions—further confirms that this 11.43% gap is robust and not due to chance.** We are 95% confident that the true population difference lies between **9.83% and 13.02%**.

*(Note: As this is an observational study, these results confirm a robust statistical association between adolescent psychological distress and tobacco use, but do not imply cross-sectional causality.)*

本研究針對 2007 年 YRBS 數據（有效樣本共 13,174 筆）進行雙樣本比例 Z 檢定，得到以下最終結論：
1. **統計結果極度顯著**：檢定統計量 $Z = 15.0536$，$P$ 值趨近於 0（$3.27 \times 10^{-51} \ll 0.05$），我們**強烈拒絕虛無假設（Reject $H_0$）**。證實在美國青少年中，過去一年曾感到悲傷或絕望者的目前吸菸比例，**顯著高於**未感到悲傷或絕望者。
2. **實質差距巨大**：感到悲傷絕望青少年的吸菸率（27.61%）比對照組（16.18%）高出了 **11.43%**。我們有 95% 的信心母體真實比例差異落在 **9.83% 至 13.02%** 之間。由馬賽克圖與雙常態分佈圖可見，兩群體的行為模式存在實質性的巨大鴻溝（Practical Significance）。

*⚠️ 核心統計把關宣告：由於本研究採用的是觀察性研究資料（Observational Data），此處結果僅能證實青少年的「心理健康狀況（悲傷絕望）」與「吸菸行為」之間存在強烈的統計相關性（Association），絕不宣稱或推論其具備因果關係（Causality）。*
