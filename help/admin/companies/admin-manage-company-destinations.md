---
description: Erstellen, bearbeiten und löschen Sie Audience Manager-Ziele.
seo-description: Erstellen, bearbeiten und löschen Sie Audience Manager-Ziele.
seo-title: Verwalten von Firmenzielen
title: Verwalten von Firmenzielen
uuid: d9a6bfb1-7629-44e0-b7d7-ece44f65ea2b
exl-id: a2e73613-07cd-4ab8-8c6e-be451ed50bfc
source-git-commit: f5d74995f0664cf63e68b46f1f3c608f34df0e80
workflow-type: tm+mt
source-wordcount: '1082'
ht-degree: 1%

---

# Verwalten von Firmenzielen {#manage-company-destinations}

Erstellen, bearbeiten und löschen Sie Audience Manager-Ziele.

<!-- t_company_destinations.xml -->

Detaillierte Informationen finden Sie unter [Ziele](https://docs.adobe.com/content/help/en/audience-manager/user-guide/features/destinations/destinations.html) im *Audience Manager-Benutzerhandbuch*.

## Erstellen oder Bearbeiten von Firmenzielen {#create-edit-company-destinations}

Scrollen Sie durch die Abschnitte, um schrittweise Anweisungen zum Erstellen neuer [!DNL Audience Manager]-Ziele oder Bearbeiten vorhandener Ziele zu erhalten.

<!-- create-edit-company-destinations.xml -->

Besuchen Sie die Seite [Experience Cloud-Partnerintegration](https://wiki.corp.adobe.com/x/mPIMPw) , bevor Sie Ziele einrichten. Die Seite enthält die spezifischen Informationen, die Sie für jede [!DNL Audience Manager] Partnerintegration ausfüllen müssen.

Wenn Ihr Client [!DNL Adobe Media Optimizer] als Ziel in [!DNL Audience Manager] verwenden möchte, müssen Sie dies in [!DNL Adobe Media Optimizer] einrichten.

## Navigieren Sie zur Registerkarte Ziele . {#navigate-destinations}

1. Klicken Sie auf **[!UICONTROL Companies]**, suchen Sie das gewünschte Unternehmen und klicken Sie auf das gewünschte Unternehmen, um dessen Seite [!UICONTROL Profile] anzuzeigen. Sie können das Feld [!UICONTROL Search] oder die Paginierungssteuerelemente am unteren Rand der Liste verwenden, um das gewünschte Unternehmen zu finden. Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Destinations]** .
1. Um ein neues Ziel zu erstellen, klicken Sie auf **[!UICONTROL Add Destination]**. Um ein vorhandenes Ziel zu bearbeiten, klicken Sie in der Spalte **[!UICONTROL Name]** auf den Namen des Ziels.

## Grundeinstellungen {#basic-settings}

Füllen Sie die Felder im Fenster **[!UICONTROL Basic Settings]** aus.

* **[!UICONTROL Name]:**  (Erforderlich) Geben Sie den Namen dieses Ziels an.
* **[!UICONTROL Description]:** Geben Sie beschreibende Informationen zu diesem Ziel an.
* **[!UICONTROL Type]:**  (Erforderlich) Wählen Sie den gewünschten Zieltyp aus:
   * **[!UICONTROL Bulk ID]**: IDs zwischen verschiedenen Plattformen synchronisieren.
   * **[!UICONTROL Bulk Trait]**: Senden Sie Eigenschaftsinformationen stapelweise an verschiedene Plattformen.
   * **[!UICONTROL Bulk Segment]**: Senden Sie Segmentinformationen stapelweise an verschiedene Plattformen.
   * **[!UICONTROL S2S]**: Verwenden Sie Server-zu-Server-Ziele, um Echtzeit- und Batch-Daten an verschiedene Plattformen zu senden.
* **[!UICONTROL Auto-Fill Destination Mapping]:** (  [!UICONTROL S2S] nur) Wählen Sie eine Option aus:
   * **[!UICONTROL Segment ID]:** Wenn Sie diese Einstellung auswählen, wird die Zielwert-Zuordnung mit der  [!DNL Audience Manager] Segment-ID ausgefüllt.
   * **[!UICONTROL Integration Code Value]:** Wenn Sie diese Einstellung auswählen, wird die Zielwert-Zuordnung mit dem  [!DNL Audience Manager] Segmentintegrationscode gefüllt.
* **[!UICONTROL User ID Key]:**  (Erforderlich) Wählen Sie den gewünschten Benutzer-ID-Schlüssel für dieses Ziel aus der Dropdownliste aus.

Diese ID wird als Übergeordnete Datenquellen-ID verwendet. Dadurch werden die Benutzer-IDs bestimmt, die in der Datei ausgelesen werden sollen.

>[!NOTE]
>
>Für den Zieltyp [!UICONTROL Bulk ID] können Sie die ID [!DNL Audience Manager] [!UICONTROL User ID] oder die ID [!DNL Adobe Experience Cloud] nicht verwenden.

Wenn Ihre Datenquellen-ID ( [!UICONTROL DPID]) nicht in der Dropdown-Liste angezeigt wird, müssen Sie das Kontrollkästchen **[!UICONTROL Outbound]** auf der Datenquellenebene auf der Seite [Datenquelleneinstellungen](https://docs.adobe.com/content/help/en/audience-manager/user-guide/features/data-sources/manage-datasources.html) aktivieren.

* **[!UICONTROL Target Data Source]:**  (Erforderlich) Wählen Sie die gewünschte Datenquelle für dieses Ziel aus der Dropdownliste aus. Diese Einstellung ermöglicht die Beschriftung ausgehender Daten, wodurch die Aufnahme in separate Systeme auf der Kundenseite möglich ist.
* **[!UICONTROL Foreign Account ID]:** Geben Sie die ausländische Konto-ID für dieses Ziel an. Dies ist der Identifikationswert im System des Empfängers für diese ausgehenden Daten.
* **[!UICONTROL Outbound Sample Rate Denominator]:** Wenn die Gesamtanzahl der zurückgegebenen Daten unbekannt ist, geben Sie mit dieser Einstellung nur eine Stichprobenmenge an Daten zurück, nicht den vollständigen Betrag. Passen Sie die Zahl hier an, um einen Bruchteil der Daten darzustellen (z. B. gibt der Wert &quot;100&quot;das 1/100-fache der regulären Datenmenge zurück, der Wert &quot;10&quot;gibt das 1/10-fache der regulären Datenmenge zurück). Der Standardwert ist &quot;1&quot;, der alle Daten zurückgibt.

## Echtzeitdaten (für S2S-Ziele) {#realtime-s2s}

Wenn Sie ein [!UICONTROL S2S]-Ziel erstellen, füllen Sie die folgenden Felder aus:

**[!UICONTROL Servers]**: Wählen Sie den gewünschten  `HTTP` Server für dieses Ziel aus.
**[!UICONTROL Format]**: Wählen Sie aus der Dropdown-Liste das gewünschte Format für dieses Ziel aus:  [!UICONTROL HTTP only].

>[!NOTE]
>
>Nur für [!DNL S2S] können Sie entweder [!UICONTROL Realtime]- oder [!UICONTROL Batch]-Ziele über die On-Screen Off/On-Regler aktivieren oder deaktivieren. Sie können beide Optionen nicht deaktivieren.

## Batch-Daten {#batch-data}

Füllen Sie für Ziele [!UICONTROL Bulk ID], [!UICONTROL Bulk Trait] oder [!UICONTROL Bulk Segment] die folgenden Felder aus:

* **[!UICONTROL Protocol]**: (Erforderlich) Wählen Sie aus der Dropdownliste das gewünschte Protokoll für dieses Ziel aus:
   * **[!UICONTROL FTP]**
   * **[!UICONTROL HTTP]**
   * **[!UICONTROL S3]**
* **[!UICONTROL Servers]**: (Erforderlich) Wählen Sie den gewünschten Server für dieses Ziel aus der Dropdownliste aus.
* **[!UICONTROL Format]**: (Erforderlich) Wählen Sie aus der Dropdownliste das gewünschte Format für dieses Ziel aus:  [!DNL HTTP] oder Dateityp, abhängig vom oben ausgewählten Protokoll.
* **[!UICONTROL Sync Type]**: (Erforderlich) Wählen Sie den gewünschten Synchronisierungstyp für dieses Ziel aus. Dies gibt die Ebene der Benutzeraktivitäten an, die Kunden in die ausgehenden Bestellungen aufnehmen möchten. Wählen Sie **[!UICONTROL Customer]** aus, wenn Kunden nur daran interessiert sind, Segmentqualifikationen anhand ihrer Eigenschaften zu analysieren. Wählen Sie **[!UICONTROL Platform]** aus, wenn Segmentqualifikationen aus Offsite-Aktivitäten für alle [!DNL Audience Manager]-Kunden einbezogen werden sollen.
* **[!UICONTROL Customer]**: Datei enthält aktive Benutzer, die mindestens 1 Merkmalrealisierung nur in den Eigenschaften des Kunden (verknüpft mit der des Kunden  [!UICONTROL PID]) für den ausgewählten Zeitraum haben. Ihre Kunden sollten diese Option verwenden, um ihre Segmentqualifikationen *in Echtzeit* an Ziele auszulösen.
* **[!UICONTROL Platform]**: Datei enthält aktive Benutzer mit mindestens 1 Echtzeit-Interaktion, ob ID-Synchronisierung oder Merkmalrealisierung, an einer beliebigen Stelle in den Eigenschaften aller  [!DNL Audience Manager] Clients (verknüpft mit allen Client-PIDs) für den ausgewählten Zeitraum. Ihre Kunden sollten diese Option verwenden, um ihre Segmentqualifikationen *total* an Ziele auszulösen.
* **[!UICONTROL Lifetime]**: Datei enthält aktive Benutzer, die seit der Erstellung des Ziels überall in den Eigenschaften aller  [!DNL Audience Manager] Clients angezeigt wurden.
* **[!UICONTROL Sync Type Lookback Period]**: Wenn Sie  [!UICONTROL Customer] oder  [!UICONTROL Platform]auswählen, wählen Sie einen Zeitraum aus. Dateien enthalten aktive Benutzer für den ausgewählten Zeitraum.
Wählen Sie als Nächstes den Bestelltyp aus. Dies gibt die Häufigkeit und den Umfang jeder ausgehenden Integration mit Partnern an. Wählen Sie zwischen inkrementellen und vollständigen Bestellungen aus.
* **[!UICONTROL Incremental Scheduled Run]**: Bei jeder Ausführung  [!DNL Audience Manager] werden nur die neuen, seit der vorherigen ausgehenden Bestellung qualifizierten Benutzer ausgeliefert. Wählen Sie den gewünschten Zeitraum aus, für den [!DNL Audience Manager] inkrementelle Synchronisierungsprozesse durchführen soll. Sie können beispielsweise alle 24 Stunden, alle 7 Tage, alle 30 Tage oder nie auswählen.

<!--
I removed {importance="high"} from note for Exp League rendering. -Bob
-->

>[!NOTE]
>
>Die erste inkrementelle Bestellung entspricht einer vollständigen Bestellung, da keine vorherigen Benutzer an das Ziel gesendet wurden.

* **[!UICONTROL Full Sync Scheduled Run]**: Bei jeder Ausführung  [!DNL Audience Manager] werden alle aktiven Benutzer ausgesendet, seit das Ziel zum ersten Mal eingerichtet wurde. Wählen Sie den gewünschten Zeitplan aus, den [!DNL Audience Manager] verwenden soll, um vollständige Synchronisierungsprozesse durchzuführen. Sie können beispielsweise alle 24 Stunden, alle 7 Tage, alle 30 Tage oder nie auswählen.

<!--
I removed {importance="high"} from note for Exp League rendering. -Bob
-->

>[!NOTE]
>
>Es wird empfohlen, inkrementelle Synchronisationen häufiger als vollständige Synchronisationen zu verwenden. Inkrementelle Synchronisierungen senden nur Dateien, die neue Eigenschaftsrealisierungen oder ID-Synchronisierungen enthalten. Vollständige Synchronisierungen senden alle Dateien, unabhängig davon, ob sie neue Realisierungen oder ID-Synchronisierungen enthalten. Verwenden Sie die [!UICONTROL Full Sync Scheduled Run]-Konfiguration nur, wenn Clients eine vollständige Kopie aller Benutzer benötigen, um das ausgehende Datenvolumen zu reduzieren.

## Data Sources konfigurieren {#configure-data-sources}

Füllen Sie für Ziele [!UICONTROL Bulk ID], [!UICONTROL Bulk Trait] oder [!UICONTROL Bulk Segment] die folgenden Felder aus. Mit diesen Einstellungen können Sie alle Daten (Eigenschaften, Segmente oder IDs, basierend auf dem ausgewählten Typ) senden, die mit den Datenquellen verknüpft sind.

* **[!UICONTROL All Unrestricted First Party Data]**: Wählen Sie aus, um alle Erstanbieter-Datenquellen zu verwenden. Wenn Sie diese Option auswählen, sind die [!UICONTROL Available Data Sources]-Optionen deaktiviert.
* **[!UICONTROL Available Data Sources]**: Verwenden Sie die Pfeile, um Datenquellen zwischen den Feldern  **[!UICONTROL Available Data Sources]** und  **[!UICONTROL In File Data Sources]** zu verschieben.

## Speichern und abschließen {#save-and-finalize}

Die Schaltfläche **[!UICONTROL Save]** wird aktiviert, nachdem alle erforderlichen Felder ausgefüllt wurden. Klicken Sie auf **[!UICONTROL Save]** , um den Prozess zum Erstellen des Ziels abzuschließen.

## Löschen von Firmenzielen {#delete-company-destinations}

<!-- delete-company-destinations.xml -->

So löschen Sie ein Ziel:

1. Klicken Sie auf **[!UICONTROL Companies]**, suchen Sie das gewünschte Unternehmen und klicken Sie auf die Registerkarte **[!UICONTROL Destinations]** .
1. Klicken Sie in der Spalte **[!UICONTROL Actions]** des gewünschten Ziels auf ![](assets/icon_delete.png) .
1. Klicken Sie auf **[!UICONTROL OK]**, um den Löschvorgang zu bestätigen.

>[!NOTE]
>
>Sie können ein Ziel nicht löschen, wenn ihm Segmente zugeordnet sind.
