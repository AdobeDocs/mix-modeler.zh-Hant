---
title: 評分資料
description: 瞭解如何在Mix Modeler中儲存模型的評分資料。
feature: Models
source-git-commit: 3596b83937b3f61ac453940f3a666d8aaf713679
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 7%

---


# 評分資料

作為對模型評分的一部分，評分資料會儲存在Experience Platform的資料集中。 此資料集符合為Mix Modeler例項中的每個模型建立的結構描述。

評分資料的結構描述命名為 `AMM AI Schema - <name of model> <id>`. 例如: `AMM AI Schema - Model for Online Conversion 10120`.

保留模型評分資料的資料集的命名如下 `AMM AI Aggregrate Scores - <id>`，例如 `AMM AI Aggregrate Scores - 10120`.


## 綱要

此結構描述包含一個欄位群組，其物件包含分數的詳細資訊。 物件包含下列欄位。

| 欄位名稱 | 類型 | 定義 |
|---|---|---|
| **campaignGroup** | 字串 | 行銷活動群組的名稱。 |
| **campaignName** | 字串 | 行銷活動的名稱。 |
| **貢獻** | 雙倍 | 歸因於指定接觸點之此轉換的貢獻。 |
| **conversionEndDate** | 日期 | 轉換期間的結束日期。 |
| **conversionName** | 字串 | 在轉換定義設定步驟中建立的轉換名稱。 |
| **conversionStartDate** | 日期 | 轉換視窗的開始日期。 |
| **地理** | 字串 | 轉換發生的地理位置。 |
| **mediaChannel** | 字串 | 在接觸點設定步驟中使用的管道名稱。 |
| **mediaSubChannel** | 字串 | 子管道的名稱。 |
| **收入** | 雙倍 | 歸因於指定接觸點之此轉換的收入。 |
| **scoreCreatedTime** | 日期時間 | 此分數記錄的建立時間。 |
| **接觸點結束日期** | 日期 | 接觸點視窗的結束日期。 |
| **接觸點名稱** | 字串 | 在接觸點定義設定步驟中建立的接觸點名稱。 目前，接觸點定義於媒體頻道上。 |
| **接觸點開始日期** | 日期 | 接觸點視窗的開始日期。 |

