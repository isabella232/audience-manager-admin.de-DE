---
description: Befolgen Sie diese Anweisungen, um eine vollständige Synchronisierungsdatei zu generieren, die nur kürzlich aktive Benutzer enthält. Sie können nach aktiven Benutzern filtern, um relevante Daten an ein On-site-Targeting-System zu übertragen oder die Größe der an einen DSP gesendeten Dateien zu begrenzen. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.
seo-description: Befolgen Sie diese Anweisungen, um eine vollständige Synchronisierungsdatei zu generieren, die nur kürzlich aktive Benutzer enthält. Sie können nach aktiven Benutzern filtern, um relevante Daten an ein On-site-Targeting-System zu übertragen oder die Größe der an einen DSP gesendeten Dateien zu begrenzen. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.
seo-title: Filtern von ausgehenden Daten nur nach aktiven Benutzern
title: Filtern von ausgehenden Daten nur nach aktiven Benutzern
uuid: a2b4a385-eee3-458c-b978-09509cacb397
exl-id: d501cfd1-64dd-448e-92c5-180c0081d3e5
source-git-commit: f5d74995f0664cf63e68b46f1f3c608f34df0e80
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 8%

---

# Filtern von ausgehenden Daten nur nach aktiven Benutzern {#filter-outbound-data-by-active-users-only}

Befolgen Sie diese Anweisungen, um eine vollständige Synchronisierungsdatei zu generieren, die nur kürzlich aktive Benutzer enthält. Sie können nach aktiven Benutzern filtern, um relevante Daten an ein On-site-Targeting-System zu übertragen oder die Größe der an einen DSP gesendeten Dateien zu begrenzen. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.

>[!NOTE]
>
>Ein Besucher muss nicht auf einer ausgewählten Kunden-Site oder in seinem Anzeigen-Traffic gesehen werden, um sich als &quot;aktiv&quot;zu qualifizieren. Sie können von jedem [!DNL Audience Manager]-Kunden oder -Partner gesehen werden, der sich als &quot;aktiv&quot;qualifiziert.

So filtern Sie nur nach aktiven Benutzern:

1. Klicken **[!UICONTROL Companies]**.
1. Wählen Sie das Unternehmen aus, mit dem Sie arbeiten möchten, und klicken Sie auf **[!UICONTROL Destinations]**.
1. Legen Sie im Abschnitt [!UICONTROL Batch Data] die folgenden Optionen fest:

   * **[!UICONTROL Sync Type]**: Wählen Sie  **[!UICONTROL Customer]** oder  **[!UICONTROL Platform]**.
   * **[!UICONTROL Sync Type Lookback Period]**: Dieses Zeitintervall definiert den Bereich Ihrer Datendatei. Zu den Optionen gehören **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]**.
   * **[!UICONTROL Incremental Sync Scheduled Run]**: Select **[!UICONTROL Never]**. Beachten Sie, dass dieser Filter nur für vollständige Synchronisierungsdateien gilt.
   * **[!UICONTROL Full Sync Scheduled Run]**: Dadurch wird bestimmt, wie oft Sie diese Datei erhalten möchten. Zu den Optionen gehören **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]** oder **[!UICONTROL Never]** (zum Deaktivieren).

1. Klicken **[!UICONTROL Save]**.
