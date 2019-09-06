---
description: Erstellen, bearbeiten und löschen Sie Zielgruppen-Manager-Ziele.
seo-description: Erstellen, bearbeiten und löschen Sie Zielgruppen-Manager-Ziele.
seo-title: Unternehmensziele verwalten
title: Unternehmensziele verwalten
uuid: d 9 a 6 bfb 1-7629-44 e 0-b 7 d 7-ece 44 f 65 ea 2 b
translation-type: tm+mt
source-git-commit: 57d7a92265e565b6c411e4cfa5c579e40eb837b3

---


# Unternehmensziele verwalten {#manage-company-destinations}

Erstellen, bearbeiten und löschen Sie Zielgruppen-Manager-Ziele.

<!-- t_company_destinations.xml -->

Detaillierte Informationen finden Sie unter [Ziele](https://docs.adobe.com/content/help/en/audience-manager/user-guide/features/destinations/destinations.html) im *Audience Manager-Benutzerhandbuch*.

## Unternehmensziele erstellen oder bearbeiten {#create-edit-company-destinations}

Blättern Sie durch die Abschnitte für Schritt-für-Schritt-Anweisungen, wie Sie neue [!DNL Audience Manager] Ziele erstellen oder vorhandene Ziele bearbeiten können.

<!-- create-edit-company-destinations.xml -->

Besuchen Sie die Seite [der Experience Cloud-Partnerintegration](https://wiki.corp.adobe.com/x/mPIMPw) , bevor Sie Ziele einrichten. Die Seite enthält die spezifischen Informationen, die Sie für die einzelnen [!DNL Audience Manager] Partnerintegration ausfüllen müssen.

Wenn Ihr Kunde als Ziel verwendet werden [!DNL Adobe Media Optimizer] möchte [!DNL Audience Manager] , müssen [!DNL Adobe Media Optimizer]Sie dies einrichten.

## Navigate to the Destinations Tab {#navigate-destinations}

1. Klicken **[!UICONTROL Companies]** Sie auf und suchen Sie dann das gewünschte Unternehmen, um dessen [!UICONTROL Profile] Seite anzuzeigen. Sie können das [!UICONTROL Search] Feld oder die Seitenumbruchsteuerelemente unten in der Liste verwenden, um das gewünschte Unternehmen zu finden. Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.
1. Click the **[!UICONTROL Destinations]** tab.
1. Klicken **[!UICONTROL Add Destination]** Sie auf, um ein neues Ziel zu erstellen. To edit an existing destination, click the destination's name in the **[!UICONTROL Name]** column.

## Grundlegende Einstellungen {#basic-settings}

Fill in the fields in the **[!UICONTROL Basic Settings]** window.

* **[!UICONTROL Name]:** (Erforderlich) Geben Sie den Namen dieses Ziels an.
* **[!UICONTROL Description]:** Geben Sie beschreibende Informationen zu diesem Ziel an.
* **[!UICONTROL Type]:** (Erforderlich) Wählen Sie den gewünschten Zieltyp aus:
   * **[!UICONTROL Bulk ID]**: IDs zwischen verschiedenen Plattformen synchronisieren.
   * **[!UICONTROL Bulk Trait]**: Senden Sie Eigenschaftsangaben stapelweise an verschiedene Plattformen.
   * **[!UICONTROL Bulk Segment]**: Senden Sie Segmentinformationen stapelweise an verschiedene Plattformen.
   * **[!UICONTROL S2S]**: Verwenden Sie Server-to-Server-Ziele, um Echtzeit- und Stapeldaten an verschiedene Plattformen zu senden.
* **[!UICONTROL Auto-Fill Destination Mapping]:** ( [!UICONTROL S2S] Nur) Wählen Sie eine Option aus:
   * **[!UICONTROL Segment ID]:** Wenn Sie diese Einstellung auswählen, wird die Zielwertzuordnung mit der [!DNL Audience Manager] Segment-ID ausgefüllt.
   * **[!UICONTROL Integration Code Value]:** Wenn Sie diese Einstellung auswählen, wird die Zielwertzuordnung mit dem [!DNL Audience Manager] Segmentintegrationscode gefüllt.
* **[!UICONTROL User ID Key]:** (Erforderlich) Wählen Sie in der Dropdownliste den gewünschten Benutzer-ID-Schlüssel für dieses Ziel aus.

Diese ID wird als Master-Datenquellen-ID verwendet. Dadurch werden die Benutzer-IDs, die in der Datei überschrieben werden sollen, bestimmt.

>[!NOTE]
>
>Für den [!UICONTROL Bulk ID] Zieltyp können Sie die [!DNL Audience Manager][!UICONTROL User ID] oder [!DNL Adobe Experience Cloud] die ID nicht verwenden.

Wenn Ihre Datenquellen-ID ( [!UICONTROL DPID]) nicht in der Dropdown-Liste angezeigt wird, müssen Sie das **[!UICONTROL Outbound]** Kontrollkästchen auf Datenquellenebene auf der Seite ["Datenquelleneinstellungen" aktivieren](https://docs.adobe.com/content/help/en/audience-manager/user-guide/features/data-sources/manage-datasources.html).

* **[!UICONTROL Target Data Source]:** (Erforderlich) Wählen Sie in der Dropdownliste die gewünschte Datenquelle für dieses Ziel aus. Diese Einstellung ermöglicht die Beschriftung von verstrichenen Daten, wodurch die Kunden die Seite in separate Systeme erfassen können.
* **[!UICONTROL Foreign Account ID]:** Geben Sie die Fremdkonto-ID für dieses Ziel an. Dies ist der Identifikationswert im System des Empfängers für diese verstrichenen Daten.
* **[!UICONTROL Outbound Sample Rate Denominator]:** Wenn die Gesamtsumme der zurückgegebenen Daten unbekannt ist, verwenden Sie diese Einstellung, um nur eine Beispielmenge an Daten zurückzugeben, nicht den vollen Betrag. Passen Sie die Zahl hier an, um einen Bruchteil der Daten darzustellen (d. h. der Wert ' 100 ' gibt 1/100. die normale Datenmenge zurück, der Wert ' 10 ' gibt also 1/10. die normale Datenmenge zurück). Der Standardwert ist "1" , der alle Daten zurückgibt.

## Echtzeitdaten (für S 2 S-Ziele) {#realtime-s2s}

Wenn Sie ein [!UICONTROL S2S] Ziel erstellen, füllen Sie die folgenden Felder aus:

**[!UICONTROL Servers]**: Wählen Sie den gewünschten `HTTP` Server für dieses Ziel aus.
**[!UICONTROL Format]**: Wählen Sie in der Dropdownliste das gewünschte Format für dieses Ziel aus: [!UICONTROL HTTP only].

>[!NOTE]
>
>Sie [!DNL S2S] können nur ein [!UICONTROL Realtime] oder [!UICONTROL Batch] mehrere Ziele aktivieren oder deaktivieren, indem Sie den "Aus/Bei" -Regler verwenden. Beide Optionen können nicht deaktiviert werden.

## Stapeldaten {#batch-data}

Füllen Sie für [!UICONTROL Bulk ID]oder [!UICONTROL Bulk Trait][!UICONTROL Bulk Segment] Ziele die folgenden Felder aus:

* **[!UICONTROL Protocol]**: (Erforderlich) Wählen Sie in der Dropdownliste das gewünschte Protokoll für dieses Ziel aus:
   * **[!UICONTROL FTP]**
   * **[!UICONTROL HTTP]**
   * **[!UICONTROL S3]**
* **[!UICONTROL Servers]**: (Erforderlich) Wählen Sie in der Dropdownliste den gewünschten Server für dieses Ziel aus.
* **[!UICONTROL Format]**: (Erforderlich) Wählen Sie in der Dropdownliste das gewünschte Format für dieses Ziel aus: [!DNL HTTP] oder Dateityp je nach ausgewähltem Protokoll.
* **[!UICONTROL Sync Type]**: (Erforderlich) Wählen Sie den gewünschten Synchronisierungstyp für dieses Ziel aus. Dies zeigt die Ebene der Benutzeraktivitäten an, die Kunden in die ausgehenden Bestellungen einbeziehen möchten. Auswählen, **[!UICONTROL Customer]** wenn Kunden lediglich an der Analyse von Segmentqualifizierungen aus ihren Eigenschaften interessiert sind. Wählen **[!UICONTROL Platform]** Sie aus, ob sie Segmentqualifizierung aus Offsite-Aktivitäten für alle [!DNL Audience Manager] Kunden einbeziehen möchten.
* **[!UICONTROL Customer]**: Datei enthält aktive Benutzer mit mindestens 1 Eigenschaften, die nur auf den Eigenschaften des Kunden (im Zusammenhang mit dem Client) während [!UICONTROL PID]des ausgewählten Zeitraums vorliegen. Ihre Kunden sollten diese Option verwenden, um ihre *Echtzeit-Segmentqualifikationen* an Ziele auszulösen.
* **[!UICONTROL Platform]**: Datei enthält aktive Benutzer mit mindestens 1 Echtzeit-Interaktion, deren ID-Synchronisierung oder -eigenschaften für den ausgewählten Zeitraum an allen [!DNL Audience Manager] Client-Eigenschaften (mit allen Clientpids verknüpft) liegen. Ihre Kunden sollten diese Option verwenden, um ihre *gesamten* Segmentqualifikationen auf Ziele auszulösen.
* **[!UICONTROL Lifetime]**: Datei enthält aktive Benutzer, die an allen [!DNL Audience Manager] anderen Clients seit der Erstellung des Ziels angezeigt werden.
* **[!UICONTROL Sync Type Lookback Period]**: Wählen Sie einen [!UICONTROL Customer] Zeitraum [!UICONTROL Platform]aus oder wählen Sie ihn aus. Dateien enthalten aktive Benutzer für den ausgewählten Zeitraum.
Wählen Sie als Nächstes den Bestelltyp aus. Dies zeigt die Häufigkeit und den Umfang der einzelnen ausgehenden Integration mit Partnern an. Wählen Sie zwischen inkrementellen und vollständigen Bestellungen.
* **[!UICONTROL Incremental Scheduled Run]**: Wird bei jedem [!DNL Audience Manager] Ausführen nur die Net-neuen Benutzer ausgehende, die seit der vorherigen ausgehende Bestellung qualifiziert sind. Wählen Sie den gewünschten Zeitraum aus, in dem [!DNL Audience Manager] Sie inkrementelle Synchronisierungsprozesse durchführen möchten. Sie können beispielsweise alle 24 Stunden, alle sieben Tage, alle 30 Tage oder nie auswählen.

>[!NOTE] {important = "high"}
>
>Die erste inkrementelle Reihenfolge entspricht einer vollständigen Reihenfolge, da keine früheren Benutzer an das Ziel gesendet wurden.

* **[!UICONTROL Full Sync Scheduled Run]**: Bei jedem Vorgang [!DNL Audience Manager] werden alle aktiven Benutzer nach dem ersten Einrichten des Ziels ausgehende ausgehende. Wählen Sie den gewünschten Zeitplan aus, der zur [!DNL Audience Manager] Durchführung vollständiger Synchronisierungsprozesse verwendet werden soll. Sie können beispielsweise alle 24 Stunden, alle sieben Tage, alle 30 Tage oder nie auswählen.

>[!NOTE] {important = "high"}
>
>Es wird empfohlen, inkrementelle Synchronisierungen häufiger als vollständige Synchronisierungen zu verwenden. Inkrementelle Synchronisierungen senden nur Dateien, die neue Eigenschaften für Eigenschaften oder Ids enthalten. Vollständige Synchronisierungen senden alle Dateien, unabhängig davon, ob sie neue Realizationen oder ID-Synchronisierungen enthalten. Verwenden Sie nur dann die [!UICONTROL Full Sync Scheduled Run] Konfiguration, wenn Kunden eine vollständige Kopie aller Benutzer benötigen, um das ausgehende Datenvolumen zu reduzieren.

## Datenquellen konfigurieren {#configure-data-sources}

Füllen Sie für [!UICONTROL Bulk ID]oder [!UICONTROL Bulk Trait][!UICONTROL Bulk Segment] Ziele die unten stehenden Felder aus. Mit diesen Einstellungen können Sie alle mit den Datenquellen verknüpften Daten (Eigenschaften, Segmente oder IDs) senden.

* **[!UICONTROL All Unrestricted First Party Data]**: Wählen Sie diese Option, um alle Erstanbieter-Datenquellen zu verwenden. Wenn Sie diese Option auswählen, sind die [!UICONTROL Available Data Sources] Optionen deaktiviert.
* **[!UICONTROL Available Data Sources]**: Verwenden Sie die Pfeile, um Datenquellen zwischen den **[!UICONTROL Available Data Sources]** Feldern und **[!UICONTROL In File Data Sources]** den Feldern zu verschieben.

## Speichern und abschließen {#save-and-finalize}

Die **[!UICONTROL Save]** Schaltfläche wird nach dem Ausfüllen aller erforderlichen Felder aktiviert. Klicken **[!UICONTROL Save]** Sie auf, um den Erstellungszielprozess abzuschließen.

## Unternehmensziele löschen {#delete-company-destinations}

<!-- delete-company-destinations.xml -->

So löschen Sie ein Ziel

1. Klicken **[!UICONTROL Companies]** Sie auf, suchen Sie das gewünschte Unternehmen und klicken Sie auf die **[!UICONTROL Destinations]** Registerkarte.
1. Klicken ![](assets/icon_delete.png) Sie in die **[!UICONTROL Actions]** Spalte des gewünschten Ziels.
1. Klicken Sie auf **[!UICONTROL OK], um den Löschvorgang zu bestätigen.**

>[!NOTE]
>
>Ein Ziel kann nicht gelöscht werden, wenn ihm Segmente zugeordnet sind.