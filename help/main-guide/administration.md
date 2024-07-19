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

使用[Adobe Admin Console](https://helpx.adobe.com/tw/enterprise/using/admin-console.html)管理Mix Modeler產品和使用者。

若要讓Mix Modeler正常運作，您必須設定正確的許可權。

在Adobe Experience Cloud UI中：

1. 從左側邊欄選取&#x200B;**[!UICONTROL ADMINISTRATION]**&#x200B;下方的&#x200B;**[!UICONTROL Permissions]**。

1. 從左側面板中選取![使用者](/help/assets/icons/User.svg) **[!UICONTROL Roles]**。

1. 選取現有的角色，或使用&#x200B;**[!UICONTROL Create role]**&#x200B;建立角色(例如，**Mix Modeler**)。 如果您選取現有的角色，請選取![編輯](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]**&#x200B;以編輯角色的許可權。 如需詳細資訊，請參閱[管理角色](https://helpx.adobe.com/tw/enterprise/using/admin-console.html)。

1. 確保您已為角色選取一或多個沙箱。

1. 將&#x200B;**Adobe Mix Modeler**&#x200B;資源新增至角色的資源清單。

1. 請確定您為正在設定的角色選取正確的&#x200B;**[!UICONTROL Adobe Mix Modeler]**&#x200B;許可權。 您可以選取下列一或多個角色：

   - **[!UICONTROL View Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL Manage Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL View Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL View Adobe Mix Modeler Plans Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Plans Configuration]**

     ![Mix ModelerRBAC](/help/assets/mix-modeler-rbac.png)


1. 請確定您為角色選取其他許可權。 例如，若要檢視或管理資料集和結構描述，您可以選取：

   - **[!UICONTROL Data Management]**：選取相關選項： **[!UICONTROL View Datasets]**&#x200B;或&#x200B;**[!UICONTROL Manage Datasets]**。

   - **[!UICONTROL Data Modeling]**：選取相關選項： **[!UICONTROL Manage Schemas]**&#x200B;或&#x200B;**[!UICONTROL View Schemas]**。

   <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    -->

   <!--![Permissions](assets/permissions-including-privacy.png)-->

   選取&#x200B;**[!UICONTROL Save]**&#x200B;以儲存許可權。

1. 在&#x200B;**[!UICONTROL Role]**&#x200B;內的&#x200B;**[!UICONTROL Details]**&#x200B;中，新增適當的&#x200B;**[!UICONTROL Users]**&#x200B;或&#x200B;**[!UICONTROL User groups]**&#x200B;以提供使用者存取Mix Modeler的許可權。
