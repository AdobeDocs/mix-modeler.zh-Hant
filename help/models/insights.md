---
title: 模型深入分析
description: 瞭解如何取得有關您模型的詳細資訊，例如Mix Modeler中的歷史總覽、模型見解和模型品質。
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: 09ec757a37725d4b41231076bd99432bffd6d555
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 0%

---

# 模型深入分析

若要檢視模型深入分析，請在Mix Modeler的![模型](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;介面中：

1. 從&#x200B;**[!UICONTROL Models]**&#x200B;表格中，選取含有<span style="color:green">●</span>之&#x200B;**[!UICONTROL Last run status]**&#x200B;的模型名稱 **[!UICONTROL Success]**。

1. 從內容功能表中，選取&#x200B;**[!UICONTROL Model Insights]**。

![模型深入分析標籤列](/help/assets/model-insights-tabbar.png)

您會看到指定模型上次重新整理的時間，並使用四個索引標籤來顯示視覺效果： [模型深入分析](#model-insights)、[歸因](#attribution)、[因素](#factors)、[診斷](#diagnostics)以及[歷史總覽](#historical-overview)。

您可以變更每個標籤上的視覺效果所根據的日期期間。 輸入日期期間或選取![行事曆](/help/assets/icons/Calendar.svg)以選取日期期間。

## [!UICONTROL Model insights]

模型深入分析索引標籤會顯示[依日期和基本媒體所區分的貢獻](#contribution-by-date-and-base-media)、[依管道所區分的貢獻](#contribution-by-channel)、[行銷績效摘要](#marketing-performance-summary)以及[邊際回應曲線](#marginal-response-curves)的視覺效果。

![模型 — 模型深入分析](/help/assets/model-insights-insights.png)

* 您可以將滑鼠停留在每個視覺效果中的個別圖表元素上，以顯示包含更多詳細資訊的彈出視窗。

* 若要下載包含視覺效果資料的CSV檔案，請選取![下載](/help/assets/icons/Download.svg)。

* 若要以Microsoft® Excel格式下載完整的模型深入分析資料，請選取![下載](/help/assets/icons/Download.svg) **[!UICONTROL Download data]**。


### 依日期和基本媒體所區分的貢獻。

棧疊圖表有序：底部為基底、中間為非支出管道、頂端為支出管道。

### 依據管道的貢獻

環形圖視覺效果會顯示依管道區分的貢獻分佈。

### 行銷績效摘要。

依管道顯示ROI績效的水準長條圖。

### 邊際回應曲線。

折線圖會視覺化並比較行銷管道投資所產生的邊際回報。  找出增量回報低於增量支出的盈虧平衡點。 因此，此視覺效果可協助您瞭解行銷投資何時開始失去影響力。

曲線、收支平衡點及對應的值是根據選取的資料範圍及您選取的管道進行計算。

若要變更頻道：

* 從&#x200B;**[!UICONTROL Channel]**&#x200B;下拉式選單中選取管道，以更新特定管道的視覺效果。



## [!UICONTROL Attribution]

使用[!UICONTROL Attribution]標籤，您可以瞭解擁有事件層級資料的接觸點和行銷活動的有效性。 支援下列歸因模型：

* 根據Mix Modeler中選取的模型：
   * 演演算法 — 受影響的
   * 演演算法 — 遞增式
* 以規則為基礎：
   * 衰減單位
   * 首次接觸
   * 上次接觸
   * 線性
   * U形

如需Mix Modeler中多重接觸歸因功能的簡介，請參閱[多重接觸歸因](../get-started/about.md#multi-touch-attribution)。

從&#x200B;**[!UICONTROL Attribution Model]**&#x200B;下拉式功能表中選取一或多個歸因模型。 所選的歸因模型會套用至「歸因」標籤中的所有視覺效果。

![歸因](/help/assets/model-insights-attribution.png)

Mix Modeler的多點接觸歸因精細事件分數會與整體Mix Modeler分數和ROI相符。 這些分數也可作為Experience Platform中的資料集使用。

「歸因」標籤包含下列視覺效果：

### [!UICONTROL Overview]

[!UICONTROL Overview]視覺效果會顯示所選歸因模型的轉換總計和百分比。 選取更多模型後，視覺效果中會新增其他圓圈，每個圓圈都有各自對應圖例的顏色。

若要檢視包含歸因模型詳細資訊的快顯視窗，請將滑鼠移到視覺效果中的任何圓圈上。

### [!UICONTROL Trends]

[!UICONTROL Daily trends]、[!UICONTROL Weekly trends]或[!UICONTROL Monthly trends]視覺效果會顯示所選歸因模型的每日、每週或每月轉換趨勢。

若要選擇句點，請從![更多](/help/assets/icons/More.svg)中選取&#x200B;**[!UICONTROL Daily trends]**、**[!UICONTROL Weekly trends]**&#x200B;或&#x200B;**[!UICONTROL Monthly trends]**。

若要檢視詳細資訊，請將滑鼠停留在特定歸因模型的資料行上，以顯示顯示該資料轉換總數的彈出視窗。

### [!UICONTROL Breakdown]

[!UICONTROL Breakdown]視覺效果是每個所選歸因模型轉換的劃分管道或接觸點。 此視覺效果有助於決定每個頻道或接觸點的成效。

若要選擇劃分型別，請從![更多](/help/assets/icons/More.svg)中選取&#x200B;**[!UICONTROL Breakdown by channel]**&#x200B;或&#x200B;**[!UICONTROL Breakdown by touchpoint]**。

若要檢視詳細資訊，請將滑鼠游標停留在任何圖表元素上。

### [!UICONTROL Top campaigns]

熱門促銷活動視覺效果會顯示熱門促銷活動表格，其中包含「促銷活動名稱」、「頻道」、「媒體型別」和「遞增式轉換」欄。 此視覺效果有助於讓您的團隊瞭解特定管道的特定行銷活動的成效，並提供您應進一步投資哪些行銷活動的深入分析。

若要針對「頻道」、「媒體型別」或「遞增轉換」↓以遞增↑或遞減順序來排序表格，請選取欄標題並切換排序。

若要在個別對話方塊中展開表格，請從![更多](/help/assets/icons/More.svg)中選取&#x200B;**[!UICONTROL Expand]**。

展開的「熱門促銷活動」對話方塊會顯示相同的表格，其中包含下列專案的額外欄

* 增量轉換
* 受影響的轉換
* 首次接觸轉換
* 上次接觸轉換

  您可以選取每個額外的欄標題，以遞增或遞減順序排序表格。

若要關閉展開的[熱門促銷活動]對話方塊，請選取&#x200B;**[!UICONTROL Close]**。


### [!UICONTROL Breakdown by touchpoint position]

[!UICONTROL Breakdown by touchpoint position]視覺效果是依據所有轉換路徑上的接觸點和接觸點的位置劃分已歸因的轉換。 此圖表可協助您比較某個接觸點在某個位置的貢獻是否優於其他位置和其他任何位置的接觸點。

>[!NOTE]
>
>歸因模型在所有接觸點和位置的貢獻百分比總和應等於100。


位置[!UICONTROL Starter]、[!UICONTROL Player]和[!UICONTROL Closer]的定義如下：

| 位置 | 說明 |
|---|---|
| [!UICONTROL Starter] | 此位置會指出該接觸點是否為轉換路徑中的首次接觸。 |
| [!UICONTROL Player] | 此位置指出接觸點是否不是導致轉換的第一次或最後一次接觸。 |
| [!UICONTROL Closer] | 此位置會指出該接觸點是否為轉換前的最後一次接觸。 |


### [!UICONTROL Top conversion paths]

[!UICONTROL Top conversion paths]視覺效果會根據選取的歸因模型顯示前5個轉換路徑。

對於每個轉換路徑，您會看到：

* 確實有影響的管道數，
* 已歸因的路徑總數，
* 此轉換路徑的已歸因路徑與已歸因路徑總數的百分比，
* 每個管道的歸因模型貢獻百分比，以及
* 這些管道歸因模型貢獻百分比的總和。

## **[!UICONTROL Factors]**

因子標籤會顯示外部因子相關的深入分析。

![因素](/help/assets/factors.png)

此視覺效果可協助您瞭解各種內部和外部因素對轉換基準線的累加影響。 例如，經濟條件或促銷活動。


若要下載包含資料表資料的CSV檔案，請選取![下載](/help/assets/icons/Download.svg)。

如果沒有可用的資料，您會看到訊息![TableAndChart](/help/assets/icons/TableAndChart.svg) **[!UICONTROL No data is available, you may need to retrain your model, or change the date range to view insights]**。

## [!UICONTROL Diagnostics]

「診斷」標籤會顯示下列專案的視覺效果：

* [!UICONTROL Model Assessment]視覺效果，您可根據「實際」與「預計」或「剩餘」轉換劃分視覺效果。

  若要劃分視覺效果，請從&#x200B;**[!UICONTROL Breakdown]**&#x200B;清單中選取&#x200B;**[!UICONTROL Actual vs. Predicted]**&#x200B;或&#x200B;**[!UICONTROL Residuals]**。

* [!UICONTROL Model fitting metrics]資料表，顯示每個轉換量度的下列資料行：

   * 實際轉換

   * 模型化轉換

   * 剩餘轉換（實際轉換與模型化轉換之間的差異）

   * 模型品質分數值：

      * R2 （R平方），表示資料符合回歸模型的程度（符合的程度）。

      * MAPE （平均絕對誤差百分比），這是最常用來測量預測準確度的KPI之一，並以實際值的百分比表示預測誤差。

      * RMSE （均方根誤差）：顯示平均誤差，根據誤差的平方加權。

  若要下載包含資料表資料的CSV檔案，請選取![下載](/help/assets/icons/Download.svg)。

* [!UICONTROL Touchpoint effectiveness]資料表，代表Attribution AI演演算法模型的結果。 只會針對特定時段產生此資料表的資料。 選取&#x200B;**[!UICONTROL As of *xx/xx/xx， xx：xx TZ *]**![資訊](/help/assets/icons/InfoOutline.svg)以取得詳細資料。

  視覺效果會以遞減順序顯示每個接觸點的[!UICONTROL Efficiency measure] ![遞減順序](/help/assets/icons/SortOrderDown.svg)：

   * [!UICONTROL Paths touched]：將達成轉換的路徑百分比與未達成轉換的路徑百分比視覺化。 對於接觸點，當歸因轉換比率很高時，您會看到更多歸因轉換。 此比率比較產生轉換的路徑百分比與&#x200B;*不會*&#x200B;產生轉換的路徑百分比。
   * [!UICONTROL Efficiency measure]：由演演算法歸因模型產生，效率測量表示某個接觸點對轉換的相對重要性，與接觸點數量無關。 效率是以1到5的級數來衡量。 請注意，接觸點數量越多並不保證測量效率越高。
   * [!UICONTROL Total volume]：使用者接觸接觸點的彙總次數。 數目包括出現在達成轉換的路徑上的接觸點，以及導致轉換的路徑&#x200B;*not*。

![診斷](/help/assets/model-insights-diagnostics.png)


## [!UICONTROL Historical overview]

「歷史總覽」標籤會顯示下列專案的視覺效果：

* 依會計季度和產品劃分的轉換與支出。

* 依據管道的支出。

* 接觸點支出。

  您可以選取要針對此視覺效果顯示的替代支出型管道。 從&#x200B;**[!UICONTROL Channels]**&#x200B;中選取頻道。

* 接觸點數量。

  您可以選取替代的音量型色版，以顯示此視覺效果。 從&#x200B;**[!UICONTROL Channels]**&#x200B;中選取頻道。

![模型 — 歷史總覽](/help/assets/model-insights-historical-overview.png)
