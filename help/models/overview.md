---
title: 模型
description: 瞭解如何在Mix Modeler中設定和使用模型。
feature: Models
source-git-commit: 08cfd4239f6bcaf885565f3ae04cbd51869e8c00
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# 模型

Mix Modeler中的模型功能可讓您設定、訓練及評分業務目標專屬的AI/ML模型，並透過多點觸控歸因與行銷組合模型之間的AI驅動傳輸學習提供支援。

這些模型以您在Mix Modeler應用程式工作流程中建立的協調資料為基礎。

若要建立模型，請使用當您選取時可用的「混合塑模工具」逐步引導模型組態流程 **[!UICONTROL Guide me]**. 另請參閱 [建立模型](create.md) 以取得更多詳細資料。

## 管理模型

若要檢視目前模型的表格，請在Mix Modeler介面中：

1. 選取 ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** 從左側邊欄。

1. 您會看到目前模型的表格。

   表格欄指定模型的詳細資訊。

   | 欄名稱 | 詳細資料 |
   |---|---|
   | 名稱 | 模型名稱 |
   | 說明 | 模型說明 |
   | 轉換事件 | 您為模型選取的轉換。 |
   | 資料集 | 模型用來訓練和評分的資料集。 這預設為協調的資料集。 |
   | 執行頻率 | 訓練模型的執行頻率。 |
   | 上次執行 | 模型上次培訓的日期和時間。 |
   | 上次執行狀態 | 模型訓練上次執行的狀態。 <br/><span style="color:green">●</span> 成功<br/><span style="color:orange">●</span> 訓練問題<br/> <span style="color:orange">●</span> 正在等待訓練 <br/><span style="color:red">●</span> 已失敗 |

   {style="table-layout:auto"}

1. 若要變更為清單顯示的欄，請選取 ![欄設定](../assets/icons/ColumnSetting.svg) 並開啟欄 ![檢查](../assets/icons/Checkmark.svg) 或關閉。

### 刪除模型

若要刪除模型，請執行下列動作：

1. 選取要刪除的模型名稱。

1. 從內容功能表中，選取 **[!UICONTROL Delete]** 以刪除模型。

### 檢視模型的詳細資料

若要檢視模型的詳細資訊：

1. 選取您要檢視其詳細資訊的模型名稱。

1. 從內容功能表中，選取 **[!UICONTROL More]**. 您會在右窗格中看到所選模型的詳細資訊。



### 模型深入分析

>[!NOTE]
>
>此選取範圍僅適用於訓練成功的模型。
>

若要檢視模型的深入分析，請在Mix Modeler介面中：

1. 選取 ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** 從左側邊欄。

1. 選取模型名稱，其中包含 **[!UICONTROL Last run status]** 之 <span style="color:green">●</span> **[!UICONTROL Success]** 從 **[!UICONTROL Models]** 表格。

1. 從內容功能表中，選取 **[!UICONTROL Model Insights]**. 您被重新導向至 [模型深入分析](insights.md).


