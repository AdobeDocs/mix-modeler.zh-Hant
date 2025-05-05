---
title: Mix Modeler工作流程
description: 瞭解Mix Modeler的典型工作流程。
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: f12eea7454d1c81b347dc4960f5c491d81725f7d
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 1%

---

# Mix Modeler工作流程

請觀看這部影片，瞭解Mix Modeler的使用者工作流程簡介。

>[!VIDEO](https://video.tv.adobe.com/v/3440218/?learn=on&captions=chi_hant)


Mix Modeler中的典型工作流程包含下列活動：

![替代文字](/help/assets/ApplicationWorkflow.svg)

|  | 活動 | 說明 |
|---|---|---|
| ![資料](/help/assets/icons/Data.svg){width="100"} | [**擷取資料**](../ingest-data/overview.md) | 從Experience Platform(例如Adobe Analytics、Web SDK、其他來源)擷取事件資料、從行銷頻道擷取彙總資料（例如電視、圍牆花園、電子郵件、擁有和經營活動）、來自客戶的外部因素資料（例如訂閱服務的價格變更）和內部因素資料（例如假日計畫）。 |
| ![資料檢查](/help/assets/icons/DataCheck.svg){width="100"} | [**協調資料**](../harmonize-data/overview.md) | 設定對應規則和衝突解決規則，以合併在Mix Modeler中測量及規劃行銷活動績效所需的各種行銷資料集。 |
| ![檔案設定](/help/assets/icons/FileGear.svg){width="100"} | [**建置模型**](../models/overview.md) | 具有行銷接觸點（例如管道）、轉換定義以及內部和外部因素的組建模型例項。 |
| ![檔案資料](/help/assets/icons/FileData.svg){width="100"} | [**訓練與評分模型**](../models/overview.md) | 使用機器學習訓練和評分，建立彙總和事件層級分數。 |
| ![檔案圖表](/help/assets/icons/FileChart.svg){width="100"} | [**建置計畫**](../plans/overview.md) | 建立並建立計畫。 使用Mix Modeler模型的輸出，決定行銷資金的最佳配置，以實現業務目標。 |
| ![儀表板](/help/assets/icons/Dashboard.svg){width="100"} | [**總覽儀表板**](../dashboard/overview.md) | 使用各種可設定的視覺效果，深入瞭解協調的資料、模型和計畫。 |

{style="table-layout:auto"}

<!---
The detailed data-oriented flowchart below illustrates how:

* harmonized data is based on:

  * experience event data (originating from Analytics source connector, collected through Experience Platform SDKs and APIs, ingested through source connectors, or using streaming ingestion),
  * aggregate or summary data from walled gardens (like Facebook, YouTube), traffic sources, or offline advertising data, and 
  * definitions of harmonized fields and dataset rules.

* a model is based on:

  * the conversion and marketing touchpoint definitions resulting from the harmonized data and 
  * non-marketing aggregate or summary data containing internal or external factors.

* mult-touch attribution event scores can potentially be fed back into Experience Platform data lake for use in subsequent model configuration, training and scoring.

![Comprehensive workflow](/help/assets/comprehensive-workflow.svg)

-->
