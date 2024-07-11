---
title: 建立計畫
description: 瞭解如何在Mix Modeler中建立計畫。
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---


# 建立計畫

在Mix Modeler中，您可以使用計畫畫布建立計畫。 在計畫畫布中，您可以設定計畫的明細與預算，以及計畫要使用的基本模型。 一旦您指定了詳細資訊、預算和模型，您就可以繼續進行AI推薦的計畫或編輯依據管道的支出。

若要建立計畫，請在 ![PLan](/help/assets//icons/FileChart.svg) **[!UICONTROL Plans]** 介面中的Mix Modeler，選取 **[!UICONTROL Open plan canvas]**.

1. 在「計畫建立」畫面中：

   1. 在 **[!UICONTROL Setup]** 區段

      1. 輸入 **[!UICONTROL Plan name]**，例如 `Demo plan`. 輸入 **[!UICONTROL Description]**，例如 `Demo plan for Luma company`.
      1. 選取 **[!UICONTROL Model]** 從 **[!UICONTROL _選取一個選項……_.]**.
      1. 您可以選取 ![連結輸出](/help/assets//icons/LinkOut.svg) **[!UICONTROL Create model]** 從計畫建立中直接建立模型。 這會在您的瀏覽器中開啟新索引標籤，並顯示 [模型](../models/overview.md) 介面。

         ![計畫設定](/help/assets//plan-setup.png)

   1. 在 **[!UICONTROL Budget]** 區段：

      1. 輸入日期或使用以下方式選取日期範圍，以指定日期範圍 ![行事曆](/help/assets//icons/Calendar.svg).
      1. 輸入預算。

      若要新增其他日期範圍（每個日期範圍都有預算），請選取「 」 ![行事曆新增](/help/assets//icons/CalendarAdd.svg) **[!UICONTROL Add row]**.

      若要刪除日期範圍與相關的預算，請選取 ![關閉](/help/assets//icons/Close.svg).

      若要定義指定的最大預算，請執行下列步驟：

      1. 切換 **[!UICONTROL Maximize budget]** 開啟。
      1. 指定最大預算金額。 金額應等於或高於為日期範圍指定的預算總金額。

         ![計畫預算](/help/assets//plan-budget.png)

   1. 選擇「**[!UICONTROL Next]**」。

1. 在 **[!UICONTROL Done with all required fields]** 對話方塊：

   ![計畫完成](/help/assets//plan-done-required-fields.png)

   * 選擇 <img src="/help/assets//icons/NewPlan.svg" width="25" /> **[!UICONTROL Create plan now]** 如果您想要產生具有預測性ROI的AI建議計畫。

     選取 **[!UICONTROL OK]**. 您的計畫已建立。


   * 選取 ![表格編輯](/help/assets//icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]** 如果您想要在建立具有預測投資報酬率的計畫之前編輯管道預算。

     選取 **[!UICONTROL OK]**，以便您在中定義您的管道支出 **[!UICONTROL Spend selection]** 在下一個步驟中。



1. 在 **[!UICONTROL Spend selection]** 區段，針對每個預算日期範圍，使用 ![V形](/help/assets//icons/ChevronRight.svg) 頂端開啟該資料範圍的管道分佈檢視。

   1. 若要定義每個管道的預算，請輸入值 **[!UICONTROL Min]** 和 **[!UICONTROL Max]** 或使用滑桿。

   1. 若要在貨幣或百分比輸入之間切換，請選取 **[!UICONTROL $]** 或 **[!UICONTROL %]** 的 **[!UICONTROL View spend by]**.

      ![花費選取範圍](/help/assets//plan-spend-selection.png)

   1. 完成後，選取 **[!UICONTROL Create]**.

   1. 在 **[!UICONTROL Create plan]** 對話方塊，選取 **[!UICONTROL Create plan]** 以建立您的計畫。 選取 **[!UICONTROL Cancel]** 以取消計畫的建立。 A **[!UICONTROL No work is saved]** 對話方塊隨即顯示以確認。
