---
title: 轉換
description: 瞭解如何建立轉換，以便用於協調Mix Modeler中的資料。
feature: Harmonized Data, Conversions
exl-id: a8559426-452a-43e8-9a60-0c0bc97d863c
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 1%

---

# 轉換

轉換事件是業務目標，可識別行銷活動的影響。 範例：電子商務訂單、店內購買、網站造訪等。

您可以定義歸因分析的行銷轉換。

## 管理轉換

若要檢視可用轉換的表格，請在Mix Modeler介面中：

1. 選取 ![資料搜尋](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 從左側邊欄。

1. 選取 **[!UICONTROL Conversions]** 從頂端列。 您會看到轉換率表格。

表格資料欄會指定轉換的詳細資訊：

| 欄名稱 | 詳細資料 |
| --- | ---|
| 名稱 | 轉換的名稱。 |
| 收入 | 用於計算轉換收入的協調資料量度。 |
| 轉換量度 | 用作分析轉換量度的協調資料量度。 |
| 類別 | 轉換的轉換類別。 |
| 已建立 | 建立轉換的日期和時間。 |
| 上次修改時間 | 上次修改轉換的日期和時間。 |

{style="table-layout:auto"}

## 新增轉換

若要新增轉換，請在 ![資料搜尋](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Conversion]** Mix Modeler介面：

1. 選取 ![新增](../assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion]**.

1. 在 **[!UICONTROL Create conversion]** 對話方塊：

   1. 輸入名稱 **[!UICONTROL Conversion]**，例如 `Store Conversions`.

   1. 定義 **[!UICONTROL Conversion category]**.

      1. 選取值，從 **[!UICONTROL *選取協調……*]**，例如 `Conversion types`.

      1. 選取運運算元的值 ![V形](../assets/icons/ChevronDown.svg)，例如 **[!UICONTROL is]**.

      1. 選取值，從 **[!UICONTROL *選取值&#x200B;*]**或輸入值，例如&#x200B;**[!UICONTROL Store]**.

   1. 選取協調欄位，從 **[!UICONTROL Conversion metric for analysis]**，例如 **[!UICONTROL Orders]**.

   1. 選取協調欄位，從 **[!UICONTROL Revenue field]**，例如 **[!UICONTROL Gross Demand]**.

   1. 若要建立轉換，請選取 **[!UICONTROL Create]**. 若要取消轉換的建立，請選取 **[!UICONTROL Cancel]**.

      ![替代文字](../assets/create-conversion.png)

1. 建立後，轉換會被新增到轉換表格中。


## 檢視轉換

若要檢視轉換：

1. 選取 ![更多](../assets/icons/More.svg) 將滑鼠游標停留在表格中的轉換名稱上時。

1. 選取 ![檢視](../assets/icons/ViewDetail.svg) **檢視**. 對話方塊會顯示轉換的詳細資料。 另請參閱 [新增轉換](#add-a-conversion) 以取得詳細資訊。 選取 **[!UICONTROL Cancel]** 以關閉對話方塊。


## 刪除轉換

若要刪除轉換：

1. 選取 ![刪除](../assets/icons/Delete.svg) **刪除** 將滑鼠游標停留在表格中的轉換名稱上時。
1. 在 **[!UICONTROL Delete conversion]** 對話方塊確認對話方塊選取 **[!UICONTROL Delete]** 以永久刪除轉換。
