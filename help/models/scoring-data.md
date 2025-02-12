---
title: 使用評分資料
description: 瞭解如何在Mix Modeler中儲存模型的評分資料。
feature: Models
exl-id: 2f2c3d20-7b14-41cc-a11a-03e8ad9e5d7a
source-git-commit: 5f6c35816a8850bf170cb73d9710e65809e5f372
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 6%

---

# 使用評分資料

作為對模型評分的一部分，評分資料會儲存在Experience Platform的資料集中。 當您在建立模型期間啟用多接觸式歸因時，其他事件分數資料會儲存在Experience Platform的資料集中。

這些資料集都符合結構描述。 本文會記錄這些結構描述。


## 彙總評分資料結構描述

評分資料的結構描述名稱為`AMM AI Schema - <name of model> <id>`。 例如： `AMM AI Schema - Model for Online Conversion 10120`。

保留模型評分資料的資料集命名為`AMM AI Aggregrate Scores - <id>`，例如`AMM AI Aggregrate Scores - 10120`。

此結構描述包含一個欄位群組，其物件包含分數的詳細資訊。 物件包含下列欄位。

| 欄位名稱 | 類型 | 定義 |
|---|---|---|
| `campaignGroup` | 字串 | 行銷活動群組的名稱。 |
| `campaignName` | 字串 | 行銷活動的名稱。 |
| `contribution` | 兩次 | 歸因於指定接觸點之此轉換的貢獻。 |
| `conversionEndDate` | 日期 | 轉換期間的結束日期。 |
| `conversionName` | 字串 | 在轉換定義設定步驟中建立的轉換名稱。 |
| `conversionStartDate` | 日期 | 轉換視窗的開始日期。 |
| `geo` | 字串 | 轉換發生的地理位置。 |
| `mediaChannel` | 字串 | 在接觸點設定步驟中使用的管道名稱。 |
| `mediaSubChannel` | 字串 | 子管道的名稱。 |
| `revenue` | 兩次 | 歸因於指定接觸點之此轉換的收入。 |
| `scoreCreatedTime` | 日期時間 | 建立此分數記錄時的時間戳記。 |
| `touchpointEndDate` | 日期 | 接觸點視窗的結束日期。 |
| `touchpointName` | 字串 | 在接觸點定義設定步驟中建立的接觸點名稱。 目前，接觸點定義於媒體頻道上。 |
| `touchpointStartDate` | 日期 | 接觸點視窗的開始日期。 |


## 事件評分資料結構

評分資料的結構描述名稱為`Attribution AI Scores - <name of model> <id> - Schema`。 例如： `Attribution AI Scores - Model for Online Conversion 10120 - Schema`。

保留模型評分資料的資料集命名為`Attribution AI Scores - <name of model> <id>`，例如`Attribution AI Scores - Model for Online Conversion 10120 `。

此結構描述包含一個欄位群組，其中包含一個包含核心詳細資訊的物件。 物件的名稱類似`attibution_AI_scores__<name of model> id`。

欄位群組包含下列欄位。

| 欄位名稱 | 類型 | 說明 |
|---|---|---|
| `conversion` | 物件 | 轉換中繼資料欄。 |
|     `passThrough` | 物件 |  |
|         `eventType` | 字串 | |
|         `channel_typeAtSource` | 字串 | |
|      `dataSource` | 字串 | 資料來源的全域唯一識別碼。<br> **範例：** `Adobe Analytics` |
|      `eventSource` | 字串 | 實際事件發生時的來源。<br> **範例：** `Adobe.com` |
|      `eventType` | 字串 | 此時間序列記錄的主要事件型別。<br> **範例：** `Order` |
|      `geo` | 字串 | 轉換傳遞的地理位置`placeContext.geo.countryCode`。<br> **範例：** `US` |
|      `path` | 字串 | |
|      `priceTotal` | 兩次 | 透過轉換<br>取得的收入 **範例：** `99.9` |
|      `product` | 字串 | 產品本身的XDM識別碼。<br> **範例：** `RX 1080 ti` |
|      `productType` | 字串 | 針對此產品檢視向使用者展示的產品顯示名稱。<br> **範例：** `Gpus` |
|      `quantity` | 整數 | 轉換期間購買的數量。<br> **範例：** `1` |
|      `receivedTimeStamp` | 日期時間 | 已收到轉換的時間戳記。<br> **範例：** `2020-06-09T00:01:51.000Z` |
|      `skuId` | 字串 | 庫存單位(SKU)，供應商所定義之產品的唯一識別碼。<br> **範例：** `MJ-03-XS-Black` |
|      `timestamp` | 日期時間 | 轉換的時間戳記。<br> **範例：** `2020-06-09T00:01:51.000Z` |
|      `totalDaysToConversion` | 整數 |  |
|      `totalTouchpointCount` | 整數 | |
| `customerProfile` | 物件 | 用來建立模型的使用者身分詳細資訊。 |
|      `identity` | 物件 | |
|           `id` | 字串 | |
|           `namespace` | 字串 | 包含用來建置模型的使用者詳細資訊，例如`id`和`namespace`。 |
| `touchpointsDetail` | 物件[] | 導致轉換的接觸點詳細資訊清單，按接觸點出現次數或時間戳記排序。 |
|      `scores` | 物件 | 以此分數表示的接觸點對此轉換的貢獻。 |
|           `algorithmicInfluenced` | 兩次 | 受影響的分數是每個行銷接觸點負責的轉換比例。 |
|           `algorithmicSourced` | 兩次 | 增量分數是行銷接觸點直接造成的邊緣影響量。 |
|           `decayUnits` | 兩次 | 規則型歸因分數，即離轉換較近的接觸點比離轉換較遠的接觸點獲得更多的評分。 |
|           `firstTouch` | 兩次 | 規則型歸因分數，可將所有點數指派給轉換路徑上的初始接觸點。 |
|           `lastTouch` | 兩次 | 規則型歸因分數，可將所有點數指派給最接近轉換的接觸點。 |
|           `linear` | 兩次 | 規則型歸因分數，可將相等點數指派給轉換路徑上的每個接觸點。 |
|           `uShape` | 兩次 | 規則型歸因分數，可將40%的評分指派給第一個接觸點，並將40%的評分指派給最後一個接觸點。 其他接觸點則平分剩餘的20%。 |
|      `touchPoint` | 物件 | 接觸點中繼資料。 |
|           `passThrough` | 物件 | |
|                `eventType` | 字串 | |
|           `campaignGroup` | 字串 |  |
|           `campaignName` | 字串 | |
|           `campaignTag` | 字串 | |
|           `eventId` | 字串 | |
|           `geo` | 字串 | |
|           `mediaAction` | 字串 | |
|           `mediaChannel` | 字串 | |
|           `receivedTimeStamp` | 日期時間 | |
|           `timestamp` | 日期時間 | |
|      `isFirstInThePosition` | 整數 | |
|      `lag` | 整數 | |
|      `position` | 字串 | |
|      `touchpointCountToConversion` | 整數 | |
|      `touchpointName` | 字串 | 安裝期間設定的接觸點名稱。<br> **範例：** `PAID_SEARCH_CLICK` |
| `conversionName` | 字串 | 設定期間設定的轉換名稱。<br> **範例：** `Order`， `Lead`， `Visit` |
| `scoreCreatedTime` | 日期時間 | |
| `segmentation` | 字串 | 轉換區段，例如建立模型時所依據的地理細分。 當區段不存在時，`segmentation`與`conversionName`相同。<br> **範例：** `ORDER_US` |





如需詳細資訊，請參閱[結構描述](../ingest-data/schemas.md)。
