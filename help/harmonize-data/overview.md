---
title: 協調資料
description: 瞭解如何協調Mix Modeler中的資料。
feature: Harmonized Data
exl-id: 6cb70762-e3b2-46a0-b028-1d6daf3edae5
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 7%

---

# 協調資料

視資料來源而定，Mix Modeler中的資料具有不同性質。 資料可以是：

* 彙總或摘要資料，例如，從圍牆花園資料來源收集而來，或是從公告牌行銷活動、事件或實體廣告行銷活動收集而來的離線廣告資料（如支出）。
* 事件資料，例如來自第一方資料來源的資料。 此事件資料可以透過Adobe Analytics來源聯結器從Adobe Analytics收集，或透過Experience Platform網頁或行動SDK或Edge Network API收集，或使用來源聯結器擷取的資料。

Mix Modeler的協調服務會將彙總和事件資料同化為一致的資料檢視。 此資料檢視結合內部和外部因素資料，是Mix Modeler中模型的來源。 此服務會使用不同資料集的最高精細度。 例如，如果某個資料集的詳細程度為每月，而其餘資料集的詳細程度為每週和每日，則協調服務會使用每月詳細程度建立資料檢視。

## 協調資料的範例

假設您有以下資料集可用於Mix Modeler。

**資料集1**

包含來自YouTube的行銷活動資料集，其彙總資料集的詳細程度為每日。

| 日期 | 日期型別 | Channel | Campaign | 品牌 | 地理 | 點按次數 | 支出 |
|---|:--:|---|---|---|---|---:|---:|
| 12-31-2021 | 天 | YouTube | Y_Fall_02 | BrandX | US | 10000 | 100 |
| 01-01-2022 | 天 | YouTube | Y_Fall_02 | BrandX | US | 1000 | 10 |
| 01-03-2022 | 天 | YouTube | Y_Fall_01 | BrandY | CA | 10000 | 100 |
| 01-04-2022 | 天 | YouTube | Y_Summer_01 | 空 | CA | 9000 | 80 |

{style="table-layout:auto"}


**資料集2**

包含Facebook的行銷成果資料集，其彙總資料的詳細程度設定為每週。

| 日期 | 日期型別 | Channel | Campaign | 地理 | 點按次數 | 支出 |
|--- |:---:|--- |---|---|---:|---:|
| 01-01-2022 | 周 | facebook | FB_Fall_01 | US | 8000 | 100 |
| 01-08-2022 | 周 | facebook | FB_Fall_02 | US | 1000 | 10 |
| 01-08-2022 | 周 | facebook | FB_Fall_01 | US | 7000 | 100 |
| 01-16-2022 | 周 | facebook | FB_Summer_01 | CA | 10000 | 80 |

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

| 時間戳記 | 身分命名空間 | 身分ID | Channel | 點按次數 |
|--- |--- |--- |--- |---:|
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 2ca2a16e-caf0-4fa9-9a8b-9774b39547c4 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 5ce99bfb-e44a-40d9-b8cd-c5408bda7cdc | CSE | 1 |

{style="table-layout:auto"}


您想要建立協調的資料集，並將詳細程度設定為每週。 事件資料會彙總至周粒度，並新增至協調的資料集。 結果為：

**協調的資料集**

| 日期 | 日期型別 | Channel | Campaign | 品牌 | 地理 | 目標 | 點按次數 | 支出 | 收入 |
|--- |:---:|--- |--- |--- |---|---|---:|---:|---:|
| 12-27-2021 | 周 | YouTube | Y_Fall_02 | BrandX | US | 空 | 11000 | 110 | 空 |
| 01-03-2022 | 周 | YouTube | Y_Fall_01 | BrandY | CA | 空 | 10000 | 100 | 空 |
| 01-03-2022 | 周 | YouTube | Y_Summer_01 | 空 | CA | 空 | 9000 | 80 | 空 |
| 01-01-2022 | 周 | facebook | FB_Fall_01 | 空 | US | 空 | 8000 | 100 | 空 |
| 01-08-2022 | 周 | facebook | FB_Fall_02 | 空 | US | 空 | 1000 | 10 | 空 |
| 01-08-2022 | 周 | facebook | FB_Fall_01 | 空 | US | 空 | 7000 | 100 | 空 |
| 01-16-2022 | 周 | facebook | FB_Summer_01 | 空 | CA | 空 | 10000 | 80 | 空 |
| 12-27-2021 | 周 | 空 | 空 | 空 | US | 時尚 | 空 | 空 | 200 |
| 01-03-2022 | 周 | 空 | 空 | 空 | US | 時尚 | 空 | 空 | 10 |
| 01-03-2022 | 周 | 空 | 空 | 空 | US | 珠寶 | 空 | 空 | 1100 |
| 01-10-2022 | 周 | 空 | 空 | 空 | CA | 珠寶 | 空 | 空 | 80 |
| 01-01-2022 | 周 | CSE | 空 | 空 | 空 | 空 | 2 | 空 | 空 |
| 01-08-2022 | 周 | CSE | 空 | 空 | 空 | 空 | 2 | 空 | 空 |

{style="table-layout:auto"}


## 設定協調資料

若要建置協調的資料集（如在簡化的[範例](#an-example-of-harmonized-data)中），您必須遵循下列步驟：

1. 定義其他[個要使用的協調欄位](fields.md)，這些協調欄位已超出可用的全球協調欄位。
1. 設定[資料集規則](dataset-rules.md)，將彙總或體驗事件資料集中的欄位對應到協調的欄位。
1. 使用您定義的標準和其他協調欄位來定義[行銷接觸點](marketing-touchpoints.md)。
1. 使用您定義的標準和其他協調欄位來定義[轉換](conversions.md)。


## 檢視已協調的資料

若要在Mix Modeler介面中檢視您的協調資料：

1. 從左側邊欄選取![資料搜尋](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized datasets]**。

1. 從頂端列選取&#x200B;**[!UICONTROL Harmonized Data]**。 系統會根據您定義的欄位、資料集規則、行銷接觸點和轉換，顯示您協調資料的摘要。

   1. 若要重新定義重新擷取協調資料所依據的期間，請輸入&#x200B;**[!UICONTROL Date range]**&#x200B;的日期範圍，或使用![行事曆](/help/assets/icons/Calendar.svg)來選取資料範圍。

   1. 若要修改「協調」資料表所顯示的協調欄位欄，請使用![設定](/help/assets/icons/Setting.svg)開啟&#x200B;**[!UICONTROL Column settings]**&#x200B;對話方塊。

      1. 從&#x200B;**[!UICONTROL AVAILABLE COLUMNS]**&#x200B;選取![SelectBox](/help/assets/icons/SelectBox.svg)一或多個資料行，並使用![右側V形](/help/assets/icons/ChevronRight.svg)將這些資料行新增到&#x200B;**[!UICONTROL SELECTED COLUMNS]**。

      1. 從&#x200B;**[!UICONTROL SELECTED COLUMNS]**&#x200B;中選取![SelectBox](/help/assets/icons/SelectBox.svg)一或多個資料行，並使用![左V形](/help/assets/icons/ChevronLeft.svg)來移除選取的資料行，並將這些資料行傳回&#x200B;**[!UICONTROL AVAILABLE COLUMNS]**。

      1. 從&#x200B;**[!UICONTROL DEFAULT SORT]**&#x200B;中選取欄，並在&#x200B;**[!UICONTROL Ascending]**&#x200B;或&#x200B;**[!UICONTROL Descending]**&#x200B;之間切換。

      1. 若要變更欄的顯示順序，您可以透過拖放將&#x200B;**[!UICONTROL SELECTED COLUMNS]**&#x200B;中的欄上下移動。

   1. 選取&#x200B;**[!UICONTROL Submit]**&#x200B;以提交您的欄設定變更。 選取&#x200B;**[!UICONTROL Close]**&#x200B;以取消您所做的任何變更。

1. 如果有更多頁面可供使用，請使用&#x200B;_x _]**的**[!UICONTROL Page _x_&#x200B;上的![向左箭頭](/help/assets/icons/ChevronLeft.svg)或![向右箭頭](/help/assets/icons/ChevronRight.svg)在頁面之間移動。
