---
title: 建置計畫
description: 瞭解如何在Mix Modeler中建置計畫。
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
source-git-commit: 498f50e4d1568e58d0ac2833022822340a5f6337
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---


# 建置計畫

在Mix Modeler中，您會使用計畫精靈來建立計畫。 在計畫精靈中，您可以設定詳細資訊和預算，或計畫的目標量度，以及用於計畫的基礎模型。 指定詳細資料、預算、目標量度和模型後，您就可以繼續進行AI建議的計畫或編輯依據管道的支出。 您可以選擇定義每個轉換的平均收入和管道成本的進階設定。

您必須定義要最大化計畫的目標。 此目標可以是您可花費的預算或您想要達成的目標。 如果目標是目標，則另外還需要指定要使用的目標量度的值：轉換、收入、CPA或ROI。

若要建立計畫，請在Mix Modeler的![PLan](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]**&#x200B;介面中選取&#x200B;**[!UICONTROL Create plan]**。


1. 在&#x200B;**[!UICONTROL Plan creation]**&#x200B;畫面中：

   1. 在&#x200B;**[!UICONTROL Setup]**&#x200B;區段中：

      1. 輸入&#x200B;**[!UICONTROL Plan name]**，例如`Goal based plan`。 輸入&#x200B;**[!UICONTROL Description]**，例如`A goal based plan`。
      1. 從&#x200B;**[!UICONTROL _中選取&#x200B;**[!UICONTROL Model]**選取選項……_.]**

         ![計畫設定](/help/assets/plan-setup.png)

   1. 在&#x200B;**[!UICONTROL Goal]**&#x200B;區段中，選取您要將計畫最佳化的目標。 您可以選取

      * **[!UICONTROL I have a budget to spend]**

        ![計畫預算](../assets/plan-budget.png)

        此選項可讓您為一個或多個日期範圍輸入預算。

         1. 在&#x200B;**[!UICONTROL Optimize]**&#x200B;容器中：
            1. 從&#x200B;**[!UICONTROL Select conversion]**&#x200B;下拉式功能表中選取轉換。
            1. 從&#x200B;**[!UICONTROL Select model]**&#x200B;下拉式功能表中選取模型。
         1. 透過輸入日期或使用![行事曆](/help/assets/icons/Calendar.svg)選取日期範圍來指定&#x200B;**[!UICONTROL Date range]**。
         1. 輸入&#x200B;**[!UICONTROL Budget]**。
若要新增其他日期範圍（每個日期範圍都有預算），請選取![行事曆新增](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**。
若要刪除日期範圍和相關預算，請選取![關閉](/help/assets/icons/Close.svg)。
         1. 若要定義您要在內限制計畫的選擇性最大預算，請執行下列步驟：
            1. 切換&#x200B;**[!UICONTROL Maximize budget]**&#x200B;開啟。
            1. 指定最大預算的金額。 金額應等於或高於為日期範圍指定的預算總金額。


      * **[!UICONTROL I have a target to achieve]** [!BADGE Beta]

        ![計畫目標](../assets/plan-target.png)

         1. 在&#x200B;**[!UICONTROL Optimize]**&#x200B;容器中
            1. 從&#x200B;**[!UICONTROL Select conversion]**&#x200B;下拉式功能表中選取轉換。
            1. 從&#x200B;**[!UICONTROL Select target metric]**&#x200B;下拉式功能表中選取目標量度。 您可以選取介於&#x200B;**[!UICONTROL Conversion]**、**[!UICONTROL CPA]**、**[!UICONTROL Revenue]**&#x200B;或&#x200B;**[!UICONTROL ROI]**&#x200B;之間。
            1. 從&#x200B;**[!UICONTROL Select model]**&#x200B;下拉式功能表中選取模型。
         1. 透過輸入日期或使用![行事曆](/help/assets/icons/Calendar.svg)選取日期範圍來指定日期範圍。
         1. 輸入所選目標量度的值。 例如，**[!UICONTROL Conversion]**&#x200B;的數字、**[!UICONTROL ROI]**&#x200B;的百分比，或&#x200B;**[!UICONTROL CPA]**&#x200B;和&#x200B;**[!UICONTROL Revenue]**的貨幣值。
若要新增其他日期範圍（每個日期範圍都有其目標量度），請選取![CalendarAdd](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**。
若要刪除日期範圍和相關聯的目標量度，請選取![關閉](/help/assets/icons/Close.svg)。
         1. 若要定義您要在內限制計畫的選擇性最大預算，請執行下列步驟：
            1. 切換&#x200B;**[!UICONTROL Maximize budget]**&#x200B;開啟。
            1. 指定最大預算的金額。


   1. 選擇「**[!UICONTROL Next]**」。

1. 在&#x200B;**[!UICONTROL Done with all required fields]**&#x200B;對話方塊：

   ![完成計畫](/help/assets/plan-done-required-fields.png)

   * 如果您想要產生具有預測ROI的AI建議計畫，請選取![NewPlan](/help/assets/icons/NewPlan.svg) **[!UICONTROL Create plan now]**。 選取&#x200B;**[!UICONTROL OK]**。 您的計畫已建立。





   * 如果您要在建立具有預測ROI的計畫之前編輯頻道預算並定義進階設定，請選取![表格編輯](/help/assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]**。  選取「**[!UICONTROL OK]**」，以便在下一個步驟中定義您在&#x200B;**[!UICONTROL Spend selection]**&#x200B;中的管道支出。


     >[!IMPORTANT]
     >
     >只有在您已選取![TableEdit](/help/assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]**&#x200B;時，以下資訊才相關


1. 在&#x200B;**[!UICONTROL Spend selection]**&#x200B;區段中，針對每個預算日期範圍，使用![V形](/help/assets/icons/ChevronRight.svg)開啟該資料範圍的管道分佈檢視。

   如果您想要使用過去的行銷支出資料和深入分析，可以使用歷史參考資料。 將歷史參考資料考慮在內：

   * 透過強調高績效管道和績效不佳的管道，改善預算分配。
   * 支援趨勢分析。
   * 在設定計畫時，找出有效策略並避免錯誤。

   如果您選取歷史參考期間，則需調整先前的支出模式偏好設定，而Mix Modeler的計畫功能可產生符合您期望的計畫。 這些計畫最終應能增強利害關係人的信心，確保行銷計畫是策略性的、高效的，並且這些計畫以證實的效能資料和業務需求為基礎。

   ![花費選取專案](/help/assets/plan-spend-selection.png)

   1. 選取 **[!UICONTROL Spend pattern]**。

      * 預設選項為&#x200B;**[!UICONTROL Automatic]**。
      * 選取「**[!UICONTROL Historical reference]**」並輸入&#x200B;**[!UICONTROL Start date]**，以參照已可供Mix Modeler使用的過去行銷支出資料。 **[!UICONTROL End date]**&#x200B;是根據您定義支出模式的日期範圍自動決定。 建議的開始日期是第一個可用的過去行銷支出日期。 若要表示您選取了不存在或無效的歷史參考期，您會看到![警示紅色](/help/assets/icons/AlertRed.svg)。

   1. 若要定義每個管道的預算，請輸入&#x200B;**[!UICONTROL Min]**&#x200B;和&#x200B;**[!UICONTROL Max]**&#x200B;的值，或使用滑桿。

   1. 若要在貨幣或百分比輸入之間切換，請為&#x200B;**[!UICONTROL View spend by]**&#x200B;選取&#x200B;**[!UICONTROL $]**&#x200B;或&#x200B;**[!UICONTROL %]**。 如果您選取的目標量度不是貨幣型量度，此切換功能會停用。

   1. 完成後，選取&#x200B;**[!UICONTROL Create]**。
      ![花費選取專案](/help/assets/plan-spend-selection.png)

   1. 選擇「**[!UICONTROL Next]**」。



1. 您可以在&#x200B;**[!UICONTROL Advanced configurations]**&#x200B;區段中輸入選用的進階組態。

   ![計畫摘要](../assets/plan-advanced-configurations.png)

   * 您的計畫名稱、模型、日期範圍和總預算已彙總起來。

   * 依預設，Mix Modeler會使用最新的歷史季節性資料，自動計算每次轉換的平均收入。 在&#x200B;**[!UICONTROL Average Revenue per conversion]**&#x200B;中，您可以定義每次轉換的特定平均收入。

      1. 針對預算中的每個日期範圍：

         1. 從&#x200B;**[!UICONTROL Date range]**&#x200B;下拉式功能表中選取日期範圍。
         1. 輸入&#x200B;**[!UICONTROL Average revenue]**&#x200B;值。

      1. 選取「![AddCircle](/help/assets/icons/AddCircle.svg)新增每個轉換單位的自訂平均收入」以新增日期範圍。
      1. 選取![RemoveCircle](/help/assets/icons/RemoveCircle.svg)以移除日期範圍。

     >[!NOTE]
     >
     >如果您的模型不包含歷史收入資料，則必須針對您為預算指定的每個日期範圍，定義每次轉換的平均收入。
     >

   * 依預設，Mix Modeler會使用最新的歷史季節性資料自動計算管道成本。 在&#x200B;**[!UICONTROL Channel costs]**&#x200B;中，您可以定義自訂管道成本。

      1. 針對模型中的各個管道，定義自訂管道成本。

         1. 從&#x200B;**[!UICONTROL Channel]**&#x200B;下拉式選單中選取頻道。
         1. 針對預算中的每個日期範圍：
            1. 從&#x200B;**[!UICONTROL Date range]**&#x200B;下拉式功能表中選取日期範圍。
            1. 輸入&#x200B;**[!UICONTROL Average revenue]**&#x200B;值。
         1. 選取![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom average revenue per conversion unit]**&#x200B;以新增日期範圍。
         1. 選取![RemoveCircle](/help/assets/icons/RemoveCircle.svg)以移除日期範圍。

      1. 選取![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom channel cost]**&#x200B;以新增頻道。
      1. 選取![CrossSize400](/help/assets/icons/CrossSize400.svg)以移除自訂頻道。


1. 完成後，選取&#x200B;**[!UICONTROL Create]**。

1. 在&#x200B;**[!UICONTROL Create plan]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL Create plan]**&#x200B;以建立計畫。 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消計畫的建立。 顯示&#x200B;**[!UICONTROL No work is saved]**&#x200B;對話方塊以進行確認。

