---
title: 行銷接觸點
description: 瞭解如何在Mix Modeler中建立行銷接觸點，以用來協調您的資料。
feature: Harmonized Data, Marketing Touch Points
exl-id: 42851107-7568-4bc9-92ca-3cba713a522e
source-git-commit: 1a9df9f9819d9e0031e58443ec6a9e755a151ba0
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 11%

---

# 行銷接觸點 {#marketing-touchpoints}

>[!CONTEXTUALHELP]
>id="harmonizeddata_marketingtouchpoint"
>title="行銷接觸點"
>abstract="行銷接觸點為收件者、個體和/或 cookie 層級的行銷事件，用於評估行銷投資對數值型或收入型轉換的影響。"


行銷接觸點為收件者、個體和/或 cookie 層級的行銷事件，用於評估行銷投資對數值型或收入型轉換的影響。

您可以定義行銷接觸點來協助進行歸因分析。

## 管理行銷接觸點

若要檢視Mix Modeler介面中可用的行銷接觸點表格：

1. 從左側邊欄選取![資料搜尋](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]**。

1. 從頂端列選取&#x200B;**[!UICONTROL Marketing touchpoint]**。 您會看到行銷接觸點表格。 如果有更多頁面可供使用，請使用![x](/help/assets/icons/ChevronLeft.svg)的![x](/help/assets/icons/ChevronRight.svg)上的&#x200B;**[!UICONTROL Page _向左箭頭&#x200B;_或_向右箭頭_]**&#x200B;在資料表的頁面之間移動。

表格欄會指定行銷接觸點的詳細資訊：

| 欄名稱 | 詳細資料 |
| --- | ---|
| 名稱 | 行銷接觸點的名稱。 |
| 支出量度 | 用於計算接觸點支出的協調資料量度。 |
| 數量度 | 用於計算接觸點數量的協調資料量度。 |
| 規則 | 要使用的接觸點規則。 |
| 已建立 | 建立行銷接觸點的日期和時間。 |
| 上次修改時間 | 上次修改行銷接觸點的日期和時間。 |


## 新增行銷接觸點

若要新增行銷接觸點，請在Mix Modeler的![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Marketing touchpoint]**&#x200B;介面中：

1. 選取![新增](/help/assets/icons/AddCircle.svg)新增行銷接觸點。

1. 在&#x200B;**[!UICONTROL Marketing touchpoint]**&#x200B;對話方塊。

   1. 輸入&#x200B;**[!UICONTROL Touchpoint Name]**&#x200B;的名稱，例如`Luma Touchpoint`。

   1. 定義&#x200B;**[!UICONTROL Touchpoint rule]**。

      1. 從&#x200B;**[!UICONTROL *選取協調的&#x200B;*]**中選取一個值，例如&#x200B;**[!UICONTROL Brand]**。

      1. 選取運運算元![V](/help/assets/icons/ChevronDown.svg)的值，例如&#x200B;**[!UICONTROL is]**。

      1. 從&#x200B;**[!UICONTROL *選取值&#x200B;*]**或輸入值，例如&#x200B;**[!DNL Luma]**。

   1. 從&#x200B;**[!UICONTROL Touchpoint volume]**&#x200B;中選取協調欄位，例如&#x200B;**[!UICONTROL Impressions]**。

   1. 從&#x200B;**[!UICONTROL Touchpoint spend]**&#x200B;中選取協調欄位，例如&#x200B;**[!UICONTROL Cost]**。

      ![行銷接觸點](/help/assets/create-touchpoint.png)

   1. 若要建立行銷接觸點，請選取&#x200B;**[!UICONTROL Create]**。 若要取消建立行銷接觸點，請選取「**[!UICONTROL Cancel]**」。

1. 建立後，接觸點會新增至行銷接觸點表格。


## 檢視詳細資料

若要檢視行銷接觸點的詳細資訊：

1. 選取![更多](/help/assets/icons/More.svg) （當滑鼠游標停留在表格中的行銷接觸點名稱上時）。

1. 選取![檢視](/help/assets/icons/ViewDetail.svg) **檢視**。 對話方塊會顯示行銷接觸點的詳細資訊。 如需詳細資訊，請參閱[新增行銷接觸點](#add-a-marketing-touchpoint)。 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以關閉對話方塊。


## 檢視報告

若要檢視行銷接觸點的報表：

1. 選取![更多](/help/assets/icons/More.svg) （當滑鼠游標停留在表格中的行銷接觸點名稱上時）。

1. 選取![GraphTrend](/help/assets/icons/GraphTrend.svg) **檢視報告**。 對話方塊會顯示行銷接觸點的報告。

   ![行銷接觸點檢視報告](../assets/marketingtouchpoint-view-report.png)

   * 若要變更報告粒度，請從&#x200B;**[!UICONTROL Weekly]**&#x200B;下拉式選單中選取值。
   * 若要變更要報告的期間，請輸入開始與結束日期，或使用![行事曆](/help/assets/icons/Calendar.svg)在行事曆快顯視窗中定義期間。

1. 選取&#x200B;**[!UICONTROL Close]**&#x200B;以關閉對話方塊。

## 刪除行銷接觸點

若要刪除行銷接觸點：

1. 選取![刪除](/help/assets/icons/Delete.svg) **刪除** （當滑鼠游標停留在表格中的行銷接觸點名稱上時）。
1. 在&#x200B;**[!UICONTROL Delete touchpoint]**&#x200B;對話確認對話方塊中，選取&#x200B;**[!UICONTROL Delete]**&#x200B;以永久刪除行銷接觸點。

