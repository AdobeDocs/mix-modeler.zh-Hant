---
title: 擷取資料概觀
description: 瞭解如何將資料擷取至Mix Modeler。
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
exl-id: dc16a601-bbd9-467b-8a7e-c32654d4069a
source-git-commit: 1a9df9f9819d9e0031e58443ec6a9e755a151ba0
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 7%

---

# 擷取資料概觀

Mix Modeler可處理來自不同圍牆花園的事件層級資料、彙總或摘要行銷成果資料。 以及來自任何其他來源（例如離線廣告、內部因素或外部因素）的彙總或摘要資料。

客戶可以使用擷取到Experience Platform中的任何型別的資料做為資料集，而且這些資料是根據以XDM ExperienceEvent或XDM摘要量度為基底類別的結構描述。

例如：

* 使用Adobe Analytics來源聯結器收集的資料。 並轉換為符合Adobe Analytics結構描述預設或自訂版本的資料集。
* 使用Experience Platform Web SDK、Mobile SDK或Edge Network Server API收集的資料，用於收集網站、行動或任何其他型別裝置上的客戶互動。
* 從封閉花園(如Facebook、YouTube)、流量來源或離線廣告資料彙總或摘要資料。
* 包含對模型建立有用的內部或外部因素的非行銷彙總或摘要資料。

您可以使用Experience Platform支援的任何一種機制，從其他來源擷取體驗事件層級、彙總行銷成果資料和資料。 例如Experience Platform SDK、API、來源聯結器，以及串流和批次擷取。 若要進一步瞭解如何在Experience Platform擷取資料以用於Adobe Mix Modeler，請參閱[資料擷取概觀](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/ingestion/home)。

## 准則

若要將資料擷取至Experience Platform以與Mix Modeler搭配使用，請遵循下列准則：

* 新增到資料集的增量資料中不應有任何重疊。
* 來自單一來源的所有資料應該具有相同的詳細程度。
* 對於所有擷取為資料集的彙總資料，日期和詳細程度是基礎結構描述中的必填欄位
* 管道是基礎結構描述中所有行銷工作/支出資料擷取為資料集的必要欄位。


## 範例

除了較標準的體驗事件資料外，以下提供Mix Modeler中通常使用的一些資料範例。

+++ 彙總行銷成果資料

| 地理 | 日期 | 日期型別 | Channel | Campaign | 按一下 | 盈餘 | 參與度 | 曝光 | 開啟 | 已擁有 | 已傳送 | 支出 |
|---|:--|---|:---:|---|--:|---|--:|---|---|---|--:|--:|
| AMER | 2021-10-31 | 天 | 電子郵件 | | 12752 | | | | | | 1132945 | |
| AMER | 2021-10-31 | 天 | FB | | 148844 | | | | | | | 42111 |
| AMER | 2021-10-31 | 天 | YT | | | | 2314452 | | | | | 10540 |
| 日文 | 2021-10-21 | 天 | 電子郵件 | | 21089 | | | | | | 3283626 | |
| 日文 | 2021-10-21 | 天 | 社交 | | | | 621 | | | | | 74512 |

{style="table-layout:auto"}

+++

+++ 彙總轉換資料

| 地理 | 日期 | 日期型別 | 產品 | 售出單位 | 收入 |
|---|:---|:---:|---|--:|--:|
| EMEA | 2021-09-13 | 天 | 創造者經濟 | 603 | 36537.68 |
| EMEA | 2021-09-13 | 天 | Metaverse | 55 | 21704.37 |
| 日文 | 2022-05-30 | 天 | Pro Imaging | 487 | 64469.60 |
| 日文 | 2022-05-30 | 天 | Document Cloud | 642 | 100509.07 |

{style="table-layout:auto"}

+++

+++ 外部因素資料

| 資料 | 日期型別 | 因數 | 價值 |
|---|:---:|:---:|:---|
| 2020-08-02 | 周 | SPX | 3325.866 |
| 2020-08-09 | 周 | SPX | 3364.158 |
| 2020-08-16 | 周 | SPX | 3385.858 |
| 2020-08-23 | 周 | SPX | 3497.965 |

{style="table-layout:auto"}

+++

若要在Mix Modeler中處理資料，您需要在資料集中收集資料，並仿照Experience Platform中的結構描述建模。 Mix Modeler介面可讓您輕鬆存取Experience Platform結構描述和資料集UI。


## 驗證

若要驗證您的資料在Mix Modeler中是否正確可用，您可以進行下列工作：

* 在[概觀](/help/overview.md)中使用視覺效果。
* 下載並檢查協調資料集中[協調的資料](/help/harmonize-data/overview.md)中的資料。

若要驗證Experience Platform中是否正確擷取您的資料，您可以[使用Experience Platform查詢服務](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/query/home)來寫入及執行SQL查詢。


>[!MORELIKETHIS]
>
>如需有關如何管理結構描述和資料集的詳細資訊，請參閱：
>
>* [結構描述](schemas.md)
>* [資料集](datasets.md)
