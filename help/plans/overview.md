---
title: 計畫總覽
description: 瞭解如何在Mix Modeler中檢視、選取和操作計畫。
feature: Plans
exl-id: 45a8dc30-3259-493d-8ea5-1899903733a6
source-git-commit: 8e1c748f3e4e267038dcac5bce82f90157e88c32
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 1%

---

# 計畫總覽

Mix Modeler中的計畫可讓您依業務單位和管道分配預算。 計畫功能會根據您協調的資料與已訓練模型的結果整合。

計畫會概述企業打算在指定的時間範圍內，為服務通用KPI （例如訂單、收入）而在行銷相關專案上花費的任意投資（例如預算）。 計畫可包含來自付費廣告、贊助網路內容、活動等管道的費用。

計畫需要：

- 模型，
- 資料範圍，
- 預算。

計畫可選擇性地包括：

- 設定的辨識視窗，
- 多個航班日期，每個日期都有目標預算，
- 依據管道和投放日期的最小和最大預算限制。

如果您用於計畫的模型已在新資料上評分，則需要建立新計畫以考慮重新評分的資料。


## 建置計畫

若要建立計畫，請使用Mix Modeler計畫建立精靈。 如需詳細資訊，請參閱[建置計畫](build.md)。

## 管理計畫

若要檢視目前計畫的表格，請在Mix Modeler介面中：

1. 從左側邊欄選取![](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]**。

1. 您會看到目前計畫及其狀態的表格。

   表格資料欄會指定計畫的詳細資訊。

   | 欄名稱 | 詳細資料 |
   |---|---|
   | 名稱 | 計畫名稱 |
   | 模型 | 作為計畫基礎的模型。 |
   | 日期範圍 | 計畫的完整日期範圍。 |
   | 預算 | 計畫的總預算。 |
   | 預測回訪 | 計畫的預測傳回 |
   | 預測的投資報酬率 | 計畫的預測ROI。 |
   | 預測的轉換 | 計畫的預測轉換 |
   | 預測的CPA | 計畫的預測CPA |
   | 狀態 | 計畫的狀態： <p><span style="color:red">●</span>失敗， <p><span style="color:blue">●</span>正在處理，或 <p><span style="color:green">●</span>完成。 |

   {style="table-layout:auto"}

   您可以使用![ColumnSetting](/help/assets/icons/ColumnSetting.svg)來選取![核取標籤](/help/assets/icons/Checkmark.svg)要在資料表中顯示的資料行。

1. 使用![搜尋](/help/assets/icons/Search.svg)來搜尋和篩選一或多個特定計畫的資料表。

### 計畫深入分析

若要檢視計畫的深入分析並編輯計畫：

1. 從左側邊欄選取![PLan](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]**。

1. 選取計畫名稱。

您被重新導向至[計畫深入分析](insights.md)。


### 複製計畫

若要複製計畫，請執行下列步驟：

- 為計畫選取![更多](/help/assets/icons/More.svg)。 從內容功能表中選取&#x200B;**[!UICONTROL Duplicate]**。
- 或者，在表格![SelectBox](/help/assets/icons/SelectBox.svg)中選取計畫，然後從藍色動作列選取![複製](/help/assets/icons/Copy.svg) **[!UICONTROL Duplicate]**。

新計畫的名稱是由原始計畫的名稱附加至&#x200B;**[!UICONTROL (Copy)](_n_)**&#x200B;所組成，已新增至表格頂端。

### 比較計畫

若要比較計畫：

1. 從表格中選取兩個計畫。
1. 從藍色動作列中選取![比較](/help/assets/icons/Compare.svg) **[!UICONTROL Compare]**。 您看見&#x200B;**[!UICONTROL Compare plans]** UI。


### 刪除計畫

若要刪除計畫，請執行下列步驟：

1. 為計畫選取![更多](/help/assets/icons/More.svg)。 從內容功能表選取&#x200B;**[!UICONTROL Delete]**。 <br/>或者，在表格![SelectBox](/help/assets/icons/SelectBox.svg)中選取計畫，然後從藍色動作列選取![刪除](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**。
1. 在&#x200B;**[!UICONTROL Delete plan]**&#x200B;確認對話方塊中選取&#x200B;**[!UICONTROL Delete]**&#x200B;以刪除計畫。 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消。

若要刪除多個計畫：

1. 選取多個計畫。
1. 從藍色動作列中，選取![刪除](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;以刪除計畫。
1. 在&#x200B;**[!UICONTROL Delete *x *計畫]**確認對話方塊中選取&#x200B;**[!UICONTROL Delete]**以刪除計畫。 選取&#x200B;**[!UICONTROL Cancel]**以取消。


