---
title: Mix Modeler工作流程
description: 瞭解Mix Modeler的典型工作流程。
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Mix Modeler工作流程

請觀看這部影片，瞭解Mix Modeler的使用者工作流程簡介。

>[!VIDEO](https://video.tv.adobe.com/v/3424854/?learn=on)


Mix Modeler中的典型工作流程包含下列活動：

![替代文字](/help/assets//ApplicationWorkflow.svg)

|  | 活動 | 說明 |
|---|---|---|
| ![資料](/help/assets//icons/Data.svg){width="100"} | [**擷取資料**](../ingest-data/overview.md) | 從Experience Platform(例如Adobe Analytics、Web SDK、其他來源)擷取事件資料、從行銷頻道擷取的彙總資料（例如電視、圍牆花園、電子郵件、擁有和經營的活動）、來自客戶的外部因素資料（例如訂閱服務的價格變更）和內部因素資料（例如假日計畫）。 |
| ![資料檢查](/help/assets//icons/DataCheck.svg){width="100"} | [**協調資料**](../harmonize-data/overview.md) | 設定對應規則和衝突解決規則，以合併在Mix Modeler中測量及規劃行銷活動績效所需的各種行銷資料集。 |
| ![檔案設定](/help/assets//icons/FileGear.svg){width="100"} | [**設定模型**](../models/create.md) | 使用行銷接觸點（例如管道）、轉換定義以及內部和外部因素來設定模型執行個體。 |
| ![檔案資料](/help/assets//icons/FileData.svg){width="100"} | [**訓練與評分模型**](../models/overview.md) | 使用機器學習訓練和評分，建立彙總和事件層級分數。 |
| ![檔案圖表](/help/assets//icons/FileChart.svg){width="100"} | [**建立計畫**](../plans/overview.md) | 使用Mix Modeler模型的輸出，決定行銷資金的最佳配置，以實現業務目標。 |
| ![儀表板](/help/assets//icons/Dashboard.svg){width="100"} | [**總覽儀表板**](../dashboard/overview.md) | 使用各種可設定的Widget，深入瞭解協調的資料、模型和計畫。 |

{style="table-layout:auto"}

以下以資料為導向的詳細流程圖會說明如何：

* 協調的資料是根據：

   * 體驗事件資料(源自Analytics來源聯結器、透過Experience PlatformSDK和API收集、透過來源聯結器擷取，或使用串流擷取)，
   * 從封閉花園(例如Facebook、YouTube)、流量來源或離線廣告資料彙總或摘要資料，以及
   * 協調欄位和資料集規則的定義。

* 模型建立在：

   * 根據協調資料和行銷活動產生的轉換和行銷接觸點定義
   * 包含內部或外部因素的非行銷彙總或摘要資料。

* 多接觸點歸因事件分數可能會傳回Experience Platform資料湖，以供後續的模型設定、訓練和評分使用。

![完整的工作流程](/help/assets//comprehensive-workflow.svg)
