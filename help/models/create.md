---
title: 建立模型
description: 瞭解如何在Mix Modeler中建立模型。
feature: Models
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# 建立模型

若要建立模型，請在Mix Modeler的![模型](/help/assets//icons/FileData.svg) **[!UICONTROL Models]**&#x200B;介面中選取&#x200B;**[!UICONTROL Open model canvas]**。

為了建置您的自訂AI支援模型，介面會提供逐步引導模型設定流程。

1. 在&#x200B;**[!UICONTROL Setup]**&#x200B;步驟中：

   1. 輸入您的模型&#x200B;**[!UICONTROL Name]**，例如`Demo model`。 輸入&#x200B;**[!UICONTROL Description]**，例如`Demo model to explore AI featues of Mix Modeler`。

      ![模型名稱和描述](/help/assets//model-name-description.png)

   1. 選取&#x200B;**[!UICONTROL Next]**&#x200B;以繼續下一個步驟。 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消模型組態。

1. 在&#x200B;**[!UICONTROL Configure]**&#x200B;步驟中：

   1. 在&#x200B;**[!UICONTROL Conversion goal]**&#x200B;區段中的容器內：

      1. 輸入轉換的&#x200B;**[!UICONTROL Conversion name]**，例如`Conversion`

      1. 從&#x200B;**[!UICONTROL *選取協調欄位&#x200B;*]**選取轉換，其中包含您在[!UICONTROL Harmonized datasets]中定義為[轉換](../harmonize-data/conversions.md)一部分的可用轉換。 例如&#x200B;**[!UICONTROL Online Conversion]**。

      1. 您可以選取![回覆](/help/assets//icons/Reply.svg) **[!UICONTROL Create new conversion]**，直接從模型組態中建立轉換。

         ![模型 — 轉換步驟](/help/assets//model-conversion-step.png)

   1. 在「**[!UICONTROL Marketing touchpoints]**」區段中，您會看到數個行銷接觸點容器，這些容器對應於您在[!UICONTROL Harmonized datasets]中定義為[行銷接觸點](../harmonize-data/marketing-touchpoints.md)一部分的行銷接觸點。

      * 對於每個容器：

         1. 您可以修改&#x200B;**[!UICONTROL Marketing touchpoint name]**。

         1. 從&#x200B;**[!UICONTROL _選取行銷接觸點_]**&#x200B;選取行銷接觸點。

         1. 您可以選取![回覆](/help/assets//icons/Reply.svg) **[!UICONTROL Create new marketing touchpoint]**，以直接從模型設定中建立行銷接觸點。

      * 若要新增行銷接觸點容器，請選取![新增](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add marketing touchpoint]**。

      * 若要移除行銷接觸點容器，請在容器中選取「![更多](/help/assets//icons/More.svg)」，然後從內容功能表中選取「**[!UICONTROL Remove container]**」。

        ![模型 — 行銷接觸點 — 步驟](/help/assets//model-marketing-touchpoint-step.png)

   1. 根據預設，系統會針對您協調檢視中的所有資料產生一個分數。 若要僅對母體的子集評分，請使用&#x200B;**[!UICONTROL Eligible data population]**&#x200B;區段中的容器定義一或多個篩選器。

      * 針對每個容器，定義一或多個事件。

         1. 針對每個事件：

            1. 從&#x200B;**[!UICONTROL _選取協調欄位_]**&#x200B;中選取量度或維度。

            1. 選取適當的運運算元： **[!UICONTROL equals]**、**[!UICONTROL not equals]**、**[!UICONTROL less than]**、**[!UICONTROL greater than]**、**[!UICONTROL starts with]**、**[!UICONTROL doesn't start with]**、**[!UICONTROL ends with]**、**[!UICONTROL doesn't end with]**、**[!UICONTROL contains]**、**[!UICONTROL doesn't contain]**、**[!UICONTROL is in]**&#x200B;或&#x200B;**[!UICONTROL is not in]**。

            1. 在&#x200B;**[!UICONTROL _輸入或選取值_]**。

         1. 若要在容器中新增其他事件，請選取![新增](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add event]**。

         1. 若要從容器移除事件，請選取![關閉](/help/assets//icons/Close.svg)。

         1. 若要使用容器中定義的所有或多個事件進行篩選，請選取&#x200B;**[!UICONTROL Any of]**&#x200B;或&#x200B;**[!UICONTROL All of]**。 標籤會相應地從&#x200B;**[!UICONTROL Include ... Or ...]**&#x200B;變更為&#x200B;**[!UICONTROL Include ... And ...]**。

      * 若要新增合格的資料母體容器，請選取![新增](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add eligible population]**。

      * 若要移除合格的資料母體容器，請在容器中選取![更多](/help/assets//icons/More.svg)，然後從內容功能表中選取&#x200B;**[!UICONTROL Remove marketing touchpoint]**。

        ![模型 — 合格的資料母體](/help/assets//model-eligible-data-population-step.png)

   1. 若要將包含外部因子的資料集新增至模型，請在&#x200B;**[!UICONTROL External factors dataset]**&#x200B;區段中使用一或多個容器。

      * 對於每個容器：

         1. 在&#x200B;**[!UICONTROL _輸入因子_]**&#x200B;輸入&#x200B;**[!UICONTROL Factor name]**。

         1. 從&#x200B;**[!UICONTROL _選取資料集_]**&#x200B;中選取資料集。 您可以選取![資料](/help/assets//icons/Data.svg)來管理資料集。 如需詳細資訊，請參閱[資料集](../ingest-data/datasets.md)。

      * 若要新增其他外部因素資料集容器，請選取![新增](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add external factor]**。

      * 若要移除外部因子資料集容器，請在容器中選取![更多](/help/assets//icons/More.svg)，然後從內容功能表中選取&#x200B;**[!UICONTROL Remove external factor]**。

        ![模型 — 外部因素資料集](/help/assets//model-external-factors-dataset-step.png)


   1. 若要將包含內部因子的資料集新增至模型，請在&#x200B;**[!UICONTROL Internal factors dataset]**&#x200B;區段中使用一或多個容器。

      * 對於每個容器：

         1. 在&#x200B;**[!UICONTROL _輸入因子_]**&#x200B;輸入&#x200B;**[!UICONTROL Factor name]**。

         1. 從&#x200B;**[!UICONTROL _選取資料集_]**&#x200B;中選取資料集。 您可以選取![資料](/help/assets//icons/Data.svg)來管理資料集。 如需詳細資訊，請參閱[資料集](../ingest-data/datasets.md)。

      * 若要新增其他內部因子資料集容器，請選取![新增](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add internal factor]**。

      * 若要移除其他內部因子資料集容器，請在容器中，從內容功能表選取![更多](/help/assets//icons/More.svg)和&#x200B;**[!UICONTROL Remove internal factor]**。

        ![模型 — 內部因素資料集](/help/assets//model-internal-factors-dataset-step.png)

   1. 若要定義模型的回顧期間，請在&#x200B;**[!UICONTROL Give contribution credit to touchpoints occurring within]**&#x200B;中輸入介於`1`到`52`之間的值…… **[!UICONTROL weeks prior to the conversion]**。

   1. 選取&#x200B;**[!UICONTROL Next]**&#x200B;以繼續下一個步驟。 如果需要更多組態，紅色外框和文字會說明需要哪些額外組態。 <br/>選取&#x200B;**[!UICONTROL Back]**&#x200B;以返回上一步。 <br/>選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消模型組態。

1. 在&#x200B;**[!UICONTROL Advanced]**&#x200B;步驟中：

   1. 在&#x200B;**[!UICONTROL Define training window]**&#x200B;區段中，選取

      * **[!UICONTROL Have Mix Modeler select a helpful training window]**&#x200B;和

      * **[!UICONTROL Manually input a training window]**。選取時，在&#x200B;**[!UICONTROL Include events the following years prior to a conversion]**&#x200B;中定義年數。

        ![模型 — 定義訓練時段](/help/assets//model-define-training-window.png)

   1. 在&#x200B;**[!UICONTROL Spend share]**&#x200B;區段中：

      * 若要在行銷資料稀疏時使用歷史行銷投資比率來通知模型，請啟動&#x200B;**[!UICONTROL Allow spend share]**。

   1. 在&#x200B;**[!UICONTROL Prior knowledge]**&#x200B;區段中：

      1. 選取 **[!UICONTROL Rule type]**。

      1. 使用&#x200B;**[!UICONTROL Contribution proportion]**&#x200B;欄，為&#x200B;**[!UICONTROL Name]**&#x200B;底下列出的任何管道指定貢獻百分比。

      1. 您可以視情況為每個管道新增&#x200B;**[!UICONTROL Level of confidence]**&#x200B;百分比。

      1. 必要時，請使用&#x200B;**[!UICONTROL Clear all]**&#x200B;清除&#x200B;**[!UICONTROL Contribution proportion]**&#x200B;與&#x200B;**[!UICONTROL Level of confidence]**&#x200B;欄的所有輸入值。

         ![模型 — 先前知識](/help/assets//model-prior-knowledge-step.png)

1. 選取&#x200B;**[!UICONTROL Finish]**&#x200B;以完成模型設定。

   * 在&#x200B;**[!UICONTROL Create instance?]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL Ok]**&#x200B;以立即觸發第一組訓練和評分回合。 您的模型已列出，狀態為<span style="color:orange">●</span> **[!UICONTROL Awaiting training]**。

     選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消。

   * 如果需要更多組態，紅色外框和文字會說明需要哪些額外組態。

   選取&#x200B;**[!UICONTROL Back]**&#x200B;以返回上一步。

   選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消模型組態。
