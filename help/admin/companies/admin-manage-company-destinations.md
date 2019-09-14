---
description: Erstellen, bearbeiten und löschen Sie Audience Manager-Ziele.
seo-description: Erstellen, bearbeiten und löschen Sie Audience Manager-Ziele.
seo-title: Unternehmensziele verwalten
title: Unternehmensziele verwalten
uuid: d9a6bfb1-7629-44e0-b7d7-ece44f65ea2b
translation-type: tm+mt
source-git-commit: 57d7a92265e565b6c411e4cfa5c579e40eb837b3

---


# Unternehmensziele verwalten {#manage-company-destinations}

Erstellen, bearbeiten und löschen Sie Audience Manager-Ziele.

<!-- t_company_destinations.xml -->

Ausführliche Informationen finden Sie unter [Ziele](https://docs.adobe.com/content/help/en/audience-manager/user-guide/features/destinations/destinations.html) im *Audience Manager-Benutzerhandbuch*.

## Unternehmensziele erstellen oder bearbeiten {#create-edit-company-destinations}

Blättern Sie durch die Abschnitte, um schrittweise Anweisungen zum Erstellen neuer [!DNL Audience Manager] Ziele oder Bearbeiten vorhandener Ziele zu erhalten.

<!-- create-edit-company-destinations.xml -->

Besuchen Sie die Seite[ zur ](https://wiki.corp.adobe.com/x/mPIMPw)Experience Cloud-Partnerintegration, bevor Sie Ziele einrichten. Die Seite enthält die spezifischen Informationen, die Sie für jede [!DNL Audience Manager] Partnerintegration eingeben müssen.

Wenn Ihr Client [!DNL Adobe Media Optimizer] als Ziel in verwenden möchte [!DNL Audience Manager] , müssen Sie dies in einrichten [!DNL Adobe Media Optimizer].

## Navigate to the Destinations Tab {#navigate-destinations}

1. Klicken Sie auf **[!UICONTROL Companies]**, suchen Sie das gewünschte Unternehmen und klicken Sie darauf, um die zugehörige [!UICONTROL Profile] Seite anzuzeigen. Sie können das gewünschte Unternehmen über das [!UICONTROL Search] Feld oder die Paginierungssteuerelemente am unteren Rand der Liste suchen. Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.
1. Click the **[!UICONTROL Destinations]** tab.
1. Um ein neues Ziel zu erstellen, klicken Sie auf **[!UICONTROL Add Destination]**. To edit an existing destination, click the destination's name in the **[!UICONTROL Name]** column.

## Grundlegende Einstellungen {#basic-settings}

Fill in the fields in the **[!UICONTROL Basic Settings]** window.

* **[!UICONTROL Name]** : (Erforderlich) Geben Sie den Namen dieses Ziels an.
* **[!UICONTROL Description]** : Geben Sie beschreibende Informationen zu diesem Ziel an.
* **[!UICONTROL Type]** : (Erforderlich) Wählen Sie den gewünschten Zieltyp aus:
   * **[!UICONTROL Bulk ID]**: Synchronisieren Sie IDs zwischen verschiedenen Plattformen.
   * **[!UICONTROL Bulk Trait]**: Senden Sie Eigenschaftsinformationen stapelweise an verschiedene Plattformen.
   * **[!UICONTROL Bulk Segment]**: Segmentinformationen stapelweise an verschiedene Plattformen senden
   * **[!UICONTROL S2S]**: Verwenden Sie Server-zu-Server-Ziele, um Echtzeit- und Stapeldaten an verschiedene Plattformen zu senden.
* **[!UICONTROL Auto-Fill Destination Mapping]** : ( [!UICONTROL S2S] nur) Wählen Sie eine Option:
   * **[!UICONTROL Segment ID]** : Wenn Sie diese Einstellung auswählen, wird die Zuordnung des Zielwerts mit der [!DNL Audience Manager] Segment-ID gefüllt.
   * **[!UICONTROL Integration Code Value]** : Wenn Sie diese Einstellung auswählen, wird die Zuordnung des Zielwerts mit dem [!DNL Audience Manager] Segmentintegrationscode gefüllt.
* **[!UICONTROL User ID Key]** : (Erforderlich) Wählen Sie den gewünschten Benutzer-ID-Schlüssel für dieses Ziel aus der Dropdownliste aus.

Diese ID wird als Master-Datenquellen-ID verwendet. Dadurch werden die Benutzer-IDs festgelegt, die in der Datei ausgebrochen werden sollen.

>[!NOTE]
>
>Für den [!UICONTROL Bulk ID] Zieltyp können Sie die [!DNL Audience Manager] oder die [!UICONTROL User ID] [!DNL Adobe Experience Cloud] ID nicht verwenden.

Wenn Ihre Datenquellen-ID ( [!UICONTROL DPID]) nicht in der Dropdownliste angezeigt wird, müssen Sie das **[!UICONTROL Outbound]** Kontrollkästchen auf der Ebene der Datenquelle auf der Seite[" ](https://docs.adobe.com/content/help/en/audience-manager/user-guide/features/data-sources/manage-datasources.html)Datenquelleneinstellungen"aktivieren.

* **[!UICONTROL Target Data Source]** : (Erforderlich) Wählen Sie die gewünschte Datenquelle für dieses Ziel aus der Dropdownliste aus. Diese Einstellung ermöglicht die Kennzeichnung von Daten, die außerhalb des Datums liegen, was die Aufnahme in separate Systeme auf der Seite des Kunden ermöglicht.
* **[!UICONTROL Foreign Account ID]** : Geben Sie die ausländische Konto-ID für dieses Ziel an. Dies ist der Identifizierungswert im System des Empfängers für diese ausgehenden Daten.
* **[!UICONTROL Outbound Sample Rate Denominator]** : Wenn die Gesamtanzahl der zurückgegebenen Daten unbekannt ist, geben Sie mit dieser Einstellung nur eine Beispieldatenmenge und nicht den vollen Betrag zurück. Passen Sie die Zahl hier an, um einen Bruchteil der Daten zu repräsentieren (z. B. gibt der Wert "100"das 1/100. fache der regulären Datenmenge zurück, der Wert "10"gibt das 1/10-fache der regulären Datenmenge zurück). Der Standardwert ist "1", der alle Daten zurückgibt.

## Echtzeitdaten (für S2S-Ziele) {#realtime-s2s}

Wenn Sie ein [!UICONTROL S2S] Ziel erstellen, füllen Sie die folgenden Felder aus:

**[!UICONTROL Servers]**: Wählen Sie den gewünschten `HTTP` Server für dieses Ziel aus.
**[!UICONTROL Format]**: Wählen Sie das gewünschte Format für dieses Ziel aus der Dropdownliste aus: [!UICONTROL HTTP only].

>[!NOTE]
>
>Mit den Schiebereglern "Aus/An"im Anzeigebereich können Sie [!DNL S2S] nur Ziele aktivieren [!UICONTROL Realtime] oder deaktivieren [!UICONTROL Batch] . Beide Optionen können nicht deaktiviert werden.

## Stapeldaten {#batch-data}

Füllen Sie für [!UICONTROL Bulk ID]Ziele [!UICONTROL Bulk Trait] oder [!UICONTROL Bulk Segment] Ziele die folgenden Felder aus:

* **[!UICONTROL Protocol]**: (Erforderlich) Wählen Sie aus der Dropdownliste das gewünschte Protokoll für dieses Ziel aus:
   * **[!UICONTROL FTP]**
   * **[!UICONTROL HTTP]**
   * **[!UICONTROL S3]**
* **[!UICONTROL Servers]**: (Erforderlich) Wählen Sie in der Dropdownliste den gewünschten Server für dieses Ziel aus.
* **[!UICONTROL Format]**: (Erforderlich) Wählen Sie aus der Dropdownliste das gewünschte Format für dieses Ziel aus: [!DNL HTTP] oder Dateityp, je nach dem oben gewählten Protokoll.
* **[!UICONTROL Sync Type]**: (Erforderlich) Wählen Sie den gewünschten Synchronisierungstyp für dieses Ziel aus. Dies zeigt die Ebene der Benutzeraktivitäten an, die Kunden in die ausgehenden Bestellungen aufnehmen möchten. Wählen Sie diese Option, **[!UICONTROL Customer]** wenn Kunden nur daran interessiert sind, Segmentqualifikationen anhand ihrer Eigenschaften zu analysieren. Wählen Sie **[!UICONTROL Platform]** aus, ob Sie die Segmentqualifikationen von Aktivitäten außerhalb des Standorts für alle [!DNL Audience Manager] Kunden einbeziehen möchten.
* **[!UICONTROL Customer]**: Datei enthält aktive Benutzer, die mindestens 1 Eigenschaftenrealisierung für den ausgewählten Zeitraum nur auf den Eigenschaften des Kunden (verknüpft mit den Eigenschaften des Kunden [!UICONTROL PID]) haben. Ihre Kunden sollten diese Option verwenden, um ihre *Echtzeit* -Segmentqualifikationen an Ziele auszuleiten.
* **[!UICONTROL Platform]**: Datei enthält aktive Benutzer, die mindestens 1 Echtzeit-Interaktion haben, sei es ID-Synchronisierung oder Eigenschaftenrealisierung, an einer beliebigen Stelle in den Eigenschaften aller [!DNL Audience Manager] Clients (die mit allen Client-PIDs verknüpft sind) im ausgewählten Zeitraum. Ihre Kunden sollten diese Option verwenden, um ihre *gesamten* Segmentqualifikationen an Ziele auszuleiten.
* **[!UICONTROL Lifetime]**: Datei enthält aktive Benutzer, die seit der Erstellung des Ziels überall auf den Eigenschaften aller [!DNL Audience Manager] Clients zu sehen sind.
* **[!UICONTROL Sync Type Lookback Period]**: Wenn Sie einen Zeitraum auswählen [!UICONTROL Customer] oder [!UICONTROL Platform]auswählen, wählen Sie einen Zeitraum aus. Dateien enthalten aktive Benutzer für den ausgewählten Zeitraum.
Wählen Sie als Nächstes den Bestelltyp aus. Dies zeigt die Häufigkeit und den Umfang jeder ausgehenden Integration mit Partnern. Wählen Sie zwischen inkrementellen und vollständigen Bestellungen.
* **[!UICONTROL Incremental Scheduled Run]**: Bei jeder Ausführung [!DNL Audience Manager] werden nur die neuen Netto-Benutzer ausgeliefert, die seit der vorherigen ausgehenden Bestellung qualifiziert sind. Wählen Sie den gewünschten Zeitraum aus, in dem Sie inkrementelle Synchronisierungsprozesse durchführen [!DNL Audience Manager] möchten. Sie können beispielsweise alle 24 Stunden, alle 7 Tage, alle 30 Tage oder nie auswählen.

>[!NOTE] {important="high"}
>
>Die erste inkrementelle Bestellung entspricht einer vollständigen Bestellung, da noch nie zuvor Benutzer an das Ziel gesendet wurden.

* **[!UICONTROL Full Sync Scheduled Run]**: Bei jeder Ausführung [!DNL Audience Manager] werden alle aktiven Benutzer ab der Einrichtung des Ziels ausgesendet. Wählen Sie den gewünschten Zeitplan aus, den Sie [!DNL Audience Manager] zum Durchführen vollständiger Synchronisierungsprozesse verwenden möchten. Sie können beispielsweise alle 24 Stunden, alle 7 Tage, alle 30 Tage oder nie auswählen.

>[!NOTE] {important="high"}
>
>Es wird empfohlen, inkrementelle Syncs häufiger zu verwenden als vollständige Synchronisierungen. Inkrementelle Synchronisierungen senden nur Dateien, die neue Eigenschaften oder ID-Synchronisierungen enthalten. Volle Synchronisierungen senden alle Dateien, unabhängig davon, ob sie neue Realisierungen oder ID-Synchronisierungen enthalten. Verwenden Sie die [!UICONTROL Full Sync Scheduled Run] Konfiguration nur, wenn Kunden eine vollständige Kopie aller ihrer Benutzer benötigen, um das Volumen der ausgehenden Daten zu reduzieren.

## Data Sources konfigurieren {#configure-data-sources}

Füllen Sie für [!UICONTROL Bulk ID][!UICONTROL Bulk Trait] oder [!UICONTROL Bulk Segment] Ziele die folgenden Felder aus. Mit diesen Einstellungen können Sie alle mit den Datenquellen verknüpften Daten (Eigenschaften, Segmente oder IDs, je nach ausgewähltem Typ) senden.

* **[!UICONTROL All Unrestricted First Party Data]**: Wählen Sie diese Option, um alle Erstanbieter-Datenquellen zu verwenden. Wenn Sie diese Option auswählen, sind die [!UICONTROL Available Data Sources] Optionen deaktiviert.
* **[!UICONTROL Available Data Sources]**: Verwenden Sie die Pfeile, um Datenquellen zwischen den Feldern **[!UICONTROL Available Data Sources]** und **[!UICONTROL In File Data Sources]** zu verschieben.

## Speichern und Fertig stellen {#save-and-finalize}

Die **[!UICONTROL Save]** Schaltfläche wird aktiviert, nachdem alle erforderlichen Felder ausgefüllt wurden. Klicken Sie auf , **[!UICONTROL Save]** um den Prozess zum Erstellen des Ziels abzuschließen.

## Unternehmensziele löschen {#delete-company-destinations}

<!-- delete-company-destinations.xml -->

So löschen Sie ein Ziel:

1. Klicken Sie auf **[!UICONTROL Companies]**, suchen Sie das gewünschte Unternehmen und klicken Sie dann auf die **[!UICONTROL Destinations]** Registerkarte.
1. Klicken Sie ![](assets/icon_delete.png) in die **[!UICONTROL Actions]** Spalte des gewünschten Ziels.
1. Klicken Sie auf **[!UICONTROL OK], um den Löschvorgang zu bestätigen.**

>[!NOTE]
>
>Ein Ziel kann nicht gelöscht werden, wenn ihm Segmente zugeordnet sind.