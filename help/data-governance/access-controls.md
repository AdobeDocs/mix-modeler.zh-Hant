---
title: 存取控制
description: 瞭解如何在Mix Modeler中設定存取控制。
feature: Administration
exl-id: c9ec97d9-b9a2-41f5-8626-1cf967d5d7fe
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 1%

---

# 存取控制

透過[Adobe Admin Console](https://adminconsole.adobe.com/)中的Experience Platform以及Experience Platform中的[許可權](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#platform-permissions)，提供Mix Modeler的存取控制。 此功能運用Admin Console中的產品設定檔，將使用者與許可權和沙箱連結。

如需存取控制的詳細資訊，請參閱[存取控制總覽](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home)。

## 角色型存取控制

請參閱[管理](../main-guide/administration.md)，瞭解如何設定Experience Platform中Mix Modeler使用者與使用者群組的角色型存取許可權。

## 屬性型存取控制

[以屬性為基礎的存取控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)是一種Experience Platform功能，可讓系統管理員根據屬性控制特定物件和/或權能的存取。 屬性可以是新增至物件的中繼資料，例如新增至結構欄位或區段的標籤。 管理員定義存取原則，其中包含管理使用者存取許可權的屬性。

此功能可讓您使用定義組織或資料使用範圍的標籤，來標籤Experience Data Model (XDM)結構描述欄位。 同時，管理員可以使用使用者和角色管理介面，在XDM結構描述欄位上定義存取原則。 也能更有效管理使用者或使用者群組（內部、外部或協力廠商使用者）的存取權。 此外，屬性型存取控制可讓管理員管理特定區段的存取權。

透過屬性型存取控制，管理員可控制使用者對所有Platform工作流程與資源的敏感個人資料(SPD)和個人識別資訊(PII)的存取權。 管理員可以定義僅能存取特定欄位以及對應至這些欄位之資料的使用者角色。

設定協調資料集的資料集規則時，會在欄位層級上強制執行Experience Platform的[屬性型存取控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)。 標籤附加至結構描述欄位時，欄位會受到限制。 並且會啟用拒絕您存取該欄位的作用中原則。 因此：

* 您沒有在建立資料集規則時看到為您限制的結構描述欄位。
* 您無法檢視或編輯一或多個限制您使用的結構描述欄位的對應。 當您編輯或檢視包含這類受限制欄位的資料集規則時，您會看到下列畫面。
  ![不允許的動作](/help/assets/action-not-permitted.png)
