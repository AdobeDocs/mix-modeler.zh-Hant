---
title: 檢視目前的Mix Modeler發行說明
description: 最新 Mix Modeler 發行說明
feature-set: Experience Cloud
feature: Release Notes
exl-id: 38a47672-2af2-437c-b769-4d5febb941f5
source-git-commit: 0a5fdbe90c4a32de45f4f2756f080dc265f5fbb7
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 4%

---

# 目前的Mix Modeler發行說明

**上次更新日期**：2026年2月26日。

以下發行說明涵蓋最新版本的Mix Modeler。 Mix Modeler版本會在持續傳遞模式上運作，允許大約每月發行。 因此，這些發行說明會相應更新，因此請定期檢視。


## 2026 年 2 月

| 功能 | 說明 | [轉出開始](#release-strategy) | [全面發佈](#release-strategy) |
|---|---|---|---|
| **協調因子工作流程** | 因子現在作為[協調因子工作流程](/help/harmonize-data/overview.md#factors)的一部分來管理。 這簡化如何[定義因子資料](/help/ingest-data/schemas.md#factor-standard-fields-field-group)、如何[管理內部和外部因子作為資料集規則的一部分](/help/harmonize-data/dataset-rules.md#factor-datasets)，以及如何在[模型](/help/models/build.md#configure)中使用因子資料。 | 2026年2月25日 | 2026年2月25日 |
| **[!UICONTROL Granular incrementality reporting]** | 定義協調的欄位，以便您可以使用[精細分析報表欄位](/help/models/build.md#granular-insights-reporting-fields)在模型報表中深入研究，而不必建立個別模型。 | 2026年2月18日 | 2026年2月18日 |

## 2026 年 1 月

| 功能 | 說明 | [轉出開始](#release-strategy) | [全面發佈](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Dataset rules]** | [已更新資料集規則表格](/help/harmonize-data/dataset-rules.md)。 您可以搜尋一或多個資料集規則，並直接從表格檢視、編輯或刪除資料集規則。 | 2026年1月13日 | 2026年1月13日 |
| **[!UICONTROL Current spend]** | 在模型深入分析的[邊際回應曲線視覺效果](/help/models/insights.md#marginal-response-curves)中新增目前支出點。 | 2026年1月13日 | 2026年1月13日 |
| **[!UICONTROL Sort and resize columns]** | 已在[模型](/help/models/overview.md)和[計畫](/help/plans/overview.md)資料表中新增資料行的排序和調整大小。 | 2026年1月13日 | 2026年1月13日 |
| **修正** | 下列票證的修正： <ul><li>AMM-3328：因子的新運運算元停用欄位輸入</li><li>AMM-3359：日期選擇器和下拉式方塊鎖定。</li><li>AMM-3441：複製計畫不會自動填入日期範圍和預算。</li></ul> | 2026年1月13日 | 2026年1月13日 |


## 發行策略

[!UICONTROL Mix Modeler]使用功能旗標（也稱為「切換」）來控制新功能的可見性，以在完整版發行之前進行有限度的規模測試。 此發行策略包含下列階段：

* **有限測試**：分階段的發行從內部Adobe使用者的測試開始。 然後，一小群客戶帳戶即可使用這項功能，以確保該功能符合客戶需求和期望。

* **開始推出**：分階段發行從有限測試階段開始。 在隨後的幾個月內，該版本對客戶的可用性會從0%擴充至100%。 分階段推出會在Experience Cloud組織層級進行，因此組織中所有已獲授權的使用者都會獲得相同的體驗。
