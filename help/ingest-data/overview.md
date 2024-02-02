---
title: 擷取資料
description: 瞭解如何將資料擷取至Mix Modeler。
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
exl-id: dc16a601-bbd9-467b-8a7e-c32654d4069a
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 8%

---

# 擷取資料

Mix Modeler可搭配事件層級資料、彙總來自各牆壁花園的oe摘要行銷成果資料，以及彙總來自任何其他來源（例如離線廣告、內部因素或外部因素）的摘要資料。

客戶可以使用任何種類的資料當作資料集擷取到Experience Platform中，而且這些資料是根據以XDM ExperienceEvent或XDM摘要量度為基底類別的結構描述。

例如：

* 使用Adobe Analytics來源聯結器收集並轉換為符合Adobe Analytics結構描述預設或自訂版本的資料集，或是
* 使用Experience Platform Web SDK、Mobile SDK或Edge Network Server API收集的資料，用於收集網站、行動或任何其他型別裝置上的客戶互動。
* 從封閉花園(例如Facebook、YouTube)、流量來源或離線廣告資料彙總或摘要資料，
* 包含對模型建立有用的內部或外部因素的非行銷彙總或摘要資料。

您可以使用Experience Platform支援的任何一種機制，從其他來源擷取體驗事件層級、彙總行銷成果資料和資料。 例如Experience PlatformSDK、API、來源聯結器，以及串流和批次擷取。


## 准則

若要將資料擷取至Experience Platform以與Mix Modeler搭配使用，請遵循下列准則：

* 新增到資料集的增量資料中不應有任何重疊。
* 來自單一來源的所有資料應該具有相同的詳細程度。
* 對於所有擷取為資料集的彙總資料，日期和詳細程度是基礎結構描述中的必填欄位
* 管道是基礎結構描述中所有行銷工作/支出資料擷取為資料集的必要欄位。


## 範例

除了較標準的體驗事件資料外，以下提供一些通常用於Mix Modeler的資料範例。

+++ 彙總行銷成果資料

| 地理 | 日期 | 日期型別 | Channel | Campaign | 按一下 | 盈餘 | 參與 | 曝光 | 開啟 | 已擁有 | 已傳送 |
|---|:--|---|:---:|---|--:|---|--:|---|---|---|--:|
| AMER | 2021-10-31 | 天 | 電子郵件 | | 12752 | | | | | | 1132945 |
| AMER | 2021-10-31 | 天 | FB | | 148844 | | | | | | |
| AMER | 2021-10-31 | 天 | YT | | | | 2314452 | | | | |
| 日文 | 2021-10-21 | 天 | 電子郵件 | | 21089 | | | | | | 3283626 |
| 日文 | 2021-10-21 | 天 | 社交 | | | | 621 | | | | |

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

| 資料 | 日期型別 | 因數 | 值 |
|---|:---:|:---:|:---|
| 2020-08-02 | 周 | SPX | 3325.866 |
| 2020-08-09 | 周 | SPX | 3364.158 |
| 2020-08-16 | 周 | SPX | 3385.858 |
| 2020-08-23 | 周 | SPX | 3497.965 |

{style="table-layout:auto"}

+++

若要在Mix Modeler中處理資料，您需要在資料集中收集資料，並在Experience Platform中根據結構描述建模。 Mix Modeler介面可讓您輕鬆存取「Experience Platform結構描述」和「資料集」UI。


>[!MORELIKETHIS]
>
>如需有關如何管理結構描述和資料集的詳細資訊，請參閱：
>
>* [方案](schemas.md)
>* [資料集](datasets.md)
