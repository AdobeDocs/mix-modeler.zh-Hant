---
title: 在Mix Modeler中建立模型
description: 瞭解如何在Mix Modeler中建立模型，包括如何設定、設定和指定模型的進階選項。 例如轉換目標、接觸點、Adstock和排程。
feature: Models
solution: Mix Modeler
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
source-git-commit: 7836e378a0f9068fc868dcede0ab8b3e2803776a
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 2%

---

# 建立模型

為了建置您的自訂AI支援模型，介面會提供逐步引導模型設定流程。

在[!DNL Mix Modeler]的![模型](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;介面中，選取&#x200B;**[!UICONTROL Open model canvas]**。

## 設定

您在&#x200B;**[!UICONTROL Setup]**&#x200B;步驟中定義名稱和說明：

1. 輸入您的模型&#x200B;**[!UICONTROL Name]**，例如`Demo model`。 輸入&#x200B;**[!UICONTROL Description]**，例如`Demo model to explore AI features of Mix Modeler`。

   ![模型名稱和描述](/help/assets/model-name-description.png)

1. 選取&#x200B;**[!UICONTROL Next]**&#x200B;以繼續下一個步驟。 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消模型組態。

## 設定 {#configure}

>[!CONTEXTUALHELP]
>id="model_marketingtouchpoints_select"
>title="行銷接觸點"
>abstract="行銷接觸點為收件者、個體和/或 cookie 層級的行銷事件，用於評估行銷投資對數值型或收入型轉換的影響。<br/><br/>您無法使用具有重疊資料的接觸點來設定模型，而且必須至少有一個具有花費的接觸點。"


您在&#x200B;**[!UICONTROL Configure]**&#x200B;步驟中設定您的模型。 設定涉及轉換目標的定義、行銷接觸點、合格的資料母體、外部和內部因素等。

1. 在&#x200B;**[!UICONTROL Conversion goal]**&#x200B;區段中：

   ![模型 — 轉換步驟](/help/assets/model-conversion-step.png)

   1. 從&#x200B;**[!UICONTROL Conversion]**&#x200B;下拉式功能表中選取轉換。 可用的轉換是您在[!UICONTROL Harmonized datasets]中定義為[轉換](../harmonize-data/conversions.md)一部分的轉換。 例如 **[!UICONTROL Online Conversion]**。

   1. 您可以選取![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a conversion]**，直接從模型組態中建立轉換。



1. 在「**[!UICONTROL Marketing touchpoints]**」區段中，您可以選取一或多個行銷接觸點，對應至您在[!UICONTROL Harmonized datasets]中定義為[行銷接觸點](../harmonize-data/marketing-touchpoints.md)一部分的行銷接觸點。


   ![模型 — 行銷接觸點步驟](/help/assets/model-marketing-touchpoint-step.png)

   1. 從&#x200B;**[!UICONTROL Touchpoint include]**&#x200B;下拉式功能表中選取一或多個行銷接觸點。

      * 您可以使用![CrossSize75](/help/assets/icons/CrossSize75.svg)移除接觸點。
      * 您可以使用&#x200B;**[!UICONTROL Clear all]**&#x200B;移除所有接觸點。

   1. 您可以選取![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a touchpoint]**，以直接從模型設定中建立行銷接觸點。

   >[!NOTE]
   >
   >您無法使用具有重疊資料的接觸點來設定模型，而且必須至少有一個具有花費的接觸點。

1. 根據預設，系統會針對您協調檢視中的所有資料產生一個分數。 若要僅對母體的子集評分，請使用&#x200B;**[!UICONTROL Eligible data population]**&#x200B;區段中的容器定義一或多個篩選器。

   ![模型 — 合格的資料母體](/help/assets/model-eligible-data-population-step.png)

   * 針對每個容器，定義一或多個事件。

      1. 針對每個事件：

         1. 從&#x200B;**[!UICONTROL _選取協調欄位_]**&#x200B;中選取量度或維度。

         1. 選取適當的運運算元： **[!UICONTROL equals]**、**[!UICONTROL not equals]**、**[!UICONTROL less than]**、**[!UICONTROL greater than]**、**[!UICONTROL starts with]**、**[!UICONTROL doesn't start with]**、**[!UICONTROL ends with]**、**[!UICONTROL doesn't end with]**、**[!UICONTROL contains]**、**[!UICONTROL doesn't contain]**、**[!UICONTROL is in]**&#x200B;或&#x200B;**[!UICONTROL is not in]**。

         1. 在&#x200B;**[!UICONTROL _輸入或選取值_]**。

      1. 若要在容器中新增其他事件，請選取![新增](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add event]**。

      1. 若要從容器移除事件，請選取![關閉](/help/assets/icons/CrossSize75.svg)。

      1. 若要使用容器中定義的所有或多個事件進行篩選，請選取&#x200B;**[!UICONTROL Any of]**&#x200B;或&#x200B;**[!UICONTROL All of]**。 標籤會相應地從&#x200B;**[!UICONTROL Include ... Or ...]**&#x200B;變更為&#x200B;**[!UICONTROL Include ... And ...]**。

   * 若要新增合格的資料母體容器，請選取![新增](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add eligible population]**。

   * 若要移除合格的資料母體容器，請在容器中選取![更多](/help/assets/icons/More.svg)，然後從內容功能表中選取&#x200B;**[!UICONTROL Remove container]**。

   * 在容器之間選取&#x200B;**And**&#x200B;和&#x200B;**Or**，為您的合格資料母體建置更複雜的定義。

1. 您可以在&#x200B;**[!UICONTROL Factor dataset]**&#x200B;區段中管理包含內部或外部因子的資料集。

   ![模型 — 因素資料集步驟](../assets/model-factors-dataset-step.png)

   * 若要新增因子資料集，請選取&#x200B;**[!UICONTROL Add Factor]**。 您最多可以新增30個因子至模型。

      1. 從下拉式功能表中選取&#x200B;**[!UICONTROL Factor dataset]**。 可用的因子是您已在[資料集規則](/help/harmonize-data/dataset-rules.md#create-a-dataset-rule)中定義協調欄位的因子。
根據選取的資料集，**[!UICONTROL Factor type]**&#x200B;為&#x200B;**[!UICONTROL Internal]**&#x200B;或&#x200B;**[!UICONTROL External]**。

      1. 從下拉式功能表中選取&#x200B;**[!UICONTROL Impact on conversion]**。 可用的選項包括： **[!UICONTROL Auto]**、**[!UICONTROL Positive]**&#x200B;或&#x200B;**[!UICONTROL Negative]**。 預設選項為&#x200B;**[!UICONTROL Auto]**，可讓模型判斷因子資料集的影響。

   * 若要刪除因子資料集，請選取![CrossSize200](/help/assets/icons/CrossSize400.svg)。


1. 若要定義模型的回顧期間，請在&#x200B;**[!UICONTROL Define lookback window]**&#x200B;區段的&#x200B;**[!UICONTROL Give contribution credit to touchpoints occurring within]** ... **[!UICONTROL weeks prior to the conversion]**&#x200B;中輸入介於`1`到`52`之間的值。

1. 若要定義模型的訓練時段，請在&#x200B;**[!UICONTROL Define training window]**，選取您要開始評分轉換的位置。

   ![模型 — 定義訓練時段](/help/assets/model-define-training-window.png)

   您可以選取：

   * **[!UICONTROL Have Mix Modeler select a helpful training window]**&#x200B;和

   * **[!UICONTROL Manually input a training window]**. 選取時，在&#x200B;**[!UICONTROL Include events the following years prior to a conversion]**&#x200B;中定義年數。

   模型需要此輸入。 年數決定您可以在&#x200B;**[!UICONTROL Advanced]**&#x200B;步驟中設定的管道adstock上限方式。

1. 選取&#x200B;**[!UICONTROL Next]**&#x200B;以繼續下一個步驟。 如果需要更多組態，紅色外框和文字會說明需要哪些額外組態。 <br/>選取&#x200B;**[!UICONTROL Back]**&#x200B;以返回上一步。 <br/>選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消模型組態。


## 進階 {#advanced}

>[!CONTEXTUALHELP]
>id="model_advanced_channeladstock"
>title="管道Adstock"
>abstract="將領域專業知識、實驗結果或先前的管道分析直接整合到模型設定中。 Adstock設定有助於引導模型符合現實世界的期望，並改善輸出的可解性和可信度。 每個管道的回顧周數加上延遲周數總計的上限為設定培訓時段的八分之一。 此上限允許模型有足夠資料來瞭解Adstock效果。"

您可以在&#x200B;**[!UICONTROL Advanced]**&#x200B;步驟中指定進階設定。 在此步驟中，您可以定義[支出共用](#spend-share)、啟用[多重接觸歸因(MTA)](#mta)的模型、定義[先前知識](#prior-knowledge)以及定義[管道adstock](#channel-adstock)。

### 支出共用

在&#x200B;**[!UICONTROL Spend share]**&#x200B;區段中：

* 若要在行銷資料稀疏時使用歷史行銷投資比率來通知模型，請啟動&#x200B;**[!UICONTROL Allow spend share]**。 建議使用此設定，尤其是在下列情況下：
   * 管道沒有足夠的觀察值（例如支出、曝光或點按頻率低）。
   * 您正在模型化尖峰但一般且可能高花費的媒體（例如某些品牌的電視節目），這些媒體中的資料可能會很稀疏。

  >[!NOTE]
  >
  >對於一次性投資（例如超級碗廣告），將該資料納入為因素，而不是依賴支出份額。
  >

### MTA

在&#x200B;**[!UICONTROL MTA enabled]**&#x200B;區段中：

* 若要啟用模型的MTA功能，請啟動&#x200B;**[!UICONTROL MTA enabled]**。 如果您已啟用MTA，則在您已訓練並評分您的模型後，即可使用多重接觸歸因深入分析。 檢視[模型深入分析](insights.md)中的[歸因](insights.md#attribution)索引標籤。


### 先前知識

在&#x200B;**[!UICONTROL Prior knowledge]**&#x200B;區段中：

![模型 — 先前知識](/help/assets/model-prior-knowledge-step.png)

1. 選取&#x200B;**[!UICONTROL Rule type]**，預設為&#x200B;**[!UICONTROL Absolute values]**。

1. 使用&#x200B;**[!UICONTROL Contribution proportion]**&#x200B;欄，為&#x200B;**[!UICONTROL Name]**&#x200B;底下列出的任何管道指定貢獻百分比。

1. 您可以視情況為每個管道新增&#x200B;**[!UICONTROL Level of confidence]**&#x200B;百分比。

1. 必要時，請使用&#x200B;**[!UICONTROL Clear all]**&#x200B;清除&#x200B;**[!UICONTROL Contribution proportion]**&#x200B;與&#x200B;**[!UICONTROL Level of confidence]**&#x200B;欄的所有輸入值。


### 管道Adstock

在&#x200B;**[!UICONTROL Channel adstock]**&#x200B;區段中，您可以針對您在模型中定義的每個管道（行銷管道），定義個別Adstock回顧（結轉或衰減效果）和延遲（延遲回應時間）。

此管道Adstock設定可讓您更精確地控制不同行銷管道如何隨著時間影響業務結果。 或者，您也可以使用系統預設值和「一刀切」組態。

頻道adstock設定可協助您擷取頻道特有的細微差別。 例如，電視促銷活動的長期影響、付費搜尋的短期影響，或影響者支出與可觀察的轉換之間的延遲。 使用Adstock回顧和延遲引數來實驗，產生更準確、量身打造且值得信賴的深入分析。 最終，管道Adstock設定可帶來更精確的預算分配和更好的業務決策。

![管道adstock](/help/assets/channel-ad-stock.png)

若要設定頻道Adstock：

* 對於每個管道(**[!UICONTROL Name]**)，定義&#x200B;**[!UICONTROL Lag (weeks)]**、**[!UICONTROL Min Lookback (weeks)]**&#x200B;和&#x200B;**[!UICONTROL Max Lookback (weeks)]**&#x200B;值。 針對每個值：

   * 使用![加](/help/assets/icons/Add.svg)增加值，![減](/help/assets/icons/Subtract.svg)減少值，或手動輸入值。

  每個管道的延遲周數加回顧周數上限為設定培訓時段的八分之一。 此上限允許模型有足夠資料來瞭解Adstock效果。 例如，對於兩年的訓練期間，管道的&#x200B;**[!UICONTROL Lag (weeks)]**&#x200B;和&#x200B;**[!UICONTROL Lookback (weeks)]**&#x200B;的上限為13週。 此上限會在您定義值時強制執行。


## 設定選項

您可以[排程訓練和評分](#schedule)，並在&#x200B;**[!UICONTROL Set options]**&#x200B;步驟中為您的模型指定[精細見解報告欄位](#granular-insights-reporting-fields)。


### 排程

在&#x200B;**[!UICONTROL Schedule]**&#x200B;區段中，您可以排程模型訓練和評分。

![排程模型](../assets/model-schedule.png)

若要排程模型評分與訓練，請執行下列步驟：

1. 開啟&#x200B;**[!UICONTROL Enable scheduled model scoring and training]**。
1. 選取&#x200B;**[!UICONTROL Scoring frequency]**：

   * **[!UICONTROL Daily]**：輸入有效的時間（例如`05:22 pm`）或使用![時鐘](/help/assets/icons/Clock.svg)來定義時間。
   * **[!UICONTROL Weekly]**：選取一週的某天，然後輸入有效的時間（例如`05:22 pm`），或使用![時鐘](/help/assets/icons/Clock.svg)來定義時間。
   * **[!UICONTROL Monthly]**：從[在每個下拉式功能表上執行]選取一個月的某天，並輸入有效的時間（例如`05:22 pm`），或使用![時鐘](/help/assets/icons/Clock.svg)來定義時間。

1. 從下拉式功能表中選取&#x200B;**[!UICONTROL Training frequency]**： **[!UICONTROL Monthly]**、**[!UICONTROL Quarterly]**、**[!UICONTROL Yearly]**&#x200B;或&#x200B;**[!UICONTROL None]**。


### 精細見解報告欄位

**[!UICONTROL Granular insights reporting fields]**&#x200B;區段使用精細的增量報表功能。 此功能可讓您選取協調的欄位，以劃分轉換和接觸點增量分數。

![定義精細的深入分析報表欄位](/help/assets/granular-insights-reporting-fields.png)

您可以定義這些協調欄位，以便使用精細的報表欄在模型的報表中深入研究，而不必建立個別模型。

例如，您建立的模型著重於收入，但您也會對行銷活動、媒體型別、地區和流量來源績效感興趣。 如果沒有精細的增量報表功能，您必須建立四個個別的模型。 使用細微的增量報告功能，您可以根據行銷活動、媒體型別、地區和流量來源來劃分收入模型。

1. 從&#x200B;**[!UICONTROL Includes]**&#x200B;底下的&#x200B;**[!UICONTROL _選取協調欄位_]**&#x200B;中，選取一或多個協調欄位。 選取的協調欄位會新增至面板。
1. 選取&#x200B;**[!UICONTROL *協調欄位&#x200B;*]**![CrossSize100](/help/assets/icons/CrossSize100.svg)，以從包含所選協調欄位的容器中移除協調欄位。
1. 選取&#x200B;**[!UICONTROL Clear all]**&#x200B;以移除所有選取的協調欄位。

為精細增量報告選取的協調欄位可作為Experience Platform [結構描述](/help/ingest-data/schemas.md)和[資料集](/help/ingest-data/datasets.md)的一部分，這些資料來自對模型計分。 在&#x200B;**[!UICONTROL conversionPassthrough]**&#x200B;和&#x200B;**[!UICONTROL touchpointPassthrough]**&#x200B;物件中可以找到精細見解報告欄位。

針對已啟用精細增量報告的模型，在結構描述中擷取conversionPassthrough和touchpointPassthrough物件的熒幕擷圖![&#128279;](/help/assets/schema-granular-insights-reporting.png)


## 完成

* 選取&#x200B;**[!UICONTROL Finish]**&#x200B;以完成您的模型設定。

   * 在&#x200B;**[!UICONTROL Create instance?]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL Ok]**&#x200B;以立即觸發第一組訓練和評分回合。 您的模型已列出，狀態為![StatusOrange](/help/assets/icons/StatusOrange.svg) **[!UICONTROL Awaiting training]**。

     選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消。

   * 如果需要更多組態，紅色外框和文字會說明需要哪些額外組態。

* 選取&#x200B;**[!UICONTROL Back]**&#x200B;以返回上一步。

* 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消模型組態。

