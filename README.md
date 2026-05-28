# Project Cycle 3: Two-Sample Inference / 雙樣本推論

## 1. Group Number / 小組編號
* Group 10

## 2. Member Names / 組員姓名
* **112370234 張智源** (Geraldand)
* **113370201 簡愷毅** (kaibao8171)
* **113370218 彭鈺芳** (Vickyfang77)

## 3. Selected Research Question / 選定的研究問題
* Is the proportion of current cigarette use different between students who felt sad or hopeless and those who did not? (Question 8)
* 過去一年曾感到悲傷或絕望之青少年與未感到者，其目前吸菸比例是否有所不同？（題目 8）

## 4. Group Variable and Response Variable / 群組變數與反應變數
* **Primary Group Variable (Explanatory) / 主要群組變數（自變數）:**
  * `SadOrHopeless_Recoded` (1 = Felt sad or hopeless / 曾感到悲傷或絕望, 0 = Did not feel sad or hopeless / 未感到悲傷或絕望)
* **Primary Response Variable / 主要反應變數（應變數）:**
  * `CurrentCigaretteUse_Recoded` (1 = Current cigarette user / 目前有吸菸, 0 = Non-user / 無吸菸)
* **Additional Exploratory Variables / 延伸探索變數:**
  * `CurrentBingeDrinking5OrMore_Recoded` (1 = Binge drinker / 有狂飲行為, 0 = Non-binge drinker / 無狂飲行為)
  * `CurrentAlcoholUse_Recoded` (1 = Current alcohol user / 目前有飲酒, 0 = Non-user / 無飲酒)

## 5. Method Used / 使用的統計方法
* **Two-proportion z-test / 雙樣本比例 Z 檢定**

## 6. Short Final Conclusion / 簡短最終結論

Based on our Two-Proportion Z-test on $N = 13,174$ students from the YRBS 2007 dataset, we found a highly statistically significant difference in cigarette use between the two groups ($Z = 15.0536$, $P = 3.27 \times 10^{-51} \ll 0.05$). We strongly reject the null hypothesis ($H_0$). Students who felt sad or hopeless have a significantly higher smoking rate (**27.61%**) than those who did not (**16.18%**). We are 95% confident that the true population difference lies between **9.83% and 13.02%** (a net difference of 11.43%). Visual evidence from our sampling distribution model confirms that this gap is robust and shows zero overlap along the estimation axis.

Furthermore, our exploratory analysis incorporating "Binge Drinking" reveals a clear risk escalator effect. While the normal baseline group has a low smoking rate, the comorbidity group (students experiencing both sadness and binge drinking) exhibits a smoking rate that skyrockets to **54.8%**. Additionally, an anatomical breakdown of the student smoking population reveals that pure smokers account for only 20.1%, meaning that **79.9%** of adolescent smokers carry invisible burdens of psychological distress or alcohol abuse. These behaviors serve as a critical "beacon" reflecting underlying psychological trauma rather than mere disciplinary issues.

*Statistical Disclaimer: As this is an observational study, these results confirm a robust statistical association between adolescent psychological distress, substance abuse, and tobacco use, but do not imply causality.*

---

本研究針對 2007 年 YRBS 數據（有效樣本共 13,174 筆）進行雙樣本比例 Z 檢定與資料探索，得到以下最終結論：

1. **統計與實質顯著性：** 檢定統計量 $Z = 15.0536$，$P$ 值趨近於 0（ $3.27 \times 10^{-51} \ll 0.05$ ），我們強烈拒絕虛無假設（Reject $H_0$）。過去一年曾感到悲傷或絕望之青少年的目前吸菸比例（27.61%）顯著高於未感到悲傷或絕望者（16.18%）。我們有 95% 的信心母體真實比例差異落在 9.83% 至 13.02% 之間（淨差異為 11.43%）。由抽樣分配模型圖可見，兩群體的估計分佈曲線完全分離且零重疊，證實此差距存在實質性的巨大鴻溝。
2. **多重風險疊加與隱形負擔（結合延伸變數之深度探索）：** 透過納入「狂飲（Binge Drinking）」進行交叉探索，發現學生的吸菸風險呈現明顯的「風險階梯式上升」。相較於雙無因子的基線群體，同時面臨悲傷情緒與狂飲行為的「高度共病群體」，其吸菸率急遽飆升至 **54.8%**。進一步解剖吸菸人口結構發現，純粹吸菸者僅佔 20.1%，意即高達 **79.9%** 的吸菸青少年皆背負著悲傷情緒或酒精濫用的隱形重擔。此類偏差行為在實質上扮演了心理健康受創的「雷達信標」，而非單純的紀律問題。

*核心統計把關宣告：由於本研究採用的是觀察性研究資料（Observational Data），此處結果僅能證實青少年的「心理健康狀況（悲傷絕望）」、「物質濫用（飲酒狂飲）」與「吸菸行為」之間存在強烈的統計相關性（Association），絕不宣稱或推論其具備因果關係（Causality）。*
