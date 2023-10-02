---
title: 協調資料
description: 瞭解如何協調Mix Modeler中的資料。
feature: Harmonized Data
source-git-commit: c145754ecd6a6d8f5aab333ced739c4053aeaae5
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 16%

---


# 協調資料

視資料來源而定，Mix Modeler中的資料具有不同性質。 資料可以是：

* 彙總資料，例如從圍牆花園資料來源收集而來，或是從廣告牌行銷活動、活動或實體廣告行銷活動收集而來的離線廣告資料（如支出），
* 事件資料，例如來自第一方資料來源的資料。 此事件資料可以透過Adobe Analytics來源聯結器從Adobe Analytics收集，或透過Adobe Experience Platform Web、Mobile SDK或Edge Network API收集，或使用來源聯結器擷取的資料。

Mix Modeler的協調服務會將彙總和事件資料同化為一致的資料檢視。 此資料檢視是Mix Modeler中計畫和模型的來源。

## 協調資料的範例

假設您有以下資料集可用於Mix Modeler。

**資料集1**

包含來自YouTube的行銷活動資料集，其彙總資料集的詳細程度為每日。

| 日期 | 日期型別 | Channel | Campaign | 品牌 | 地理 | 點擊數 | 支出 |
|---|:--:|---|---|---|---|---:|---:|
| 12-31-2021 | 天 | YouTube | Y_Fall_02 | BrandX | US | 10000 | 100 |
| 01-01-2022 | 天 | YouTube | Y_Fall_02 | BrandX | US | 1000 | 10 |
| 01-03-2022 | 天 | YouTube | Y_Fall_01 | BrandY | CA | 10000 | 100 |
| 01-04-2022 | 天 | YouTube | Y_Summer_01 | 空 | CA | 9000 | 80 |

{style="table-layout:auto"}


**資料集2**

包含Facebook的行銷成果資料集，其彙總資料的詳細程度設定為每週。

| 日期 | 日期型別 | Channel | Campaign | 地理 | 點擊數 | 支出 |
|--- |:---:|--- |---|---|---:|---:|
| 01-01-2022 | 週 | facebook | FB_Fall_01 | US | 8000 | 100 |
| 01-08-2022 | 週 | facebook | FB_Fall_02 | US | 1000 | 10 |
| 01-08-2022 | 週 | facebook | FB_Fall_01 | US | 7000 | 100 |
| 01-16-2022 | 週 | facebook | FB_Summer_01 | CA | 10000 | 80 |

{style="table-layout:auto"}


**資料集3**

轉換資料集，彙總資料集的粒度設定為每日。

| 日期 | 日期型別 | 地理 | 目標 | 收入 |
|--- |:---: |---|---|---:|
| 01-01-2022 | 天 | US | 時尚 | 200 |
| 01-08-2022 | 天 | US | 時尚 | 10 |
| 01-08-2022 | 天 | US | 珠寶 | 1100 |
| 01-16-2022 | 天 | CA | 珠寶 | 80 |

{style="table-layout:auto"}


**資料集4**

來自客戶的體驗事件資料集（Web SDK事件）範例。

| 時間戳記 | 身分識別命名空間 | 身分ID | Channel | 點擊數 |
|--- |--- |--- |--- |---:|
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 2ca2a16e-caf0-4fa9-9a8b-9774b39547c4 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 5ce99bfb-e44a-40d9-b8cd-c5408bda7cdc | CSE | 1 |

{style="table-layout:auto"}


您想要建立協調的資料集，並將詳細程度設定為每週。 事件資料會彙總至周粒度，並新增至協調的資料集。 結果為：

**協調的資料集**

| 日期 | 日期型別 | Channel | Campaign | 品牌 | 地理 | 目標 | 點擊數 | 支出 | 收入 |
|--- |:---:|--- |--- |--- |---|---|---:|---:|---:|
| 12-27-2021 | 週 | YouTube | Y_Fall_02 | BrandX | US | 空 | 11000 | 110 | 空 |
| 01-03-2022 | 週 | YouTube | Y_Fall_01 | BrandY | CA | 空 | 10000 | 100 | 空 |
| 01-03-2022 | 週 | YouTube | Y_Summer_01 | 空 | CA | 空 | 9000 | 80 | 空 |
| 01-01-2022 | 週 | facebook | FB_Fall_01 | 空 | US | 空 | 8000 | 100 | 空 |
| 01-08-2022 | 週 | facebook | FB_Fall_02 | 空 | US | 空 | 1000 | 10 | 空 |
| 01-08-2022 | 週 | facebook | FB_Fall_01 | 空 | US | 空 | 7000 | 100 | 空 |
| 01-16-2022 | 週 | facebook | FB_Summer_01 | 空 | CA | 空 | 10000 | 80 | 空 |
| 12-27-2021 | 週 | 空 | 空 | 空 | US | 時尚 | 空 | 空 | 200 |
| 01-03-2022 | 週 | 空 | 空 | 空 | US | 時尚 | 空 | 空 | 10 |
| 01-03-2022 | 週 | 空 | 空 | 空 | US | 珠寶 | 空 | 空 | 1100 |
| 01-10-2022 | 週 | 空 | 空 | 空 | CA | 珠寶 | 空 | 空 | 80 |
| 01-01-2022 | 週 | CSE | 空 | 空 | 空 | 空 | 2 | 空 | 空 |
| 01-08-2022 | 週 | CSE | 空 | 空 | 空 | 空 | 2 | 空 | 空 |

{style="table-layout:auto"}


## 設定協調資料

建立統一的資料集，如簡化的資料集 [範例](#an-example-of-harmonized-data)，您必須遵循下列步驟：

1. 定義其他 [協調的欄位](fields.md) 您想要使用已提供的全球協調欄位以外的其他欄位。
1. 設定 [資料集規則](dataset-rules.md) 將彙總或體驗事件資料集中的欄位對應到協調的欄位。
1. 定義 [行銷接觸點](marketing-touchpoints.md) 使用您定義的標準和其他協調欄位。
1. 定義 [轉換](conversions.md) 使用您定義的標準和其他協調欄位。


## 檢視已協調的資料

若要在Mix Modeler介面中檢視您的協調資料：

1. 選取 ![資料搜尋](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized datasets]** 從左側邊欄。

1. 選取 **[!UICONTROL Harmonized Data]** 從頂端列。 您可以根據欄位、資料集規則、行銷接觸點以及您定義的轉換，檢視已協調的資料摘要。

   1. 若要重新定義重新計算協調資料所依據的期間，請輸入日期範圍 **[!UICONTROL Date range]** 或使用 ![行事曆](../assets/icons/Calendar.svg) 以選取資料範圍。

   1. 若要修改「協調資料」表格中顯示的欄，請使用 ![設定](../assets/icons/Setting.svg) 以開啟 **[!UICONTROL Column settings]** 對話方塊。

      1. 選取 ![SelectBox](../assets/icons/SelectBox.svg) 一或多個資料行 **[!UICONTROL AVAILABLE COLUMNS]** 和使用 ![V形箭號右側](../assets/icons/ChevronRight.svg) 以新增這些欄至 **[!UICONTROL SELECTED COLUMNS]**.

      1. 選取 ![SelectBox](../assets/icons/SelectBox.svg) 一或多個資料行 **[!UICONTROL SELECTED COLUMNS]** 和使用 ![左側V形](../assets/icons/ChevronLeft.svg) 以移除選取的欄，並將這些欄傳回 **[!UICONTROL AVAILABLE COLUMNS]**.

      1. 選取欄，從 **[!UICONTROL DEFAULT SORT]** 並在兩者之間切換 **[!UICONTROL Ascending]** 或 **[!UICONTROL Descending]**.

      1. 若要變更欄的顯示順序，您可以將欄移入 **[!UICONTROL SELECTED COLUMNS]** 透過拖放方式來上下移動。

   1. 選取 **[!UICONTROL Submit]** 以提交欄設定變更。 選取 **[!UICONTROL Close]** 以取消您所做的任何變更。


