---
description: Führen Sie die folgenden Schritte aus, um eine vollständige Synchronisierungsdatei zu erstellen, die nur aktive Benutzer enthält. Möglicherweise möchten Sie nach aktiven Benutzern filtern, um relevante Daten an ein Onsite-Targeting-System zu senden oder die Größe der an eine DSP gesendeten Dateien einzuschränken. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.
seo-description: Führen Sie die folgenden Schritte aus, um eine vollständige Synchronisierungsdatei zu erstellen, die nur aktive Benutzer enthält. Möglicherweise möchten Sie nach aktiven Benutzern filtern, um relevante Daten an ein Onsite-Targeting-System zu senden oder die Größe der an eine DSP gesendeten Dateien einzuschränken. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.
seo-title: Nur ausgehende Daten nach aktiven Benutzern filtern
title: Nur ausgehende Daten nach aktiven Benutzern filtern
uuid: a 2 b 4 a 385-eee 3-458 c-b 978-09509 cacb 397
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54

---


# Nur ausgehende Daten nach aktiven Benutzern filtern {#filter-outbound-data-by-active-users-only}

Führen Sie die folgenden Schritte aus, um eine vollständige Synchronisierungsdatei zu erstellen, die nur aktive Benutzer enthält. Möglicherweise möchten Sie nach aktiven Benutzern filtern, um relevante Daten an ein Onsite-Targeting-System zu senden oder die Größe der an eine DSP gesendeten Dateien einzuschränken. Sie können diesen Filter nicht mit inkrementeller Synchronisierung verwenden.

>[!NOTE]
>
>Ein Besucher muss nicht auf einer ausgewählten Kunden-Site oder in ihrem Anzeigenverkehr gesehen werden, um ihn als "aktiv" zu qualifizieren. Sie können von jedem [!DNL Audience Manager] Kunden oder Partner gesehen werden, um als "aktiv" zu qualifizieren.

So filtern Sie nur nach aktiven Benutzern:

1. Klicken Sie auf **[!UICONTROL Companies]**.
1. Wählen Sie das Unternehmen aus, mit dem Sie arbeiten möchten, und klicken **[!UICONTROL Destinations]** Sie auf.
1. Legen Sie im [!UICONTROL Batch Data] Abschnitt die folgenden Optionen fest:

   * **[!UICONTROL Sync Type]**: Auswählen **[!UICONTROL Customer]** oder **[!UICONTROL Platform]**.
   * **[!UICONTROL Sync Type Lookback Period]**: Dieses Zeitintervall definiert den Bereich Ihrer Datendatei. Die Optionen umfassen **[!UICONTROL 24 hours]****[!UICONTROL 7 days]****[!UICONTROL 30 days]**.
   * **[!UICONTROL Incremental Sync Scheduled Run]**: Wählen **[!UICONTROL Never]** Sie. Denken Sie daran, dass dieser Filter nur für vollständige Synchronisierungsdateien gilt.
   * **[!UICONTROL Full Sync Scheduled Run]**: Dies bestimmt, wie oft Sie diese Datei erhalten möchten. Die Optionen **[!UICONTROL 24 hours]****[!UICONTROL 7 days]** umfassen **[!UICONTROL 30 days]**, oder **[!UICONTROL Never]** (zur Deaktivierung).

1. Klicken Sie auf **[!UICONTROL Save]**.
