---
description: Erstellen, bearbeiten und löschen Sie Audience Manager-Ziele.
seo-description: Erstellen, bearbeiten und löschen Sie Audience Manager-Ziele.
seo-title: Verwalten von Firmenzielen
title: Verwalten von Firmenzielen
uuid: d9a6bfb1-7629-44e0-b7d7-ece44f65ea2b
translation-type: tm+mt
source-git-commit: f247457004a624297ddc8847dd256dbb7d8da418
workflow-type: tm+mt
source-wordcount: '1082'
ht-degree: 1%

---


# Verwalten von Firmenzielen {#manage-company-destinations}

Erstellen, bearbeiten und löschen Sie Audience Manager-Ziele.

<!-- t_company_destinations.xml -->

Ausführliche Informationen finden Sie unter [Ziele](https://docs.adobe.com/content/help/en/audience-manager/user-guide/features/destinations/destinations.html) im *Audience Manager-Benutzerhandbuch*.

## Erstellen oder Bearbeiten von Firmenzielen {#create-edit-company-destinations}

Blättern Sie durch die Abschnitte, um schrittweise Anweisungen zum Erstellen neuer [!DNL Audience Manager]-Ziele oder Bearbeiten vorhandener Ziele zu erhalten.

<!-- create-edit-company-destinations.xml -->

Rufen Sie die [Experience Cloud-Partnerintegrationsseite](https://wiki.corp.adobe.com/x/mPIMPw) auf, bevor Sie Ziele einrichten. Die Seite enthält die spezifischen Informationen, die Sie für jede [!DNL Audience Manager] Partnerintegration eingeben müssen.

Wenn Ihr Client [!DNL Adobe Media Optimizer] als Ziel in [!DNL Audience Manager] verwenden möchte, müssen Sie dies in [!DNL Adobe Media Optimizer] einrichten.

## Navigieren Sie zum Register Ziele {#navigate-destinations}

1. Klicken Sie auf **[!UICONTROL Companies]**, suchen Sie die gewünschte Firma und klicken Sie darauf, um deren [!UICONTROL Profile]-Seite anzuzeigen. Sie können das Feld [!UICONTROL Search] oder die Paginierungssteuerelemente am unteren Rand der Liste verwenden, um die gewünschte Firma zu finden. Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Destinations]**.
1. Um ein neues Ziel zu erstellen, klicken Sie auf **[!UICONTROL Add Destination]**. Um ein vorhandenes Ziel zu bearbeiten, klicken Sie in der Spalte **[!UICONTROL Name]** auf den Namen des Ziels.

## Grundlegende Einstellungen {#basic-settings}

Füllen Sie die Felder im Fenster **[!UICONTROL Basic Settings]** aus.

* **[!UICONTROL Name]:** (Erforderlich) Geben Sie den Namen dieses Ziels an.
* **[!UICONTROL Description]:** Geben Sie beschreibende Informationen zu diesem Ziel an.
* **[!UICONTROL Type]:** (Erforderlich) Wählen Sie den gewünschten Zieltyp aus:
   * **[!UICONTROL Bulk ID]**: Synchronisieren Sie IDs zwischen verschiedenen Plattformen.
   * **[!UICONTROL Bulk Trait]**: Senden Sie Eigenschaftsinformationen stapelweise an verschiedene Plattformen.
   * **[!UICONTROL Bulk Segment]**: Segmentinformationen stapelweise an verschiedene Plattformen senden
   * **[!UICONTROL S2S]**: Verwenden Sie Server-zu-Server-Ziele, um Echtzeit- und Stapeldaten an verschiedene Plattformen zu senden.
* **[!UICONTROL Auto-Fill Destination Mapping]:** (  [!UICONTROL S2S] Nur) Wählen Sie eine Option aus:
   * **[!UICONTROL Segment ID]:** Wenn Sie diese Einstellung auswählen, wird die Zuordnung des Zielwerts mit der  [!DNL Audience Manager] Segment-ID ausgefüllt.
   * **[!UICONTROL Integration Code Value]:** Wenn Sie diese Einstellung auswählen, wird die Zuordnung des Zielwerts mit dem  [!DNL Audience Manager] Segmentintegrationscode gefüllt.
* **[!UICONTROL User ID Key]:** (Erforderlich) Wählen Sie in der Dropdown-Liste den gewünschten Benutzer-ID-Schlüssel für dieses Ziel aus.

Diese ID wird als Übergeordnet-Datenquellen-ID verwendet. Dadurch werden die Benutzer-IDs festgelegt, die in der Datei ausgebrochen werden sollen.

>[!NOTE]
>
>Für den Zieltyp [!UICONTROL Bulk ID] können Sie weder die ID [!DNL Audience Manager] [!UICONTROL User ID] noch die ID [!DNL Adobe Experience Cloud] verwenden.

Wenn Ihre Datenquellen-ID ( [!UICONTROL DPID]) nicht in der Dropdown-Liste angezeigt wird, müssen Sie das Kontrollkästchen **[!UICONTROL Outbound]** auf der Datenquellenebene auf der Seite [Datenquelleneinstellungen](https://docs.adobe.com/content/help/en/audience-manager/user-guide/features/data-sources/manage-datasources.html) aktivieren.

* **[!UICONTROL Target Data Source]:** (Erforderlich) Wählen Sie in der Dropdown-Liste die gewünschte Datenquelle für dieses Ziel aus. Diese Einstellung ermöglicht die Kennzeichnung von Daten, die außerhalb des Datums liegen, was die Aufnahme in separate Systeme auf der Seite des Kunden ermöglicht.
* **[!UICONTROL Foreign Account ID]:** Geben Sie die ausländische Konto-ID für dieses Ziel an. Dies ist der Identifizierungswert im System des Empfängers für diese ausgehenden Daten.
* **[!UICONTROL Outbound Sample Rate Denominator]&lt;** Wenn die Gesamtanzahl der zurückgegebenen Daten unbekannt ist, geben Sie mit dieser Einstellung nur eine Beispieldatenmenge und nicht den vollen Betrag zurück. Passen Sie die Zahl hier an, um einen Bruchteil der Daten zu repräsentieren (z. B. gibt der Wert &quot;100&quot;das 1/100. fache der regulären Datenmenge zurück, der Wert &quot;10&quot;gibt das 1/10-fache der regulären Datenmenge zurück). Der Standardwert ist &quot;1&quot;, der alle Daten zurückgibt.

## Echtzeitdaten (für S2S-Ziele) {#realtime-s2s}

Wenn Sie ein [!UICONTROL S2S]-Ziel erstellen, füllen Sie die folgenden Felder aus:

**[!UICONTROL Servers]**: Wählen Sie den gewünschten  `HTTP` Server für dieses Ziel aus.
**[!UICONTROL Format]**: Wählen Sie in der Dropdown-Liste das gewünschte Format für dieses Ziel aus:  [!UICONTROL HTTP only].

>[!NOTE]
>
>Nur für [!DNL S2S] können Sie entweder [!UICONTROL Realtime]- oder [!UICONTROL Batch]-Ziele mithilfe der Schieberegler &quot;Aus/Ein&quot;auf dem Bildschirm aktivieren oder deaktivieren. Beide Optionen können nicht deaktiviert werden.

## Stapeldaten {#batch-data}

Füllen Sie für [!UICONTROL Bulk ID]-, [!UICONTROL Bulk Trait]- oder [!UICONTROL Bulk Segment]-Ziele die folgenden Felder aus:

* **[!UICONTROL Protocol]**: (Erforderlich) Wählen Sie in der Dropdown-Liste das gewünschte Protokoll für dieses Ziel aus:
   * **[!UICONTROL FTP]**
   * **[!UICONTROL HTTP]**
   * **[!UICONTROL S3]**
* **[!UICONTROL Servers]**: (Erforderlich) Wählen Sie in der Dropdown-Liste den gewünschten Server für dieses Ziel aus.
* **[!UICONTROL Format]**: (Erforderlich) Wählen Sie in der Dropdown-Liste das gewünschte Format für dieses Ziel aus:  [!DNL HTTP] oder Dateityp, abhängig vom oben gewählten Protokoll.
* **[!UICONTROL Sync Type]**: (Erforderlich) Wählen Sie den gewünschten Synchronisierungstyp für dieses Ziel aus. Dies zeigt die Aktivitäten an, die Kunden bei ausgehenden Bestellungen berücksichtigen möchten. Wählen Sie **[!UICONTROL Customer]**, wenn Kunden nur daran interessiert sind, die Segmentqualifikationen anhand ihrer Eigenschaften zu analysieren. Wählen Sie **[!UICONTROL Platform]** aus, wenn Segmentqualifikationen von Offsite-Aktivitäten für alle [!DNL Audience Manager]-Kunden einbezogen werden sollen.
* **[!UICONTROL Customer]**: Datei enthält aktive Benutzer, die mindestens 1 Eigenschaftenrealisierung für den ausgewählten Zeitraum nur auf den Eigenschaften des Kunden (verknüpft mit den Eigenschaften des Kunden  [!UICONTROL PID]) haben. Ihre Kunden sollten diese Option verwenden, um ihre *Echtzeit*-Segmentqualifikationen an Ziele auszuleiten.
* **[!UICONTROL Platform]**: Datei enthält aktive Benutzer, die mindestens 1 Echtzeit-Interaktion haben, sei es ID-Synchronisierung oder Eigenschaftenrealisierung, an einer beliebigen Stelle in den Eigenschaften aller  [!DNL Audience Manager] Clients (die mit allen Client-PIDs verknüpft sind) während des ausgewählten Zeitraums. Ihre Kunden sollten diese Option verwenden, um ihre Qualifikationen für *Gesamtsegmente* an Ziele auszuleiten.
* **[!UICONTROL Lifetime]**: Datei enthält aktive Benutzer, die seit der Erstellung des Ziels überall auf den Eigenschaften aller  [!DNL Audience Manager] Clients zu sehen sind.
* **[!UICONTROL Sync Type Lookback Period]**: Wenn Sie einen Zeitraum auswählen  [!UICONTROL Customer] oder  [!UICONTROL Platform]auswählen, wählen Sie einen Zeitraum aus. Dateien enthalten aktive Benutzer für den ausgewählten Zeitraum.
Wählen Sie als Nächstes den Bestelltyp aus. Dies zeigt die Häufigkeit und den Umfang jeder ausgehenden Integration mit Partnern an. Wählen Sie zwischen inkrementellen und vollständigen Bestellungen.
* **[!UICONTROL Incremental Scheduled Run]**: Bei jeder Ausführung  [!DNL Audience Manager] werden nur die neuen Netto-Benutzer ausgeliefert, die sich seit der letzten ausgehenden Bestellung qualifiziert haben. Wählen Sie den gewünschten Zeitraum aus, für den [!DNL Audience Manager] inkrementelle Synchronisierungsprozesse durchführen soll. Sie können beispielsweise alle 24 Stunden, alle 7 Tage, alle 30 Tage oder nie auswählen.

<!--
I removed {importance="high"} from note for Exp League rendering. -Bob
-->

>[!NOTE]
>
>Die erste inkrementelle Bestellung entspricht einer vollständigen Bestellung, da noch nie zuvor Benutzer an das Ziel gesendet wurden.

* **[!UICONTROL Full Sync Scheduled Run]**: Bei jeder Ausführung  [!DNL Audience Manager] werden alle aktiven Benutzer ab der Einrichtung des Ziels ausgesendet. Wählen Sie den gewünschten Zeitplan aus, den [!DNL Audience Manager] zum Durchführen vollständiger Synchronisierungsprozesse verwenden soll. Sie können beispielsweise alle 24 Stunden, alle 7 Tage, alle 30 Tage oder nie auswählen.

<!--
I removed {importance="high"} from note for Exp League rendering. -Bob
-->

>[!NOTE]
>
>Es wird empfohlen, inkrementelle Syncs häufiger zu verwenden als vollständige Synchronisierungen. Inkrementelle Synchronisierungen senden nur Dateien, die neue Eigenschaften oder ID-Synchronisierungen enthalten. Volle Synchronisierungen senden alle Dateien, unabhängig davon, ob sie neue Realisierungen oder ID-Synchronisierungen enthalten. Verwenden Sie die [!UICONTROL Full Sync Scheduled Run]-Konfiguration nur, wenn Clients eine vollständige Kopie aller ihrer Benutzer benötigen, um das ausgehende Datenvolumen zu reduzieren.

## Data Sources konfigurieren {#configure-data-sources}

Füllen Sie für [!UICONTROL Bulk ID]-, [!UICONTROL Bulk Trait]- oder [!UICONTROL Bulk Segment]-Ziele die folgenden Felder aus. Mit diesen Einstellungen können Sie alle mit den Datenquellen verknüpften Daten (Eigenschaften, Segmente oder IDs, je nach ausgewähltem Typ) senden.

* **[!UICONTROL All Unrestricted First Party Data]**: Wählen Sie diese Option, um alle Erstanbieter-Datenquellen zu verwenden. Wenn Sie diese Option auswählen, sind die [!UICONTROL Available Data Sources]-Optionen deaktiviert.
* **[!UICONTROL Available Data Sources]**: Verwenden Sie die Pfeile, um Datenquellen zwischen den Feldern  **[!UICONTROL Available Data Sources]** und  **[!UICONTROL In File Data Sources]** zu verschieben.

## Speichern und Fertigstellen von {#save-and-finalize}

Die Schaltfläche **[!UICONTROL Save]** wird aktiviert, nachdem alle erforderlichen Felder ausgefüllt wurden. Klicken Sie auf **[!UICONTROL Save]**, um den Prozess zum Erstellen des Ziels abzuschließen.

## Firmen-Ziele {#delete-company-destinations} löschen

<!-- delete-company-destinations.xml -->

So löschen Sie ein Ziel:

1. Klicken Sie auf **[!UICONTROL Companies]**, suchen Sie die gewünschte Firma und klicken Sie dann auf die Registerkarte **[!UICONTROL Destinations]**.
1. Klicken Sie in der Spalte **[!UICONTROL Actions]** des gewünschten Ziels auf ![](assets/icon_delete.png).
1. Klicken Sie auf **[!UICONTROL OK]**, um den Löschvorgang zu bestätigen.

>[!NOTE]
>
>Ein Ziel kann nicht gelöscht werden, wenn ihm Segmente zugeordnet sind.