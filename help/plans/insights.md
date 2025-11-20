---
title: 計畫深入分析
description: 瞭解如何檢視計畫的深入分析以及在Mix Modeler中編輯計畫。
feature: Plans
exl-id: 91385595-284f-4fcb-b54b-9539905e552b
source-git-commit: 86b58717c3c8be183c70d1ceccf6f7c757303518
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 0%

---

# 計畫深入分析


在[!UICONTROL Plan insights]中建立您的計畫深入分析，顯示[!UICONTROL Model]、[!UICONTROL Data range]以及計畫所依據的[!UICONTROL Plan target]。


建立前瞻分析時，您會看到計畫的概覽，包括：

- 顯示計畫所依據之[!UICONTROL Model]、[!UICONTROL Data range]和[!UICONTROL Plan target]的標頭。
   - 如果您已定義目標型計畫，徽章會指出目標的狀態。可能的選項包括：

      - [!BADGE 目標可達成]{type=Positive}
      - [!BADGE 目標無法達成]{type=Negative}

   - 選取![V形箭號](/help/assets/icons/ChevronDown.svg) **[!UICONTROL Show more]**&#x200B;以顯示更多詳細資料。

- [[!UICONTROL Forecasted paid channel ROI]視覺效果](#forecasted-paid-channel-spend-and-roi)
- [[!UICONTROL Forecasted revenue]視覺效果](#forecasted-revenue)
- [[!UICONTROL Forecasted conversion]視覺效果](#forecasted-conversions)
- [[!UICONTROL Marginal channel return]視覺效果](#marginal-channel-return)
- 計畫[[!UICONTROL Data range breakdown]的](#date-range-breakdown)資料表，顯示資料行

   - Channel
   - ROI
   - CPA
   - 收入
   - 轉換目標
   - 支出

若要關閉介面，請選取&#x200B;**[!UICONTROL Close]**。

若要變更如何檢視您計畫的ROI，請在&#x200B;**[!UICONTROL X]**&#x200B;選取&#x200B;**[!UICONTROL &#x200B; %]**&#x200B;或&#x200B;**[!UICONTROL View ROI]**。

## 預測的付費管道支出和ROI

此視覺效果會根據模式、日期範圍和預算，顯示付費管道上預測支出和投資回報的散點圖。

![預測的付費管道支出和ROI視覺效果](../assets/overview-plan-forecasted-paid-channel-send-roi.png)


## 預測收入

此長條圖視覺效果會根據模式、日期範圍和預算，顯示管道的預計收入。

![預測的收入視覺效果](../assets/overview-plan-forecasted-revenue.png)


## 預測的轉換

此長條圖視覺效果會根據模型、日期範圍和預算，顯示管道的預測轉換。

![預測的轉換視覺效果](../assets/overview-plan-forecasted-conversions.png)


## 邊際管道退貨

此折線圖視覺效果顯示所選頻道的邊際回訪曲線，其中包含&#x200B;**[!UICONTROL Marginal break-even]**&#x200B;和&#x200B;**[!UICONTROL Return point]**&#x200B;的指標。 此視覺效果可協助您瞭解管道支出如何達到邊際收支平衡點。 您是否有空間增加在管道上的支出，或是應該減少在管道上的支出，以提高管道的支出效率。

![邊際管道回報視覺效果](../assets/overview-plan-marginal-channel-return.png)

若要選取視覺效果的特定管道，請從「**[!UICONTROL View]**」下拉式選單中選取管道。

## 通路協同效應

管道協同效應矩陣可協助您識別行銷管道如何互動，除了個別貢獻外，還能產生乘數效應。

![計畫通路協同效應](/help/assets/plan-channel-synergies.png)

若要下載代表矩陣的CSV檔案，請選取![下載](/help/assets/icons/Download.svg) **[!UICONTROL Download]**。

## 日期範圍劃分

[!UICONTROL Date range breakdown]表格顯示[!UICONTROL ROI]、[!UICONTROL Revenue]、[!UICONTROL CPA]、[!UICONTROL Conversions]和[!UICONTROL Spend]的每個管道的詳細精細資料。

![日期範圍劃分表格](../assets/overview-plan-date-range-breakdown.png)

1. 若要下載包含日期範圍劃分資料的CSV檔案，請選取![下載](/help/assets/icons/Download.svg) **[!UICONTROL Download CSV]**。 從內容功能表：

   - 針對CSV格式的詳細資料選取![下載](/help/assets/icons/Download.svg) **[!UICONTROL Detailed CSV]**。
   - 針對CSV格式的摘要資料選取![下載](/help/assets/icons/Download.svg) **[!UICONTROL Summary CSV]**。

   詳細資料是按周劃分鍵的精細資料。 摘要資料是以模型提供的日期範圍作為關鍵字的資料。

1. 若要依管道類別檢視日期範圍劃分，請從&#x200B;**[!UICONTROL All channels]**&#x200B;選項中選取&#x200B;**[!UICONTROL Paid channels]**、**[!UICONTROL Non-paid channels]**&#x200B;或&#x200B;**[!UICONTROL View]**。


## 編輯計畫

若要編輯計畫，請選取![編輯](/help/assets/icons/Edit.svg) **[!UICONTROL Edit plan]**。

1. 在&#x200B;**[!UICONTROL Spend selection]**&#x200B;區段中，針對每個預算日期範圍，使用![V形](/help/assets/icons/ChevronRight.svg)開啟該資料範圍的管道分佈檢視。

   如果您想要使用過去的行銷支出資料和深入分析，可以使用歷史參考資料。 將歷史參考資料考慮在內：

   - 透過強調高績效管道和績效不佳的管道，改善預算分配。
   - 支援趨勢分析。
   - 在設定計畫時，找出有效策略並避免錯誤。

   如果您選取歷史參考期間，則需調整先前的支出模式偏好設定，而Mix Modeler的計畫功能可產生符合您期望的計畫。 這些計畫最終應能增強利害關係人的信心，確保行銷計畫是策略性的、高效的，並且這些計畫以證實的效能資料和業務需求為基礎。

   ![花費選取專案](/help/assets/plan-spend-selection.png)

   1. 選取 **[!UICONTROL Spend pattern]**。

      - 預設選項為&#x200B;**[!UICONTROL Automatic]**。
      - 選取「**[!UICONTROL Historical reference]**」並輸入&#x200B;**[!UICONTROL Start date]**，以參照已可供Mix Modeler使用的過去行銷支出資料。 **[!UICONTROL End date]**&#x200B;是根據選取的資料範圍自動決定。 建議的開始日期是第一個可用的過去行銷支出資料。 若要指出您已選取不存在的歷史參考期，您會看到![警示紅色](/help/assets/icons/AlertRed.svg)。


   1. 若要修改每個管道的預算，請修改&#x200B;**[!UICONTROL Min]**&#x200B;和&#x200B;**[!UICONTROL Max]**&#x200B;的值，或使用滑桿。

   1. 若要在貨幣或百分比輸入之間切換，請為&#x200B;**[!UICONTROL $]**&#x200B;選取&#x200B;**[!UICONTROL %]**&#x200B;或&#x200B;**[!UICONTROL View spend by]**。

   1. 若要編輯計畫的詳細資料，請選取&#x200B;**[!UICONTROL Edit details]**：

      1. 在&#x200B;**[!UICONTROL Setup]**&#x200B;區段中：

         1. 輸入&#x200B;**[!UICONTROL Plan name]**，例如`Demo plan`。 輸入&#x200B;**[!UICONTROL Description]**，例如`Demo plan for Luma company`。
         1. 從&#x200B;**[!UICONTROL Model]**&#x200B;中選取&#x200B;**[!UICONTROL _選取選項……_.]**

            ![計畫設定](/help/assets/plan-setup.png)

      1. 在&#x200B;**[!UICONTROL Goal]**&#x200B;區段中，選取您要將計畫最佳化的目標。 您可以選取
         - **[!UICONTROL I have a budget to spend]**

           ![計畫預算](../assets/plan-budget.png)

           此選項可讓您為一個或多個日期範圍輸入預算。

            1. 在&#x200B;**[!UICONTROL Optimize]**&#x200B;容器中：
               1. 從&#x200B;**[!UICONTROL Select conversion]**&#x200B;下拉式功能表中選取轉換。
               1. 從&#x200B;**[!UICONTROL Select model]**&#x200B;下拉式功能表中選取模型。
            1. 透過輸入日期或使用&#x200B;**[!UICONTROL Date range]**&#x200B;行事曆![選取日期範圍來指定](/help/assets/icons/Calendar.svg)。
            1. 輸入&#x200B;**[!UICONTROL Budget]**。
若要新增其他日期範圍（每個日期範圍都有預算），請選取![行事曆新增](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**。
若要刪除日期範圍和相關預算，請選取![關閉](/help/assets/icons/Close.svg)。
            1. 若要定義您要在內限制計畫的選擇性最大預算，請執行下列步驟：
               1. 切換&#x200B;**[!UICONTROL Maximize budget]**&#x200B;開啟。
               1. 指定最大預算的金額。 金額應等於或高於為日期範圍指定的預算總金額。


         - **[!UICONTROL I have a target to achieve]** [!BADGE Beta]

           ![計畫目標](../assets/plan-target.png)

            1. 在&#x200B;**[!UICONTROL Optimize]**&#x200B;容器中
               1. 從&#x200B;**[!UICONTROL Select conversion]**&#x200B;下拉式功能表中選取轉換。
               1. 從&#x200B;**[!UICONTROL Select target metric]**&#x200B;下拉式功能表中選取目標量度。 您可以選取介於&#x200B;**[!UICONTROL Conversion]**、**[!UICONTROL CPA]**、**[!UICONTROL Revenue]**&#x200B;或&#x200B;**[!UICONTROL ROI]**&#x200B;之間。
               1. 從&#x200B;**[!UICONTROL Select model]**&#x200B;下拉式功能表中選取模型。
            1. 透過輸入日期或使用![行事曆](/help/assets/icons/Calendar.svg)選取日期範圍來指定日期範圍。
            1. 輸入所選目標量度的值。 例如，**[!UICONTROL Conversion]**&#x200B;的數字、**[!UICONTROL ROI]**&#x200B;的百分比，或&#x200B;**[!UICONTROL CPA]**&#x200B;和&#x200B;**[!UICONTROL Revenue]**&#x200B;的貨幣值。
若要新增其他日期範圍（每個日期範圍都有其目標量度），請選取![CalendarAdd](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**。
若要刪除日期範圍和相關聯的目標量度，請選取![關閉](/help/assets/icons/Close.svg)。
            1. 若要定義您要在內限制計畫的選擇性最大預算，請執行下列步驟：
               1. 切換&#x200B;**[!UICONTROL Maximize budget]**&#x200B;開啟。
               1. 指定最大預算的金額。

         1. 選取&#x200B;**[!UICONTROL Next]**&#x200B;以返回&#x200B;**[!UICONTROL Spend selection]**&#x200B;區段。

1. 在&#x200B;**[!UICONTROL Advanced configuration]**&#x200B;區段中：

   ![編輯進階設定](../assets/edit-plan-advanced-configuration.png)

   - 您的計畫名稱、模型、日期範圍和總預算已彙總起來。

   - 依預設，Mix Modeler會使用最新的歷史季節性資料，自動計算每次轉換的平均收入。 在&#x200B;**[!UICONTROL Average Revenue per conversion]**&#x200B;中，您可以定義每次轉換的特定平均收入。

   1. 針對預算中的每個日期範圍：
      1. 從&#x200B;**[!UICONTROL Date range]**&#x200B;下拉式功能表中選取日期範圍。
      1. 輸入&#x200B;**[!UICONTROL Average revenue]**&#x200B;值。
   1. 選取「![AddCircle](/help/assets/icons/AddCircle.svg)新增每個轉換單位的自訂平均收入」以新增日期範圍。
   1. 選取![RemoveCircle](/help/assets/icons/RemoveCircle.svg)以移除日期範圍。

   >[!NOTE]
   >
   >如果您的模型不包含歷史收入資料，則必須針對您為預算指定的每個日期範圍，定義每次轉換的平均收入。
   >

   - 依預設，Mix Modeler會使用最新的歷史季節性資料自動計算管道成本。 在&#x200B;**[!UICONTROL Channel costs]**&#x200B;中，您可以定義自訂管道成本。

   1. 針對模型中的各個管道，定義自訂管道成本。
      1. 從&#x200B;**[!UICONTROL Channel]**&#x200B;下拉式選單中選取頻道。
      1. 針對預算中的每個日期範圍：
         1. 從&#x200B;**[!UICONTROL Date range]**&#x200B;下拉式功能表中選取日期範圍。
         1. 輸入&#x200B;**[!UICONTROL Average revenue]**&#x200B;值。
      1. 選取![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom average revenue per conversion unit]**&#x200B;以新增日期範圍。
      1. 選取![RemoveCircle](/help/assets/icons/RemoveCircle.svg)以移除日期範圍。

   1. 選取![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom channel cost]**&#x200B;以新增頻道。
   1. 選取![CrossSize400](/help/assets/icons/CrossSize400.svg)以移除自訂頻道。


1. 當您完成計畫編輯時，請選取&#x200B;**[!UICONTROL Edit]**。

   在&#x200B;**[!UICONTROL All changes are final]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL OK]**&#x200B;以更新計畫的目前支出分配以及ROI和收入預測。 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消計畫的更新。


- 若要隨時取消計畫更新，請選取&#x200B;**[!UICONTROL Cancel]**。 在&#x200B;**[!UICONTROL No work will be saved]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以繼續處理您的計畫，或選取&#x200B;**[!UICONTROL OK]**&#x200B;以返回Plans介面。
- 若要返回精靈，請選取&#x200B;**[!UICONTROL Back]**。
