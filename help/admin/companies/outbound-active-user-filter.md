---
description: Befolgen Sie diese Anweisungen, um eine vollständige Synchronisierungsdatei zu erstellen, die nur kürzlich aktive Benutzer enthält. Möglicherweise möchten Sie nach aktiven Benutzern filtern, um relevante Daten an ein Onsite-Targeting-System zu übertragen oder die Größe der an eine DSP gesendeten Dateien zu beschränken. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.
seo-description: Befolgen Sie diese Anweisungen, um eine vollständige Synchronisierungsdatei zu erstellen, die nur kürzlich aktive Benutzer enthält. Möglicherweise möchten Sie nach aktiven Benutzern filtern, um relevante Daten an ein Onsite-Targeting-System zu übertragen oder die Größe der an eine DSP gesendeten Dateien zu beschränken. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.
seo-title: Filtern von ausgehenden Daten nur nach aktiven Benutzern
title: Filtern von ausgehenden Daten nur nach aktiven Benutzern
uuid: a2b4a385-eee3-458c-b978-09509cacb397
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 8%

---


# Filtern von ausgehenden Daten nur nach aktiven Benutzern {#filter-outbound-data-by-active-users-only}

Befolgen Sie diese Anweisungen, um eine vollständige Synchronisierungsdatei zu erstellen, die nur kürzlich aktive Benutzer enthält. Möglicherweise möchten Sie nach aktiven Benutzern filtern, um relevante Daten an ein Onsite-Targeting-System zu übertragen oder die Größe der an eine DSP gesendeten Dateien zu beschränken. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.

>[!NOTE]
>
>Ein Besucher muss nicht auf einer bestimmten Kundensite oder in ihrem Anzeigen-Traffic angezeigt werden, um sich als &quot;aktiv&quot;zu qualifizieren. Sie können von jedem [!DNL Audience Manager]-Kunden oder -Partner als &quot;aktiv&quot;angesehen werden.

So filtern Sie nur nach aktiven Benutzern:

1. Klicken **[!UICONTROL Companies]**.
1. Wählen Sie die Firma aus, mit der Sie arbeiten möchten, und klicken Sie auf **[!UICONTROL Destinations]**.
1. Legen Sie im Abschnitt [!UICONTROL Batch Data] die folgenden Optionen fest:

   * **[!UICONTROL Sync Type]**: Wählen Sie  **[!UICONTROL Customer]** oder  **[!UICONTROL Platform]**.
   * **[!UICONTROL Sync Type Lookback Period]**: Dieses Zeitintervall definiert den Bereich Ihrer Datendatei. Zu den Optionen gehören **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]**.
   * **[!UICONTROL Incremental Sync Scheduled Run]**: Select **[!UICONTROL Never]**. Beachten Sie, dass dieser Filter nur für vollständige Synchronisierungsdateien gilt.
   * **[!UICONTROL Full Sync Scheduled Run]**: Dadurch wird bestimmt, wie oft Sie diese Datei erhalten möchten. Zu den Optionen gehören **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]** oder **[!UICONTROL Never]** (zum Deaktivieren).

1. Klicken **[!UICONTROL Save]**.
