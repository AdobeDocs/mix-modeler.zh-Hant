---
title: Mix Modeler工作流程
description: 瞭解Mix Modeler的典型工作流程。
feature: Ingest Data, Plans, Harmonized Data, Models
source-git-commit: 08cfd4239f6bcaf885565f3ae04cbd51869e8c00
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 3%

---


# Mix Modeler工作流程

Mix Modeler中的典型工作流程如下所示：

![替代文字](../assets/ApplicationWorkflow.svg)

|  | 活動 | 說明 |
|---|---|---|
| ![資料](../assets/icons/Data.svg){width="100"} | [**擷取資料**](../ingest-data/overview.md) | 從Adobe Experience Platform (例如Adobe Analytics、Web SDK、其他來源)擷取事件資料、來自行銷管道的彙總資料（例如電視、圍牆花園、電子郵件、擁有和經營活動）以及來自客戶的外部因素資料（例如訂閱服務的價格變更）。 |
| ![資料檢查](../assets/icons/DataCheck.svg){width="100"} | [**協調資料**](../harmonize-data/overview.md) | 設定對應規則和衝突解決規則，以合併在Mix Modeler中測量及規劃行銷活動績效所需的各種行銷資料集。 |
| ![FileConfig](../assets/icons/FileGear.svg){width="100"} | [**設定模型**](../models/create.md) | 使用行銷接觸點（例如管道）和轉換定義設定模型執行個體。 |
| ![檔案資料](../assets/icons/FileData.svg){width="100"} | [**訓練模型並為其評分**](../models/overview.md) | 使用機器學習訓練和評分，建立彙總和事件層級分數。 |
| ![檔案圖表](../assets/icons/FileChart.svg){width="100"} | [**建立計畫**](../plans/overview.md) | 使用Mix Modeler模型的輸出，決定行銷資金的最佳配置，以實現業務目標。 |
| ![控制面板](../assets/icons/Dashboard.svg){width="100"} | [**總覽儀表板**](../dashboard/overview.md) | 使用各種可設定的Widget，深入瞭解協調的資料、模型和計畫。 |

{style="table-layout:auto"}

