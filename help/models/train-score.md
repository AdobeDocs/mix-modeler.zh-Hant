---
title: 訓練模型並為其評分
description: 瞭解如何訓練模型並為其評分。
feature: Models
source-git-commit: 6855d19347b7f6f1477a6265310df5950b8463c9
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# 訓練模型並為其評分

在您[建立](/help/models/build.md)模型後，模型會自動接受訓練並評分。 您可以手動重新訓練或重新核心模型。

## 訓練

當您想要包含新的增量行銷和因子資料時，請考慮重新訓練模型。 例如，在上個季度，市場動態已變更，或您的行銷資料分佈已大幅變更。

若要重新訓練模型，請執行下列動作：

1. 從左側邊欄選取![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**。

1. 為模型選取![更多](/help/assets/icons/More.svg)，然後從內容功能表選取&#x200B;**[!UICONTROL Train]**。 或者，從藍色動作列選取![DataRefresh](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Train]**。

   在&#x200B;**[!UICONTROL Train model]**&#x200B;對話方塊中，選取選項以：

   * **[!UICONTROL Train model with last 2 years of marketing data]**，或
   * **[!UICONTROL Train model using specific date range of data]**。
指定日期範圍。 您可以使用![行事曆](/help/assets/icons/Calendar.svg)來選取日期範圍。 您至少必須選取一年內的資料範圍。

   ![重新訓練模型](../assets/retrain-model.png)

1. 選取&#x200B;**[!UICONTROL Train]**&#x200B;以重新訓練模型。


您只能在成功訓練模型時重新訓練模型。


## 分數


您可以根據新的行銷資料對模型遞增評分，或針對特定日期範圍重新核心模型。

當您想要執行下列動作時，請考慮重新核心模型：

* 更正不正確的行銷資料。 例如，您納入模型訓練和評分的最近付費搜尋資料遺漏了一週的資料。
* 使用新的增量行銷資料，這些資料已透過您設定為協調資料一部分的資料集更新而提供。

若要評分或重新核心模型：

1. 從左側邊欄選取![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**。

1. 為模型選取![更多](/help/assets/icons/More.svg)，然後從內容功能表選取&#x200B;**[!UICONTROL Score]**。 或者，從藍色動作列選取![DataRefresh](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Score]**。

   在&#x200B;**[!UICONTROL Score marketing data]**&#x200B;對話方塊中，選取選項以：

   * **[!UICONTROL Score new marketing data from *mm/dd/yyyy *]**，使用新的行銷資料逐步為您的模型評分，或
   * **[!UICONTROL Score specific date range of marketing data]**以針對特定日期範圍重新核心。
指定日期範圍。 您可以使用![行事曆](/help/assets/icons/Calendar.svg)來選取日期範圍。

   ![重新核心模型](../assets/rescore-model.png)

1. 選取&#x200B;**[!UICONTROL Score]**。 使用特定資料範圍重新評分模型時，您會看到&#x200B;**[!UICONTROL Existing model is replaced]**&#x200B;對話方塊，提示您確認以所選日期範圍的新分數取代模型。 選取&#x200B;**[!UICONTROL Replace model]**&#x200B;以確認。

>[!IMPORTANT]
>
>重新核心模型不會變更任何已根據重新核心模型建立的計畫。 若要在計畫中使用新的重新整理模型，您必須建立新計畫。

