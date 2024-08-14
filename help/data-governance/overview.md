---
title: 資料控管
description: 瞭解如何使用Experience Platform中的服務和工具，讓您控制收集的體驗資料。 這樣一來，您就能遵守業務實務、法律義務和開發程式。
feature: Administration
source-git-commit: 6776a91563f120db1341adef923aab4b0f582c9d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 2%

---

# 資料控管

Mix Modeler與Experience Platform之間的整合為Mix Modeler提供了運用Experience Platform內建資料控管功能的功能。 本檔案區段詳細說明Mix Modeler中可用資料控管功能的細節。

Experience Platform資料控管讓您能夠控制並理解資料經過Experience Platform的整個歷程。 此歷程涉及維護資料品質、資料譜系、資料編目等等。

在資料集上建立的資料使用標籤和原則，會由Mix Modeler中的Experience Platform表面適時使用。 例如，在刪除屬於協調資料中資料集規則一部分的資料集時，這些標籤會停止或警告使用者。 或是在建立資料集規則時隱藏使用者限制的結構描述欄位。

資料控管整合可讓您更有效率地管理合規性。 您組織中的資料管理員可以設定原則來限制使用。 因此，您可以使用符合資料管理員所定義原則的資料。 請閱讀[標籤和原則](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/data-governance)的相關檔案以深入瞭解。

下列資料控管功能可供使用：

| 功能 | 詳細資料 |
|---|---|
| 存取控制 | 支援角色型存取控制及屬性型（欄位層級）存取控制。 如需詳細資訊，請參閱[存取控制](access-controls.md)。 |
| 稽核記錄 | 當使用者建立、更新或刪除特定Mix Modeler類別時，「Experience Platform稽核」功能會在稽核記錄中記錄該活動。 如需詳細資訊，請參閱[稽核記錄](audit-logs.md)。 |
| 原則 | 在協調的資料工作流程中，會強制執行Experience Platform定義的原則。 任何違反資料使用標籤的情況都會向使用者報告和顯示。 如需詳細資訊，請參閱[原則](policies.md)。 |
| 加密 | 所有用於模型輸入和輸出的資料集都遵循Experience Platform准則。 Experience Platform資料加密適用於閒置和傳輸中的資料。 |
| 資料衛生 | 所有用於模型輸入和輸出的資料集都遵循Experience Platform准則。 Experience Platform提供一套工具來管理客戶的資料生命週期，包括支援不同型別的資料有效期。 當您從Experience Platform中刪除來源資料集（用於協調資料的一部分）時，您會收到通知。 如需詳細資訊，請參閱[資料集規則](/help/harmonize-data/dataset-rules.md)。 |
| 客戶託管金鑰 | 當您具有Privacy Security Shield或Healthcare Shield附加元件的授權Mix Modeler時，您可以使用客戶自控金鑰功能來運用Azure金鑰儲存庫，透過API自備金鑰。 您可以在Mix Modeler的模型內完整管理正在處理的資料。 |
