---
title: 資料集規則
description: 瞭解如何定義資料集規則，以便用於協調Mix Modeler中的資料。
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---

# 資料集規則

資料集規則可協助您將協調的欄位與您在Mix Modeler中擷取的資料欄位進行對應。

* 對於您在Adobe Experience Platform中擷取的彙總資料，您可以將一個或多個可用的資料集欄位對應到適當的和諧欄位。
* 對於事件資料，您可以直接或使用條件，個別將一個或多個和諧的欄位對應到資料集中的欄位。


## 管理資料集規則

若要檢視可用資料集規則的表格，請在Mix Modeler介面中：

1. 從左側邊欄選取![資料搜尋](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]**。

1. 從頂端列選取&#x200B;**[!UICONTROL Dataset rules]**。 您會看到資料集規則的表格。

表格欄會指定資料集規則的詳細資料：

| 欄名稱 | 詳細資料 |
| ---------------------- | ----------|
| 資料集 | 資料集的名稱。 |
| 來源 | 資料集的來源： Adobe Analytics、體驗事件、摘要（彙總）或取用者體驗事件。 |
| 結構描述 | 資料集符合的結構描述。 您可以在![結構描述](/help/assets//icons/Schemas.svg) [結構描述](../ingest-data/schemas.md)的結構描述編輯器中，快速選取結構描述名稱以在新的索引標籤中開啟結構描述。 |
| 詳細程度 | 資料集中的資料粒度。 可能的值為每日、每週、每月或每年。 |
| 一週開始 | 針對特定資料集，指定將一週中的哪一天視為新一週的開始。 |
| 狀態 | 欄位的狀態： <p><span style="color:gray">●</span>草稿或 <p><span style="color:green">●</span>使用中 |
| 上次修改時間 | 上次修改資料集規則的資料和時間。 |

{style="table-layout:auto"}

### 建立資料集規則

若要建立資料集規則，請在Mix Modeler的![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]**&#x200B;介面中，選取&#x200B;**[!UICONTROL Dataset rules configuration]**&#x200B;精靈中的&#x200B;**[!UICONTROL Create a dataset rule]**。

在&#x200B;**[!UICONTROL Create]**&#x200B;畫面中，

1. 在&#x200B;**[!UICONTROL Dataset details]**&#x200B;中，從&#x200B;**[!UICONTROL Select dataset]**&#x200B;中選取資料集以開始設定。 在清單中，資料集分類為&#x200B;**[!UICONTROL Consumer Experience Events]**、**[!UICONTROL Adobe Analytics]**、**[!UICONTROL Experience Event]**&#x200B;和&#x200B;**[!UICONTROL Summary]**。

1. 選取&#x200B;**[!UICONTROL Start of the week]**&#x200B;的日期。

1. 選取&#x200B;**[!UICONTROL Granularity]**&#x200B;的&#x200B;**[!UICONTROL Daily]**、**[!UICONTROL Weekly]**、**[!UICONTROL Monthly]**&#x200B;或&#x200B;**[!UICONTROL Yearly]**。

1. 當您選取&#x200B;**[!UICONTROL Summary]**&#x200B;類別的資料集時：

   1. 若要定義資料集的資料是否彙總或取代現有資料，請為&#x200B;**[!UICONTROL Data restatement is by]**&#x200B;選取&#x200B;**[!UICONTROL Aggregation]**&#x200B;或&#x200B;**[!UICONTROL Replacement]**。

   1. 將每個&#x200B;**[!UICONTROL Available dataset fields]**&#x200B;對應至&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;中對應的&#x200B;**[!UICONTROL Standard harmonized fields]**。 如果您不想將資料集欄位對應到協調的欄位，請明確選取&#x200B;**[!UICONTROL -- None --]**。

   1. 如果您需要新的協調欄位，但無法從清單中取得，請選取&#x200B;**[!UICONTROL Create New]**&#x200B;以建立新的協調欄位。 您會看到對話方塊，如[新增協調欄位](fields.md#add-a-harmonized-field)中所列。

   1. 當規則的所有欄位對應完成時，請選取&#x200B;**[!UICONTROL Save as draft]**&#x200B;以儲存規則的草稿版本，或選取&#x200B;**[!UICONTROL Save]**&#x200B;以儲存並啟動規則。 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消規則設定。

      ![建立資料集規則](/help/assets//dataset-create-summary.png)

1. 當您在&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;下方的方塊中選取事件類別資料集(**[!UICONTROL Experience Events]**， **[!UICONTROL Adobe Analytics]**， **[!UICONTROL Consumer Experience Events]**)時：

   1. 從&#x200B;**[!UICONTROL Standard harmonized field]**&#x200B;中選取協調欄位。

   1. 當選取的協調欄位屬於型別量度時：

      1. 從&#x200B;**[!UICONTROL Mapping type]**&#x200B;中選取&#x200B;**[!UICONTROL Count]**&#x200B;或&#x200B;**[!UICONTROL Sum]**。

      1. 選取您預設要將協調欄位對應到的&#x200B;**[!UICONTROL *AEP資料集欄位&#x200B;*]**。

   1. 當選取的欄位屬於型別維度時：

      1. 從&#x200B;**[!UICONTROL Mapping type]**&#x200B;中選取&#x200B;**[!UICONTROL Map Into]**&#x200B;或&#x200B;**[!UICONTROL Case]**。

      1. 當您已選取&#x200B;**[!UICONTROL Map Into]**&#x200B;時，請選取&#x200B;**[!UICONTROL Field]**&#x200B;和&#x200B;**[!UICONTROL *AEP資料集欄位&#x200B;*]**或&#x200B;**[!UICONTROL Value]**，以及預設值，以將協調欄位依預設對應至資料集欄位或輸入的值。

      1. 當您選取&#x200B;**[!UICONTROL Case]**&#x200B;時，請選取&#x200B;**[!UICONTROL Field]**&#x200B;和&#x200B;**[!UICONTROL *AEP資料集欄位&#x200B;*]**或&#x200B;**[!UICONTROL Value]**，以及預設值，以將協調欄位依預設對應到資料集欄位或輸入的值。

         1. 若要明確設定值，您可以定義一或多個案例，由一或多個條件組成。 每個條件都可以檢查特定的&#x200B;**[!UICONTROL *AEP資料集欄位&#x200B;*]**，無論是它&#x200B;**[!UICONTROL Exists]**或&#x200B;**[!UICONTROL Not Exists]**，還是它&#x200B;**[!UICONTROL Contains]**、**[!UICONTROL Not Contains]**、**[!UICONTROL Equals]**、**[!UICONTROL Not Equals]**、**[!UICONTROL Starts With]**或&#x200B;**[!UICONTROL Ends With]**在**[!UICONTROL *&#x200B;輸入的值輸入值&#x200B;*]**。

         1. 若要新增其他案例，請選取![新增](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add case]**，若要新增其他條件，請選取![新增](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add condition]**。

         1. 若要刪除案例或條件，請選取對應容器中的![關閉](/help/assets//icons/Close.svg)。

         1. 若要選取任何或所有條件是否應該套用至案例，請選取&#x200B;**[!UICONTROL Any of]**&#x200B;或&#x200B;**[!UICONTROL All of]**。

         1. 若要設定案例的結果值，請在&#x200B;**[!UICONTROL Then]**&#x200B;輸入值。

      以下範例

      * 使用&#x200B;**[!UICONTROL Map Into]** **[!UICONTROL Mapping type]**&#x200B;將&#x200B;**[!UICONTROL Channel Type At Source]**&#x200B;協調欄位對應到&#x200B;**[!DNL Luma Transactions]**&#x200B;資料集中的&#x200B;**[!UICONTROL channel_type]**&#x200B;欄位。

      * 使用&#x200B;**[!UICONTROL Case]** **[!UICONTROL Mapping type]**&#x200B;有條件地將&#x200B;**[!DNL Luma Transactions]**&#x200B;資料集中的&#x200B;**[!UICONTROL marketing.campaignName]**&#x200B;欄位值對應到&#x200B;**[!UICONTROL Campaign]**&#x200B;協調欄位。 「行銷活動協調」欄位設為：

         * **[!UICONTROL marketing.campaignName]**&#x200B;為`_black_friday`或`BlackFriday`時的`Black Friday`。
         * 到所有其他情況下的&#x200B;**[!UICONTROL marketing.campaignName]**&#x200B;的值。

        ![資料集規則事件](/help/assets//dataset-create-event.png)

1. 選取![新增](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add field]**&#x200B;以定義其他欄位。

完成後，選取&#x200B;**[!UICONTROL Save as draft]**&#x200B;以儲存規則的草稿版本，或選取&#x200B;**[!UICONTROL Save]**&#x200B;以儲存並啟動規則。 選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消規則設定。


### 編輯資料集規則

若要編輯資料集規則，請在Mix Modeler的![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]**&#x200B;介面中：

1. 針對您要編輯的資料集規則，在&#x200B;**[!UICONTROL Dataset]**&#x200B;欄中選取![更多](/help/assets//icons/More.svg)。
1. 從內容功能表中，選取![編輯](/help/assets//icons/Edit.svg) **[!UICONTROL Edit]**&#x200B;以開始編輯資料集規則。 如需詳細資訊，請參閱[建立資料集規則](#create-a-dataset-rule)。


### 刪除資料集規則

若要刪除資料集規則，請在Mix Modeler的![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]**&#x200B;介面中：

1. 針對您要刪除的資料集規則，在&#x200B;**[!UICONTROL Dataset]**&#x200B;欄中選取![更多](/help/assets//icons/More.svg)。
1. 從內容功能表中，選取![刪除](/help/assets//icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;以刪除資料集規則。 系統會提示您進行確認。 選取&#x200B;**[!UICONTROL Delete]**&#x200B;以永久刪除選取的資料集規則。


## 同步資料

若要在調和的資料和摘要及/或事件資料集之間同步資料，請遵循資料集規則中的所有邏輯：

1. 選擇「**[!UICONTROL Sync data]**」。

1. 從&#x200B;**[!UICONTROL Sync data for dataset rules]**&#x200B;對話方塊中，選取
   * **[!UICONTROL Refresh harmonized data for summary datasets]**，
   * **[!UICONTROL Refresh harmonized data for event datasets]**，或
   * **[!UICONTROL Refresh harmonized data for both summary + event datasets]**。

1. 若要根據已定義的資料集規則，在資料集中的已協調資料和資料之間開始同步，請選取&#x200B;**[!UICONTROL Sync]**。 若要取消同步處理，請選取&#x200B;**[!UICONTROL Cancel]**。

   ![同步處理資料](/help/assets//sync-data.png)


## 資料合併偏好設定

>[!NOTE]
>
>[!BADGE beta]{type=Informative}

合併摘要資料和事件資料來源中的資料時，資料合併偏好設定可協助解決衝突。 使用案例包括：

* 在多個資料集中測量和報告相同的廣告量度，或
* 某些資料集中的量度測量可能不完整，而另一個資料集可能是特定量度的超集，導致重複計數。

為確保模型預測準確，您可以定義資料合併偏好設定：

1. 選取![資料合併偏好設定](/help/assets//icons/Merge.svg) [!BADGE beta]。

1. 在&#x200B;**[!UICONTROL Data merge preferences]** [!BADGE beta]中{type=Informative}

   ![資料合併喜好設定](/help/assets//data-merge-preferences.png)

   * 選取&#x200B;**[!UICONTROL Default metric preference]**。 在協調期間，當多個資料來源更新指定頻道的量度欄位時，會套用選取的預設量度偏好設定。 此偏好設定會套用至沙箱層級，除非根據特定量度的偏好設定加以覆寫。 您可以選取&#x200B;**[!UICONTROL Summary data]**、**[!UICONTROL Event data]**&#x200B;與&#x200B;**[!UICONTROL Sum of summmary and event data]**&#x200B;之間。

   * 若要新增特定量度型偏好設定：

      1. 選取![加](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add a metric]**。
         1. 從&#x200B;**[!UICONTROL *度量選擇&#x200B;*]**清單中選取度量。
         1. 選取&#x200B;**[!UICONTROL CHANNELS]**&#x200B;或&#x200B;**[!UICONTROL CONVERSION TYPES]**。 從清單中選取&#x200B;**[!UICONTROL All]**&#x200B;或特定的管道或轉換型別。
         1. 選取&#x200B;**[!UICONTROL Summary]**&#x200B;或&#x200B;**[!UICONTROL Event]**，以指定合併資料時，彙總資料或事件資料是否偏好量度（以及所有或選取的管道）。

         若要新增一或多個其他管道或轉換型別：

         1. 選取![加](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add a channel]**&#x200B;或![加](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add a conversion type]**。
         1. 選取「**[!UICONTROL Summary]**」或「**[!UICONTROL Event]**」。

         若要刪除管道或轉換型別，請選取![交叉](/help/assets//icons/Close.svg)。

      1. 若要新增更具體的量度型偏好設定，請重複上一步驟。

   * 若要刪除現有的特定量度型偏好設定，請選取![刪除](/help/assets//icons/Delete.svg)。

1. 選取&#x200B;**[!UICONTROL Save]**&#x200B;以儲存資料合併偏好設定。 已開始重新同步資料。 <br/>選取&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消。


## 欄位層級存取控制

設定協調資料集的資料集規則時，會在欄位層級上強制執行Experience Platform的[屬性型存取控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)。 當標籤附加至結構描述欄位並啟用拒絕您存取該欄位的作用中原則時，欄位會受到限制。 因此：

* 您沒有在建立資料集規則時看到為您限制的結構描述欄位。
* 您無法檢視或編輯一或多個限制您使用的結構描述欄位的對應。 當您編輯或檢視包含這類受限制欄位的資料集規則時，您會看到下列畫面。
  ![不允許的動作](/help/assets//action-not-permitted.png)
