---
title: 建置計畫
description: 瞭解如何在Mix Modeler中建置計畫。
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
source-git-commit: d05eccef370598ce64363ca6ae20886b0e5dccd0
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---


# 建置計畫

在Mix Modeler中，您可以使用計畫畫布建立計畫。 在計畫畫布中，您可以設定計畫的明細與預算，以及計畫要使用的基本模型。 一旦您指定了詳細資訊、預算和模型，您就可以繼續進行AI推薦的計畫或編輯依據管道的支出。

若要建立計畫，請在Mix Modeler的![PLan](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]**&#x200B;介面中選取&#x200B;**[!UICONTROL Create plan]**。

1. 在&#x200B;**[!UICONTROL Plan creation]**&#x200B;畫面中：

   1. 在&#x200B;**[!UICONTROL Setup]**&#x200B;區段中：

      1. 輸入&#x200B;**[!UICONTROL Plan name]**，例如`Demo plan`。 輸入&#x200B;**[!UICONTROL Description]**，例如`Demo plan for Luma company`。
      1. 從&#x200B;**[!UICONTROL _中選取&#x200B;**[!UICONTROL Model]**選取選項……_.]**
      1. 您可以選取![LinkOut](/help/assets/icons/LinkOut.svg) **[!UICONTROL Create model]**，以直接從計畫建立中建立模型。 這會在您的瀏覽器中開啟新索引標籤，並顯示[模型](../models/overview.md)介面。

         ![計畫設定](/help/assets/plan-setup.png)

   1. 在&#x200B;**[!UICONTROL Budget]**&#x200B;區段中：

      1. 透過輸入日期或使用![行事曆](/help/assets/icons/Calendar.svg)選取日期範圍來指定日期範圍。
      1. 輸入預算。

      若要新增其他日期範圍（每個日期範圍都有預算），請選取![行事曆新增](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**。

      若要刪除日期範圍和相關預算，請選取![關閉](/help/assets/icons/Close.svg)。

      若要定義指定的最大預算，請執行下列步驟：

      1. 切換&#x200B;**[!UICONTROL Maximize budget]**&#x200B;開啟。
      1. 指定最大預算金額。 金額應等於或高於為日期範圍指定的預算總金額。

         ![計畫預算](/help/assets/plan-budget.png)

   1. 選擇「**[!UICONTROL Next]**」。

1. 在&#x200B;**[!UICONTROL Done with all required fields]**&#x200B;對話方塊：

   ![完成計畫](/help/assets/plan-done-required-fields.png)

   * 選擇 <img src="/help/assets/icons/NewPlan.svg" width="25" /> **[!UICONTROL Create plan now]** （如果您想要產生具有預測ROI的AI建議計畫）。

     選取&#x200B;**[!UICONTROL OK]**。 您的計畫已建立。


   * 若要在建立具有預測投資報酬率的計畫之前編輯管道預算，請選取![表格編輯](/help/assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]**。

     選取「**[!UICONTROL OK]**」，以便在下一個步驟中定義您在&#x200B;**[!UICONTROL Spend selection]**&#x200B;中的管道支出。



1. 在&#x200B;**[!UICONTROL Spend selection]**&#x200B;區段中，針對每個預算日期範圍，使用![V形](/help/assets/icons/ChevronRight.svg)頂端開啟該資料範圍的管道分佈檢視。

   1. 若要定義每個管道的預算，請輸入&#x200B;**[!UICONTROL Min]**&#x200B;和&#x200B;**[!UICONTROL Max]**&#x200B;的值，或使用滑桿。

   1. 若要在貨幣或百分比輸入之間切換，請為&#x200B;**[!UICONTROL View spend by]**&#x200B;選取&#x200B;**[!UICONTROL $]**&#x200B;或&#x200B;**[!UICONTROL %]**。

      ![花費選取專案](/help/assets/plan-spend-selection.png)

   1. 完成後，選取&#x200B;**[!UICONTROL Create]**。

   1. 在&#x200B;**[!UICONTROL Create plan]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL Create plan]**&#x200B;以建立計畫。 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消計畫的建立。 顯示&#x200B;**[!UICONTROL No work is saved]**&#x200B;對話方塊以進行確認。
