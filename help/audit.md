---
title: 稽核
description: 瞭解如何稽核Mix Modeler。
feature: Administration
exl-id: aa65aac5-bea4-43ff-b0d0-9e8a6a97d3ca
source-git-commit: 3f816c9a88ea9e49cf6744d41c9ff1753c29dd30
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 6%

---

# 稽核

>[!AVAILABILITY]
>
>本文所述的功能處於發行的有限測試階段，可能尚未在您的環境中提供。 當功能正式可用時，將移除此附註。 如需有關最新Mix Modeler版本的資訊，請參閱 [Mix Modeler版本](/help/releases/latest.md).

您可以使用Mix Modeler的稽核介面部分和內嵌在Mix ModelerUI中，稽核使用者在Experience Platform中執行的操作。

若要檢查稽核記錄，請在Mix Modeler介面中：

1. 選取 ![任務清單](/help/assets/icons/TaskList.svg) **[!UICONTROL Audits]** 從 **[!UICONTROL PRIVACY]**.

1. 在 **[!UICONTROL Audits]** 您可找到 **[!UICONTROL Activity log]**. 活動記錄會顯示下列Mix Modeler類別、動作和狀態的專案。

   | 類別 | 動作 | 狀態 |
   |---|---|---|
   | Mix Modeler資料集規則 | 建立 | 允許或拒絕 |
   | Mix Modeler資料集規則 | 更新 | 允許或拒絕 |
   | Mix Modeler資料集規則 | 刪除 | 允許或拒絕 |
   | Mix Modeler欄位 | 建立 | 允許或拒絕 |
   | Mix Modeler欄位 | 更新 | 允許或拒絕 |
   | Mix Modeler欄位 | 刪除 | 允許或拒絕 |
   | Mix Modeler行銷接觸點 | 建立 | 允許或拒絕 |
   | Mix Modeler行銷接觸點 | 更新 | 允許或拒絕 |
   | Mix Modeler行銷接觸點 | 刪除 | 允許或拒絕 |
   | Mix Modeler轉換 | 建立 | 允許或拒絕 |
   | Mix Modeler轉換 | 更新 | 允許或拒絕 |
   | Mix Modeler轉換 | 刪除 | 允許或拒絕 |
   | Mix Modeler模型 | 建立 | 允許或拒絕 |
   | Mix Modeler模型 | 更新 | 允許或拒絕 |
   | Mix Modeler模型 | 刪除 | 允許或拒絕 |

1. 在活動記錄中選取專案以開啟面板，瞭解更多詳細資訊。

   ![Mix Modeler稽核](/help/assets/mix-modeler-audit.png)

1. 篩選依據 **[!UICONTROL Category]**， **[!UICONTROL Action]**， **[!UICONTROL Request ID]**， **[!UICONTROL User]**， **[!UICONTROL Status]** 或 **[!UICONTROL Date]** 範圍，選取 ![篩選](/help/assets/icons/Filter.svg).

1. 若要修改活動記錄中顯示的欄，請選取 ![欄](/help/assets/icons/ColumnSetting.svg) 和 **[!UICONTROL Customize table]** 對話方塊選取要顯示的欄。 選取 **[!UICONTROL Apply]** 若要套用選取範圍， **[!UICONTROL Cancel]** 以取消選取。

1. 若要下載稽核記錄，請選取 ![下載](/help/assets/icons/Download.svg) **[!UICONTROL Download log]**. 在 **[!UICONTROL Download log]** 對話方塊選取 **[!UICONTROL CSV]** 或 **[!UICONTROL JSON]** 格式並選取「 」 **[!UICONTROL Download]**.

