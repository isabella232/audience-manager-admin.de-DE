---
description: Befolgen Sie diese Anweisungen, um eine vollständige Synchronisierungsdatei zu erstellen, die nur kürzlich aktive Benutzer enthält. Möglicherweise möchten Sie nach aktiven Benutzern filtern, um relevante Daten an ein Onsite-Targeting-System zu übertragen oder die Größe der an ein DSP gesendeten Dateien zu beschränken. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.
seo-description: Befolgen Sie diese Anweisungen, um eine vollständige Synchronisierungsdatei zu erstellen, die nur kürzlich aktive Benutzer enthält. Möglicherweise möchten Sie nach aktiven Benutzern filtern, um relevante Daten an ein Onsite-Targeting-System zu übertragen oder die Größe der an ein DSP gesendeten Dateien zu beschränken. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.
seo-title: Ausgehende Daten nur nach aktiven Benutzern filtern
title: Ausgehende Daten nur nach aktiven Benutzern filtern
uuid: a2b4a385-ee3-458c-b978-09509cacb397
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54

---


# Ausgehende Daten nur nach aktiven Benutzern filtern {#filter-outbound-data-by-active-users-only}

Befolgen Sie diese Anweisungen, um eine vollständige Synchronisierungsdatei zu erstellen, die nur kürzlich aktive Benutzer enthält. Möglicherweise möchten Sie nach aktiven Benutzern filtern, um relevante Daten an ein Onsite-Targeting-System zu übertragen oder die Größe der an ein DSP gesendeten Dateien zu beschränken. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.

>[!NOTE]
>
>Ein Besucher muss nicht auf einer bestimmten Kundensite oder in seinem Anzeigen-Traffic gesehen werden, um sich als "aktiv"zu qualifizieren. Sie können von jedem [!DNL Audience Manager] Kunden oder Partner als "aktiv"angesehen werden.

So filtern Sie nur nach aktiven Benutzern:

1. Klicken Sie auf **[!UICONTROL Companies]**.
1. Wählen Sie das Unternehmen aus, mit dem Sie arbeiten möchten, und klicken Sie auf **[!UICONTROL Destinations]**.
1. Legen Sie im [!UICONTROL Batch Data] Abschnitt die folgenden Optionen fest:

   * **[!UICONTROL Sync Type]**: Wählen Sie **[!UICONTROL Customer]** oder **[!UICONTROL Platform]**.
   * **[!UICONTROL Sync Type Lookback Period]**: Dieses Zeitintervall definiert den Bereich Ihrer Datendatei. Zu den Optionen zählen **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]**.
   * **[!UICONTROL Incremental Sync Scheduled Run]**: Wählen Sie **[!UICONTROL Never]**. Beachten Sie, dass dieser Filter nur für vollständige Synchronisierungsdateien gilt.
   * **[!UICONTROL Full Sync Scheduled Run]**: Dadurch wird bestimmt, wie oft Sie diese Datei erhalten möchten. Zu den Optionen gehören **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]** oder **[!UICONTROL Never]** (deaktivieren).

1. Klicken Sie auf **[!UICONTROL Save]**.
