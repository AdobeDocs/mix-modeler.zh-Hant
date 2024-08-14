---
title: 原則
description: 瞭解如何從Mix Modeler存取原則。
feature: Administration
exl-id: 4dba7c30-ad1e-4213-a2b0-afc55f2448a3
source-git-commit: 132dc18b84723358a7d65e2aaadd49cf1deb2dd8
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---

# 原則

一旦您通過工作流程建立模型並提交模型的組態，[原則執行](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/enforcement/overview#automatic-enforcement)會檢查是否有任何違規。 如果發生原則違規，會出現一個彈出視窗，指出已違反一或多個原則。 此檢查旨在確保您在Experience Platform中的資料作業和行銷動作符合資料使用原則。

依預設，Mix Modeler會檢查與下列標籤和行銷動作相關聯的Adobe定義原則是否違規：

| 原則名稱 | 關聯的標籤 | 關聯的行銷動作 |
|---|---|---|
| 限制使用分析和以使用者為基礎的測量 | C8 | Analytics |
| 限制資料科學 | C9 | 資料科學 |
| 限制資料匯出 | C12 | 資料匯出 |

也會檢查您自行定義且包含上表所列之任何行銷動作的原則，是否違規。

在建置資料集規則時違反原則時，您會看到顯示原則違規相關資訊的彈出視窗。

例如：

- 您已啟用具有關聯標籤[!UICONTROL C9]和相關聯行銷動作[!UICONTROL Data Science]的[!UICONTROL Restrict data science]原則，
- 您已將[!UICONTROL C9] - [!UICONTROL No data science]標籤套用至轉換資料結構描述中的`totalCost`欄位，
- 您要設定資料集規則，將轉換資料結構描述的`totalCost`欄位對應到名為`spend` （和顯示名稱`Spend`）的協調欄位。

當您想要儲存資料集規則時，您會看到&#x200B;**[!UICONTROL Data governance policy violation detected]**&#x200B;快顯視窗，其中顯示違反的原則清單。 當您選取原則名稱時，在[!UICONTROL Violation summary]中，您會看到[!UICONTROL Active data governance labels]的清單，包含[!UICONTROL Entity]、[!UICONTROL Type]、[!UICONTROL Field]和[!UICONTROL Government labels]已套用。

<!-- pending screenshot -->

將資料使用標籤套用至已用於協調資料的結構描述欄位時，您會看到顯示原則違規相關資訊的彈出視窗。

例如：

- 您已設定資料集規則，其中將轉換資料結構描述的`totalCost`欄位對應到名稱為`spend` （和顯示名稱`Spend`）的協調欄位。
- 您至少已順利同步一次協調資料（請參閱[資料集規則 — 同步資料](/help/harmonize-data/dataset-rules.md#sync-data)）。
- 您啟用具有關聯標籤[!UICONTROL C9]和相關聯行銷動作[!UICONTROL Data Science]的[!UICONTROL Restrict data science]原則，
- 您想要將[!UICONTROL C9] - [!UICONTROL No data science]標籤套用至轉換資料結構描述中的`totalCost`欄位。

當您想要儲存結構描述更新時，您會看到&#x200B;**[!UICONTROL Data governance policy violation detected]**&#x200B;快顯視窗，顯示違反的原則清單。 在[!UICONTROL Violation summary]中選取原則名稱，以在[!UICONTROL Data Lineage]清單中尋找更多詳細資料。

<!-- pending screenshot -->

## 偵測到違規的彈出視窗

偵測到資料治理原則違規的彈出視窗，會提供有關違規的特定資訊。 您可以透過原則設定及其他與組態工作流程不直接相關的測量來解決這些違規。 例如，您可以變更標籤，讓某些欄位可運用於資料科學目的。 或者，您也可以修改模型組態本身，使模型不使用具有資料使用標籤的物件。

左側邊欄中的![隱私權](/help/assets/icons/Privacy.svg) **[!UICONTROL Policies]**&#x200B;選項可讓您存取Experience Platform的[!UICONTROL Policies]介面，進而管理您的原則、標籤和行銷動作。

<!--
Currently,  Mix Modeler does not support all of the data governance functionality offered by Experience Platform. Field level access control is supported. See [Field level access control](../harmonize-data/dataset-rules.md#field-level-access-control)
-->

>[!MORELIKETHIS]
>
>[資料使用原則概觀](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/policies/overview)
>
>

