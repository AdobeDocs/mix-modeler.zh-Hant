---
title: 存取控制
description: 瞭解如何在Mix Modeler中設定存取控制。
feature: Administration
exl-id: c9ec97d9-b9a2-41f5-8626-1cf967d5d7fe
TQID: https://experienceleague.adobe.com/EoiF5ui2Bqq0Oxuv-s5E5pQclj9gnjoKgZ1bOzRK-vY
product_v2: id: b88c80e3-31df-4609-989d-d4dac0e6d973
feature_v2: id: fe2edbb1-46f9-4347-a27c-577cab3640cb
subfeature_v2: id: abe9e290-7d2f-4131-b71e-ef9900865044
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
autotag-review: '2026-05-01T09:20:37.287Z'
source-git-commit: 5579087b9381c4d8e909ed5fe3099fd42d5c6799
workflow-type: tm+mt
source-wordcount: 412
ht-degree: 1%

---

# 存取控制

Mix Modeler的存取控制是透過[Adobe Admin Console](https://adminconsole.adobe.com/)中的Experience Platform以及Experience Platform中的[許可權](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#platform-permissions)提供。 此功能運用Admin Console中的產品設定檔，將使用者與許可權和沙箱連結。

如需存取控制的詳細資訊，請參閱[存取控制總覽](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home)。

## 角色型存取控制

請參閱[管理](../main-guide/administration.md)，瞭解如何在Experience Platform中為Mix Modeler使用者和使用者群組設定角色型存取許可權。

## 屬性型存取控制

[以屬性為基礎的存取控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)是Experience Platform的一項功能，可讓管理員根據屬性控制特定物件和/或功能的存取。 屬性可以是新增至物件的中繼資料，例如新增至結構欄位或區段的標籤。 管理員定義存取原則，其中包含管理使用者存取許可權的屬性。

此功能可讓您使用定義組織或資料使用範圍的標籤，來標籤Experience Data Model (XDM)結構描述欄位。 同時，管理員可以使用使用者和角色管理介面，在XDM結構描述欄位上定義存取原則。 也能更有效管理使用者或使用者群組（內部、外部或協力廠商使用者）的存取權。 此外，屬性型存取控制可讓管理員管理特定區段的存取權。

透過屬性型存取控制，管理員可控制使用者對所有Platform工作流程與資源的敏感個人資料(SPD)和個人識別資訊(PII)的存取權。 管理員可以定義僅能存取特定欄位以及對應至這些欄位之資料的使用者角色。

設定協調資料集的資料集規則時，會在欄位層級強制執行Experience Platform的[屬性型存取控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)。 標籤附加至結構描述欄位時，欄位會受到限制。 並且會啟用拒絕您存取該欄位的作用中原則。 因此：

* 您沒有在建立資料集規則時看到為您限制的結構描述欄位。
* 您無法檢視或編輯一或多個限制您使用的結構描述欄位的對應。 當您編輯或檢視包含這類受限制欄位的資料集規則時，您會看到下列畫面。
  ![不允許的動作](/help/assets/action-not-permitted.png)
