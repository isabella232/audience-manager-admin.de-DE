---
description: Informationen, die Sie bei der Einrichtung von Zielen in Audience Manager unterstützen und allgemeine Probleme vermeiden.
seo-description: Informationen, die Sie bei der Einrichtung von Zielen in Audience Manager unterstützen und allgemeine Probleme vermeiden.
seo-title: Fehlerbehebung für Zielgruppen
title: Fehlerbehebung für Zielgruppen
uuid: 04080 fb 9-6 c 7 b -4 de 7-960 e -54482 be 2 de 83
translation-type: tm+mt
source-git-commit: 118e8fa3f35bc77846c6518268448d57d779a2ee

---


# Fehlerbehebung für Zielgruppen {#destination-setup-troubleshooting}

Informationen, die Sie bei der Einrichtung von Zielen in Audience Manager unterstützen und allgemeine Probleme vermeiden.

## Ich habe ein Ziel eingerichtet, aber keine Dateien. Wo sind sie? {#destination-no-files}

<!-- c_dest_tshooting.xml -->

Häufige Probleme bei der Zielkonfiguration sind die folgenden:

### Falsch konfiguriertes Ziel

* **Falscher[!UICONTROL UserID]Schlüssel:** Der [!UICONTROL UserID] Schlüssel ist der [!UICONTROL MasterDPID] von diesem Ziel und stellt die Basis für die ID-Werte dar, die überfallen werden. Auch wenn ein [!UICONTROL UserID] Schlüssel über die Dropdown-Liste auswählbar ist, bedeutet dies nicht notwendigerweise, dass diesem Wert IDs/Eigenschaften/Segmente zugeordnet sind. Wenn der [!UICONTROL Outbound] Prozess (der nach der Erstellung der Ziele ausgeführt wird) keine dem [!UICONTROL UserID] Schlüssel zugeordneten Benutzer findet, werden keine Daten verworfen.
* **Nein in Dateidatenquellen ausgewählt:** Wenn Sie einen anderen Zieltyp als [!UICONTROL S2S]ein anderer Zieltyp auswählen, wird unten im Bildschirm ein Abschnitt [!UICONTROL Configure Data Sources]angezeigt. Wenn dieser Abschnitt zuerst angezeigt wird, werden keine Werte ausgewählt. Wenn Sie vergessen, auf das [!UICONTROL All First Party] Kontrollkästchen zu klicken oder die Datenquellen einzeln aus dem [!UICONTROL Available Data Sources] Fenster auszuwählen, werden keine Daten verworfen.

### Falsch konfiguriertes Format

Wenn Sie ein Format für Ihre verstrichenen Daten auswählen, empfiehlt es sich, nach Möglichkeit ein vorhandenes Format erneut zu verwenden. Die Verwendung eines bereits bewährten Formats gewährleistet, dass Ihre ausgehenden Daten erfolgreich generiert werden. Um genau zu sehen, wie ein vorhandenes Format formatiert ist, klicken Sie in der Menüleiste auf die [!UICONTROL Formats] Option und suchen Sie entweder nach dem Namen oder nach der ID-Nummer nach Ihrem Format. Fehlerhafte Formate oder Makros, die in Formaten verwendet werden, liefern falsch formatierte Ausgabe oder verhindern, dass Informationen vollständig ausgegeben werden.

Weitere Informationen zum Einrichten von Formaten und zum Verwenden von Makros finden Sie unter [Dateiformat-Makros](formats/file-formats.md#) und [HTTP-Format-Makros](formats/web-formats.md).

### Falsch konfigurierter Server

* **[!DNL FTP]**
   * **[!UICONTROL Domain]**
      * Geben Sie keine Präfixe für Hostnamen ein. Wenn Sie ein Konto [!DNL ftp://hello.com]erhalten, geben [!DNL hello.com] Sie einfach in dieses Feld ein.
   * **[!UICONTROL Port/Type Combination]**
      * Für [!DNL FTP] eine Übertragung ist der bevorzugte Übertragungstyp [!DNL SFTP].
      * Bei Auswahl des [!DNL SFTP] Typs ist der Anschluss fast immer 22.
      * Bei Auswahl des [!DNL FTPs/TLS] Typs ist der Anschluss fast immer 21.
      * Der [!DNL FTPs/TLS] Typ ist nicht gleich einer regulären [!DNL FTP] Übertragung. Reguläre (ungesicherte) [!DNL FTP] Übertragungen werden nicht unterstützt.
   * **[!UICONTROL Remote Path]**
      * Wenn Sie einen Remote-Unterpfad auswählen, sollte er ohne führende Schrägstrich eingegeben werden.
      * Wenn die übertragene Datei im [!DNL (root)/inbound] Unterordner platziert werden soll, müssen Sie einfach [!DNL inbound] für den Remote-Pfad hinzufügen, nicht [!DNL /inbound]für den Remote-Pfad.
      * Wenn Sie Ihre Dateien mit mehreren Ordnern nach unten versenden, geben Sie zwischen den einzelnen Ordnern Schrägstriche ein. Wenn Sie den Speicherort von erhalten, [!DNL /inbound/subdirectory1/subdirectory2]sollten Sie in [!DNL inbound/subdirectory1/subdirectory2] dieses Feld eingeben.
      * Wenn die Datei in dem Ordner platziert werden soll, der automatisch vom externen Server weitergeleitet wird, können Sie diesen Speicherplatz leer lassen. Geben Sie keinen Punkt ein (. ), Schrägstrich (/) usw.

* **[!DNL S3]**
   * [!DNL S3] ist das bevorzugte Übertragungsprotokoll (über [!DNL FTP] oder [!DNL HTTP]).
      * **[!UICONTROL Bucket]**
         * Der Behältername sollte ohne Schrägstriche, Präfixe, Suffixe usw. aufgelistet werden. Wenn Sie die Adresse [!DNL s3://your-bucket] erhalten haben, die Sie einfach zu diesem Feld hinzufügen [!DNL your-bucket] sollten.
      * **[!UICONTROL Directory]**
         * Lassen Sie dieses Feld leer, es sei denn, Sie erhalten ausdrücklich einen Unterordner, in dem die Daten platziert werden sollen. Wenn Sie die Adresse [!DNL s3://your-bucket/your-subdirectory]erhalten, geben Sie in [!DNL your-bucket] das [!UICONTROL Bucket] Feld ein und [!DNL your-subdirectory] sollten Sie dem [!UICONTROL Directory] Feld hinzugefügt werden. Fügen Sie keine vorherigen Schrägstriche hinzu.
         * Wenn Sie mehrere Ordner nach unten verschieben müssen, sollten Sie nur Schrägstriche als Trennzeichen verwenden. Eine Position von [!DNL s3://your-bucket/your-subdirectory1/your-subdirectory2] würde sich also [!DNL your-bucket] im [!UICONTROL Bucket] Feld befinden und [!DNL your-subdirectory1/your-subdirectory2] in das [!UICONTROL Directory] Feld eingegeben werden.
      * **[!UICONTROL Access / Secret Keys]**
         * Wenn [!DNL TechOps] ein Behälter erstellt wird und Zugriff/geheimer Schlüssel einem Berater gewährt wird, sind diese Anmeldeinformationen normalerweise `READ-ONLY` Anmeldedaten, die an den Client übermittelt werden sollen. Diese Anmeldeinformationen sollten nicht in [!UICONTROL Access / Secret Key] die Felder eingegeben werden, da dadurch die Übertragung fehlschlägt (da diese Anmeldeinformationen schreibgeschützt, schreibgeschützt sind). In dem Fall, dass [!DNL TechOps] ein Behälter erstellt und Anmeldeinformationen bereitgestellt werden, sollte der Berater auch ein Adobe-Schlüsselpaar anfordern - NICHT FÜR DEN CLIENT ANGEGEBEN -, das Dateien in diesen Behälter schreibt. Dieser Schlüssel sollte zu diesen Feldern hinzugefügt werden.

* **[!DNL HTTP]**
   * **[!UICONTROL Domain]**
      * Geben Sie die Präfix-Informationen für [!DNL HTTP] Einträge ein. Wenn Sie ein Konto [!DNL https://superduper.com]erhalten, geben [!DNL https://superduper.com] Sie in dieses Feld ein.
      * **[!UICONTROL URL Prefix]**
         * Wenn Sie ein [!DNL URL] Präfix hinzufügen, lassen Sie den vorherigen Schrägstrich deaktiviert. Eine Adresse sollte [!DNL https://hello.com/r/x/y/z] in [!DNL https://hello.com] das [!UICONTROL Domain] Feld eingegeben und [!DNL r/x/y/z] hier eingegeben [!UICONTROL URL Prefix] werden.
         * Wenn kein Wert [!UICONTROL URL Prefix] benötigt wird, lassen Sie diesen Wert leer.
      * **[!UICONTROL Authentication - SSH Key]**
         * Geben Sie den vollständigen `SSH PRIVATE` Schlüsselwert in dieses Feld ein, einschließlich Kopf- und Fußzeilen sowie Zeilenumbrüchen, um eine genaue Verschlüsselung/einen wichtigen Speicherplatz sicherzustellen.

### Nicht genügend Zeit für Ausgehende Generierung

Der ausgehende Prozess läuft zweimal täglich und mehrere Prozesse (Ausgehende, Veröffentlichung, an externe Standorte weiterleiten usw.) muss ausgeführt werden, bevor eine Datei an das endgültige Ziel gesendet wird. Eine gute Faustregel besteht darin, dass ein Ziel mindestens 24 Stunden, bevor Sie Daten an einen externen Ort senden können, vollständig konfiguriert werden sollte.

### Dateiaufteilung zu groß

Wenn Sie ausgehende Dateien zu Zielen auswählen, können Sie größere ausgehende Dateien in Dateiabschnitten aufteilen. Stellen Sie sicher, dass die einzelnen Dateiblöcke 10 GB nicht überschreiten. Siehe auch [Ausgehende Datendateiname: Syntax und Beispiele](https://docs.adobe.com/help/en/audience-manager/user-guide/implemenation-integration-guides/receiving-audience-data/batch-outbound-data-transfers/outbound-file-name-contents.html).


## So richten Sie Ihre Ziele so ein, dass Sie Erlebnis-Ids, Kunden-IDs oder Audience Manager-IDs in ausgehende Datendateien exportieren {#set-up-destinations-export}

Auf dieser Seite erfahren Sie, wie Sie Ziele einrichten, die den aus dem gewünschten ID-Typ stammenden Datensatz exportieren [!UICONTROL Outbound Data Files].

<!-- set-up-destinations-mcid-aamid.xml -->

Ziele ermöglichen es unseren Kunden, ihre Daten über beliebige digitale Kanäle hinweg zu aktivieren. Sie können beispielsweise Zielgruppendaten in andere [!DNL Adobe Experience Cloud] Lösungen ([!DNL Target], [!DNL Campaign]usw.) exportieren. Oder sie könnten Daten an [!UICONTROL DSP]s, [!UICONTROL SSP]s oder beliebige Plattformen senden, die in Audience Manager integriert sind. Wir behalten eine Liste von Partnern bei, mit denen wir arbeiten auf unserer [Integrations-Wiki-Seite](https://wiki.corp.adobe.com/display/MCPI).

>[!NOTE]
>
>Eine detaillierte Anleitung zum Erstellen von Zielen in der Admin-Benutzeroberfläche finden Sie [im Artikel "Unternehmensziele](companies/admin-manage-company-destinations.md#create-edit-company-destinations) erstellen oder bearbeiten" .

Ihre Kunden möchten je nach Ziel verschiedene ID-Typen exportieren. Im folgenden Konfigurationsdiagramm werden die Optionen angezeigt, die Sie zum Exportieren von Profilinformationen in Bezug auf verschiedene ID-Typen auswählen sollten. Wir empfehlen Ihnen auch, in Audience Manager auf den [Index von IDs zu verweisen](https://marketing.adobe.com/resources/help/en_US/aam/ids-in-aam.html). Es gibt drei wichtige Einstellungen, die beachtet werden sollten: [!UICONTROL User ID Key], a [!UICONTROL Data Source Type] und. [!UICONTROL Format] Wir werden alle weiter unten detailliert.

* [!UICONTROL User ID Key]. [!UICONTROL Admin UI]**[!UICONTROL Companies]** Navigieren Sie zu. Suchen Sie nach dem Unternehmen Ihres Kunden und klicken Sie darauf. Suchen Sie nach der **[!UICONTROL Destinations]** Registerkarte und drücken **[!UICONTROL Add Destination]** Sie. Wählen Sie im **[!UICONTROL Add Destination]** Arbeitsablauf die [!UICONTROL User ID Key]. Die [!UICONTROL User ID Key] eingehende ID filtert die eingehenden IDs aus der Zieldatenquelle und gestattet nur die Weitergabe der IDs.

   ![](assets/user_id_key.PNG)

* [!UICONTROL Data Source Type]. Wählen Sie dies beim Erstellen eines Ziels in der Benutzeroberfläche von Audience Manager aus. Wählen Sie zuerst den [!UICONTROL Inbound]gewünschten ID-Typ aus und wählen Sie ihn aus. Die Optionen sind:

   ![](assets/data_source_settings.PNG)

* [!UICONTROL Format]. Diese Option bestimmt das Dateiformat, das Sie exportieren werden. Wählen Sie im **[!UICONTROL Add Destination]** Arbeitsablauf das **[!UICONTROL Batch Data]** Format aus.

Um ein Format zu prüfen, suchen **[!UICONTROL Admin UI > Formats]** Sie das [!UICONTROL Data Row] Element und suchen Sie es. Dieses Element enthält das Makro-Format &lt; MCID &gt; im unten stehenden Beispiel.

![](assets/data_row.PNG)

<table id="table_DAEE5BC75DCB4FC690C4BAE41F627DEC"> 
 <thead> 
  <tr> 
   <th colname="col01" class="entry"> Konfiguration Nein. </th> 
   <th colname="col1" class="entry"> <p>Benutzerschlüssel </p> </th> 
   <th colname="col2" class="entry"> <p>Datenquellen-Typ </p> </th> 
   <th colname="col3" class="entry"> <p>Format </p> </th> 
   <th colname="col4" class="entry"> <p>Exportierter ID-Typ </p> </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col01"> 1 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Experience Cloud ID </p> </td> 
   <td colname="col3"> <p>&lt; DP_ UUID &gt; </p> </td> 
   <td colname="col4"> <p>Experience Cloud ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 2 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Experience Cloud ID </p> </td> 
   <td colname="col3"> <p>MCID </p> </td> 
   <td colname="col4"> <p>Audience Manager UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 3 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Experience Cloud ID </p> </td> 
   <td colname="col3"> <p>UUID </p> </td> 
   <td colname="col4"> <p>Experience Cloud ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 4 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>&lt; DP_ UUID &gt; </p> </td> 
   <td colname="col4"> <p>Audience Manager UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 5 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>MCID </p> </td> 
   <td colname="col4"> <p>Experience Cloud ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 6 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>UUID </p> </td> 
   <td colname="col4"> <p>Audience Manager UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 7 </td> 
   <td colname="col1"> <p>DPID (beliebige Datenquelle, auf die das Unternehmen Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Customer ID </p> </td> 
   <td colname="col3"> <p>&lt; DP_ UUID &gt; </p> </td> 
   <td colname="col4"> <p>Kunden-ID (DPUUID) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 8 </td> 
   <td colname="col1"> <p>DPID (beliebige Datenquelle, auf die das Unternehmen Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Customer ID </p> </td> 
   <td colname="col3"> <p>MCID </p> </td> 
   <td colname="col4"> <p>Experience Cloud ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 9 </td> 
   <td colname="col1"> <p>DPID (beliebige Datenquelle, auf die das Unternehmen Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Customer ID </p> </td> 
   <td colname="col3"> <p>UUID </p> </td> 
   <td colname="col4"> <p>Audience Manager UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 10 </td> 
   <td colname="col1"> <p>DPID (beliebige Datenquelle, auf die das Unternehmen Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>&lt; DP_ UUID &gt; </p> </td> 
   <td colname="col4"> <p>Audience Manager UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 11 </td> 
   <td colname="col1"> <p>DPID (beliebige Datenquelle, auf die das Unternehmen Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>MCID </p> </td> 
   <td colname="col4"> <p>Experience Cloud ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 12 </td> 
   <td colname="col1"> <p>DPID (beliebige Datenquelle, auf die das Unternehmen Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>UUID </p> </td> 
   <td colname="col4"> <p>Audience Manager UUID </p> </td> 
  </tr> 
 </tbody> 
</table>

## Nutzungsszenarios

Nehmen wir an, Sie verwenden Audience Manager und [!DNL Campaign]. Um die Kundendaten in zu [!DNL Campaign]übernehmen [!UICONTROL Experience Cloud IDs], möchten Sie den Export exportieren. In diesem Fall sollten Sie die Konfigurationsnummer 3 verwenden.