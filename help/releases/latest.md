---
title: 檢視目前的Mix Modeler發行說明
description: 最新 Mix Modeler 發行說明
feature-set: Experience Cloud
feature: Release Notes
exl-id: 38a47672-2af2-437c-b769-4d5febb941f5
source-git-commit: 6fe334458e8d7fabbd7cbaa027e13eadbf703325
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 4%

---

# 目前的Mix Modeler發行說明

**上次更新日期**：2025年9月12日。

以下發行說明涵蓋最新版本的Mix Modeler。 Mix Modeler版本會在持續傳遞模式上運作，允許大約每月發行。 因此，這些發行說明會相應更新，因此請定期檢視。


## 2025 年 9 月

| 功能 | 說明 | [轉出開始](#release-strategy) | [全面發佈](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Dataset mapping validations]** | 已新增驗證至和諧欄位的Experience Platform資料集對應。 | 2025年9月9日 | 2025年9月9日 |
| **[!UICONTROL Context menu on links to model and plans]** | 啟用模型及計畫連結的瀏覽器內容功能表。 您現在可以使用該瀏覽器前後關聯功能表，在新的標籤或視窗中開啟特定計畫或模型。 | 2025年9月9日 | 2025年9月9日 |
| **修正** | 下列票證的修正： <ul><li>AMM-3101：修正為規則建立的不正確對應： `event_date`已傳遞為欄位名稱而非`timestamp`。</li><li>AMM-3092：修正無法變更重複預算型計畫的管道最大限制值。</li><li>AM3130：修正模型詳細資訊快顯視窗中的錯誤&#x200B;**[!UICONTROL Run frequency]**&#x200B;資訊。</li><li>AMM3158：已更新&#x200B;**[!UICONTROL Select target metric]**&#x200B;選項的標籤，這些選項是&#x200B;**[!UICONTROL Optimize]**&#x200B;計畫建立[介面中](/help/plans/build.md)窗格的一部分。</li><li>AMM 3176：修正無法在[的](/help/models/insights.md#breakdown)索引標籤中檢視&#x200B;**[!UICONTROL Attribution]**&#x200B;依管道&#x200B;**[!UICONTROL Model Insights]**&#x200B;劃分的視覺效果。</li></ul> | 2025年9月9日 | 2025年9月9日 |
| **修正** | 下列票證的修正： <ul><li>AMM-3174：改善沒有現有計畫可用的體驗。</li><li>AMM-3216：增強自訂日期範圍的驗證。</li><li>AMM-3240：固定執行模型頻率顯示。</ul> | 2025年9月23日 | 2025年9月23日 |


## 2025 年 7 - 8 月

| 功能 | 說明 | [轉出開始](#release-strategy) | [全面發佈](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Compare plans update]** | [比較計畫](/help/plans/compare.md) UI現在會顯示付費行銷的其他詳細資料：ROI或CPA以及收入。 | 2025年8月20日 | 2025年8月20日 |
| **協調更新** | 所有資料集規則現在都會使用類似的[一般對應到協調欄位體驗](/help/harmonize-data/dataset-rules.md)，無論資料集型別為何。 當您從摘要資料集對應標準協調欄位時，Mix Modeler會嘗試自動推斷對應的Experience Platform資料集欄位。 | 2025年7月29日 | 2025年7月29日 |


## 2025年5月至6月

| 功能 | 說明 | [轉出開始](#release-strategy) | [全面發佈](#release-strategy) |
|---|---|---|---|
| **目標型計畫** | 在預算旁邊，您可以在您[建立](/help/plans/build.md)或[編輯](/help/plans/insights.md#edit-plan)計畫時定義目標（目標）。 目標量度的範例包括收入、轉換、CPA或ROI。 | 2025年6月18日 | 2025年7月8日 |
| **支出模式設定** | 當您建立計畫時，您現在可以選擇在定義每個預算日期範圍的支出模式時使用[歷史參考](/help/plans/build.md)資料（例如過去行銷支出資料和深入分析）。 | 2025年5月14日 | 2025年5月14日 |
| **進階計畫組態** | 您可以為計畫定義[進階設定](/help/plans/build.md)，例如每次轉換的平均收入和管道成本。 | 2025年5月14日 | 2025年5月14日 |

## 2025年3月至4月

| 功能 | 說明 | [轉出開始](#release-strategy) | [全面發佈](#release-strategy) |
|---|---|---|---|
| **模型漂移偵測** | 開啟模型時，系統會在偵測到模型漂移時[提示您重新訓練模型](/help/models/insights.md#model-drift)。 | 2025年4月3日 | 2025 年 5 月 7 日 |
| **計畫深入分析中的邊際管道回訪** | 將[邊際管道回訪](/help/plans/insights.md#marginal-channel-return)視覺效果新增到計畫深入分析中，其中顯示所有或選取管道的邊際收支平衡與計畫回訪。 | 2025年4月3日 | 2025年4月24日 |


## 2025年1月至2月

| 功能 | 說明 | [轉出開始](#release-strategy) | [全面發佈](#release-strategy) |
|---|---|---|---|
| **巢狀條件** | 當您定義合格的資料母體作為模型[的](/help/models/build.md#configure)組態的一部分時，可以使用AND和OR來建立巢狀條件。 | 2025年1月15日 | 2025年2月18日 |
| **檢視報告** | 您可以檢視有關您定義為協調資料一部分的[轉換](/help/harmonize-data/conversions.md#view-report)或[行銷接觸點](/help/harmonize-data/marketing-touchpoints.md#view-report)的報告。 | 2025年1月15日 | 2025年2月18日 |
| **刪除確認** | 系統會提示您確認刪除[計畫](/help/plans/overview.md#delete-plans)或[模型](/help/models/overview.md#delete-models)。 | 2025年1月15日 | 2025年2月18日 |
| **因素UI改善** | 您可以選取要在模型深入分析中顯示的[因素](/help/models/insights.md#factors-beta)。 | 2025年1月15日 | 2025年2月18日 |
| **錯誤處理** | 使用者易記的錯誤訊息，以及改善使用者在資料協調與計畫中的錯誤情境體驗。 | 2025年2月18日 | 2025年2月18日 |
| **模型狀態** | 重新定義整個模型生命週期中的[模型狀態](/help/models/overview.md#manage-models)。 | 2025年2月18日 | 2025年2月18日 |


## 發行策略

[!UICONTROL Mix Modeler]使用功能旗標（也稱為「切換」）來控制新功能的可見性，以在完整版發行之前進行有限度的規模測試。 此發行策略包含下列階段：

* **有限測試**：分階段的發行從內部Adobe使用者的測試開始。 然後，一小群客戶帳戶即可使用這項功能，以確保該功能符合客戶需求和期望。

* **開始推出**：分階段發行從有限測試階段開始。 在隨後的幾個月內，該版本對客戶的可用性會從0%擴充至100%。 分階段推出會在Experience Cloud組織層級進行，因此組織中所有已獲授權的使用者都會獲得相同的體驗。
