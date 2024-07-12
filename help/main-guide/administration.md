---
title: 管理
description: 瞭解如何管理Mix Modeler。
feature: Administration
exl-id: 76d6d15d-a838-4ee2-9929-e55ea8946b80
source-git-commit: 4d84c93121fc476cc6610ad572bab161bbacfc23
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# 管理

使用 [Adobe Admin Console](https://helpx.adobe.com/tw/enterprise/using/admin-console.html) 管理Mix Modeler產品和使用者。

若要讓Mix Modeler正常運作，您必須設定正確的許可權。

在Adobe Experience Cloud UI中：

1. 選取 **[!UICONTROL Permissions]** 從左側邊欄，底下 **[!UICONTROL ADMINISTRATION]**.

1. 選取 ![使用者](/help/assets/icons/User.svg) **[!UICONTROL Roles]** 從左側面板。

1. 選取現有角色，或使用以下方式建立角色 **[!UICONTROL Create role]** (例如， **Mix Modeler**)。 如果您選取現有角色，請選取 ![編輯](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]** 編輯角色的許可權。 另請參閱 [管理角色](https://helpx.adobe.com/tw/enterprise/using/admin-console.html) 以取得詳細資訊。

1. 確保您已為角色選取一或多個沙箱。

1. 新增 **Adobe Mix Modeler** 資源到角色的資源清單。

1. 請確定您選取正確的專案 **[!UICONTROL Adobe Mix Modeler]** 您設定之角色的許可權。 您可以選取下列一或多個角色：

   - **[!UICONTROL View Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL Manage Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL View Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL View Adobe Mix Modeler Plans Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Plans Configuration]**

     ![MIX MODELERRBAC](/help/assets/mix-modeler-rbac.png)


1. 請確定您為角色選取其他許可權。 例如，若要檢視或管理資料集和結構描述，您可以選取：

   - **[!UICONTROL Data Management]**：選取相關選項： **[!UICONTROL View Datasets]** 或 **[!UICONTROL Manage Datasets]**.

   - **[!UICONTROL Data Modeling]**：選取相關選項： **[!UICONTROL Manage Schemas]** 或 **[!UICONTROL View Schemas]**.

   <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    -->

   <!--![Permissions](assets/permissions-including-privacy.png)-->

   選取 **[!UICONTROL Save]** 以儲存許可權。

1. 在 **[!UICONTROL Details]** 範圍 **[!UICONTROL Role]**，新增適當的 **[!UICONTROL Users]** 或 **[!UICONTROL User groups]** 提供使用者存取Mix Modeler的許可權。
