---
title: 稽核記錄
description: 瞭解如何從Mix Modeler存取稽核記錄。
feature: Administration
exl-id: aa65aac5-bea4-43ff-b0d0-9e8a6a97d3ca
source-git-commit: 85f9b42a775006cd3566447b2bb9d0a806fa3e73
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 5%

---

# 稽核記錄

為了提高系統中所執行活動的透明度和可見度，Mix Modeler工作流程中的使用者活動會擷取在Experience Platform稽核記錄中，以瞭解Mix Modeler類別的任何使用者導向變更。 這些記錄形成了稽核軌跡，可以幫助解決問題，並且可以幫助您的企業有效地遵守公司資料管理政策和監管要求。

<!-- DO WE HAVE TO ADD THIS
If you are subject to the Health Insurance Portability and Accountability Act (HIPAA) and create, receive, maintain, or transmit permitted sensitive personal data through Mix Modeler, you are responsible for executing a BAA with Adobe and licensing Healthcare Shield.
-->

稽核記錄會通知執行動作的人及時間。 記錄中記錄的每個動作都包含中繼資料，其指出動作型別、日期和時間、執行動作之使用者的電子郵件ID，以及與動作型別相關的其他屬性。 它會追蹤使用者在Mix Modeler中採取的建立、更新和刪除動作。

若要檢查稽核記錄，請在Mix Modeler介面中：

1. 從&#x200B;**[!UICONTROL PRIVACY]**&#x200B;選取![工作清單](/help/assets/icons/TaskList.svg) **[!UICONTROL Audits]**。

1. 在&#x200B;**[!UICONTROL Audits]**&#x200B;中，您可以找到&#x200B;**[!UICONTROL Activity log]**。 活動記錄會顯示下列Mix Modeler類別、動作和狀態的專案。

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
   | Mix Modeler模型 | Rescore | 允許或拒絕 |
   | Mix Modeler模型 | 原地複製 | 允許或拒絕 |
   | Mix Modeler模型 | 訓練/重新訓練 | 允許或拒絕 |
   | Mix Modeler模型 | 下載/儲存中繼資料 | 允許或拒絕 |
   | Mix Modeler計畫 | 建立 | 允許或拒絕 |
   | Mix Modeler計畫 | 更新 | 允許或拒絕 |
   | Mix Modeler計畫 | 變更關聯的模型 | 允許或拒絕 |
   | Mix Modeler資料協調 | 觸發同步 | 允許或拒絕 |


1. 在活動記錄中選取專案以開啟面板，瞭解更多詳細資訊。

   ![Mix Modeler稽核](/help/assets/mix-modeler-audit.png)

1. 若要篩選&#x200B;**[!UICONTROL Category]**、**[!UICONTROL Action]**、**[!UICONTROL Request ID]**、**[!UICONTROL User]**、**[!UICONTROL Status]**&#x200B;或&#x200B;**[!UICONTROL Date]**&#x200B;範圍，請選取![篩選器](/help/assets/icons/Filter.svg)。

1. 若要修改活動記錄中顯示的欄，請選取![欄](/help/assets/icons/ColumnSetting.svg)，然後在&#x200B;**[!UICONTROL Customize table]**&#x200B;對話方塊中選取要顯示的欄。 選取&#x200B;**[!UICONTROL Apply]**&#x200B;以套用選取專案，**[!UICONTROL Cancel]**&#x200B;以取消選取專案。

1. 若要下載稽核記錄，請選取![下載](/help/assets/icons/Download.svg) **[!UICONTROL Download log]**。 在&#x200B;**[!UICONTROL Download log]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL CSV]**&#x200B;或&#x200B;**[!UICONTROL JSON]**&#x200B;作為格式，並選取&#x200B;**[!UICONTROL Download]**。

## 存取稽核記錄

為您的組織啟用此功能後，活動發生時會自動收集稽核記錄。 您不需要手動啟用稽核記錄收集。

若要檢視和匯出稽核記錄，您必須已被授與稽核記錄存取權存取控制許可權。 若要瞭解如何管理Mix Modeler功能的個別許可權，請參閱[存取控制檔案](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home)。
