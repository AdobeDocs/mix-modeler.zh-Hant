---
title: Mix Modeler工作流程
description: 瞭解Mix Modeler的典型工作流程。
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
TQID: https://experienceleague.adobe.com/PAKsHAqpIeBVCJGIPS2ZqWw-vVpS9LUpYdJRFKP0ynY
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
feature_v2:
  - id: e0abf868-dae2-4c1c-83e9-b21799232845
  - id: fbd94e4b-f9b8-42a4-8df5-3f917aabae24
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
  - id: d822825b-9821-40d5-9b0d-42a9e3f317c5
subfeature_v2:
  - id: ad7101f7-ae92-401b-a25a-d3060d42989d
  - id: a4dc3e7d-bd07-4ac8-8e49-ff2e8fecf1e7
  - id: ee1bf083-e090-4def-936b-c111d29f42d0
  - id: d1167c89-f64a-42ca-ac95-1d91b7790df2
  - id: bc2f5225-03d4-4bc8-89ec-99d78c30e6dd
  - id: d4b8ba18-64c1-4413-be54-74405ec7f558
  - id: ba4fd72c-282e-4fb6-abc1-08e6fb87b2ad
  - id: b4655f7e-1a6e-4fa3-a7c5-3c34d4786e49
  - id: b2d4aeb9-eabe-49f6-8edb-bb2862d5980b
  - id: c89e26b6-808d-4500-8b01-450a63466999
  - id: a9505d76-24a1-4ffe-bd01-6ac32d5af453
  - id: cb40363e-1205-4921-971c-9ee6bdb18329
  - id: d7b067e6-4f39-41e9-a081-7650346a84cd
  - id: b2520ae7-8f6c-4952-935e-aacc2c10256f
  - id: e6c284e0-b6e6-4f82-bf96-e96bb5157b90
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
autotag-review: '2026-05-01T09:15:33.908Z'
source-git-commit: 5579087b9381c4d8e909ed5fe3099fd42d5c6799
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 1%

---

# Mix Modeler工作流程

請觀看這部影片，瞭解Mix Modeler的使用者工作流程簡介。

>[!VIDEO](https://video.tv.adobe.com/v/3440218/?captions=chi_hant&learn=on)


Mix Modeler中的典型工作流程包含下列活動：

![替代文字](/help/assets/ApplicationWorkflow.svg)

|  | 活動 | 說明 |
|---|---|---|
| ![資料](/help/assets/icons/Data.svg){width="100"} | [**擷取資料**](../ingest-data/overview.md) | 從Experience Platform （例如Adobe Analytics、Web SDK、其他來源）擷取事件資料、從行銷頻道擷取的彙總資料（例如電視、圍牆花園、電子郵件、擁有和經營活動）、來自客戶的外部因素資料（例如訂閱服務的價格變更）和內部因素資料（例如假日計畫）。 |
| ![資料檢查](/help/assets/icons/DataCheck.svg){width="100"} | [**協調資料**](../harmonize-data/overview.md) | 設定對應規則和衝突解決規則，以合併Mix Modeler中測量及規劃行銷活動績效所需的各種行銷資料集。 |
| ![檔案設定](/help/assets/icons/FileGear.svg){width="100"} | [**建置模型**](../models/overview.md) | 具有行銷接觸點（例如管道）、轉換定義以及內部和外部因素的組建模型例項。 |
| ![檔案資料](/help/assets/icons/FileData.svg){width="100"} | [**訓練與評分模型**](../models/overview.md) | 使用機器學習訓練和評分，建立彙總和事件層級分數。 |
| ![檔案圖表](/help/assets/icons/FileChart.svg){width="100"} | [**建置計畫**](../plans/overview.md) | 建立並建立計畫。 使用Mix Modeler模型的輸出，決定行銷資金的最佳配置，以實現業務目標。 |
| ![儀表板](/help/assets/icons/Dashboard.svg){width="100"} | [**總覽儀表板**](../dashboard/overview.md) | 使用各種可設定的視覺效果，深入瞭解協調的資料、模型和計畫。 |

{style="table-layout:auto"}

以下說明輸入資料如何流入Mix Modeler以及Mix Modeler如何為其自己的介面以及其他解決方案（如Customer Journey Analytics）產生輸出資料的概觀。

![Mix Modeler輸入輸出資料流程](../assets/mm-input-output.png)

<!--
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
