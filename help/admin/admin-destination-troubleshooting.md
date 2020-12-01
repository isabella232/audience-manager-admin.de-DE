---
description: Informationen, die Sie bei der Einrichtung von Zielen in Audience Manager unterstützen und häufig auftretende Probleme vermeiden.
seo-description: Informationen, die Sie bei der Einrichtung von Zielen in Audience Manager unterstützen und häufig auftretende Probleme vermeiden.
seo-title: Fehlerbehebung bei der Zieleinrichtung
title: Fehlerbehebung bei der Zieleinrichtung
uuid: 04080fb9-6c7b-4de7-960e-54482be2de83
translation-type: tm+mt
source-git-commit: 118e8fa3f35bc77846c6518268448d57d779a2ee
workflow-type: tm+mt
source-wordcount: '1331'
ht-degree: 4%

---


# Fehlerbehebung bei der Zieleinrichtung {#destination-setup-troubleshooting}

Informationen, die Sie bei der Einrichtung von Zielen in Audience Manager unterstützen und häufig auftretende Probleme vermeiden.

## Ich habe ein Ziel eingerichtet, sehe aber keine Dateien. Wo sind sie? {#destination-no-files}

<!-- c_dest_tshooting.xml -->

Häufige Probleme bei der Konfiguration von Zielen sind unter anderem folgende:

### Fehlkonfiguriertes Ziel

* **Falscher  [!UICONTROL UserID] Schlüssel:** Der  [!UICONTROL UserID] Schlüssel ist der  [!UICONTROL MasterDPID] dieses Ziels und bildet die Grundlage für die ID-Werte, die überschrieben werden. Auch wenn eine [!UICONTROL UserID]-Taste über die Dropdown-Liste ausgewählt werden kann, bedeutet dies nicht unbedingt, dass diesem Wert IDs/Eigenschaften/Segmente zugeordnet sind. Wenn der [!UICONTROL Outbound]-Prozess (der nach dem Erstellen von Zielen ausgeführt wird) keine Benutzer findet, die diesem [!UICONTROL UserID]-Schlüssel zugeordnet sind, werden keine Daten überschrieben.
* **Keine Auswahl in Datenquellen in der Datei:** Bei Auswahl eines anderen Zieltyps als  [!UICONTROL S2S]wird am unteren Rand des Bildschirms ein Abschnitt mit der Bezeichnung angezeigt  [!UICONTROL Configure Data Sources]. Wenn dieser Abschnitt zum ersten Mal angezeigt wird, werden keine Werte ausgewählt. Wenn Sie vergessen haben, auf das Kontrollkästchen [!UICONTROL All First Party] zu klicken oder Datenquellen einzeln aus dem Fenster [!UICONTROL Available Data Sources] auszuwählen, werden keine Daten mehr ausgegeben.

### Nicht konfiguriertes Format

Bei der Auswahl eines Formats für Ihre Daten im Ausland sollten Sie möglichst ein vorhandenes Format wiederverwenden. Die Verwendung eines bereits bewährten Formats stellt sicher, dass Ihre ausgehenden Daten erfolgreich generiert werden. Um genau zu sehen, wie ein vorhandenes Format formatiert ist, klicken Sie in der Menüleiste auf die Option [!UICONTROL Formats] und suchen Sie nach Ihrem Format entweder nach Namen oder nach ID-Nummer. Falsche Formate oder Makros, die in Formaten verwendet werden, liefern eine falsch formatierte Ausgabe oder verhindern, dass Informationen vollständig ausgegeben werden.

Weitere Informationen zum Einrichten von Formaten und zum Verwenden von Makros finden Sie unter [Dateiformatmakros](formats/file-formats.md#) und [HTTP-Formatmakros](formats/web-formats.md).

### Nicht konfigurierter Server

* **[!DNL FTP]**
   * **[!UICONTROL Domain]**
      * Geben Sie keine Präfixe für Hostnamen ein. Wenn Sie ein Konto [!DNL ftp://hello.com] haben, geben Sie einfach [!DNL hello.com] in dieses Feld ein.
   * **[!UICONTROL Port/Type Combination]**
      * Bei einer [!DNL FTP]-Übertragung ist der bevorzugte Transfertyp [!DNL SFTP].
      * Bei Auswahl des Typs [!DNL SFTP] ist der Anschluss fast immer 22.
      * Bei Auswahl des Typs [!DNL FTPs/TLS] ist der Anschluss fast immer 21.
      * Der Typ [!DNL FTPs/TLS] ist nicht identisch mit einer regulären [!DNL FTP]-Übertragung. Wir unterstützen keine regelmäßigen (ungesicherten) [!DNL FTP] Übertragungen.
   * **[!UICONTROL Remote Path]**
      * Bei der Auswahl eines Remote-Unterpfads sollte dieser ohne Schrägstrich eingegeben werden.
      * Wenn Ihre übertragene Datei im Unterordner [!DNL (root)/inbound] abgelegt werden soll, fügen Sie für den Remote-Pfad einfach [!DNL inbound] und nicht [!DNL /inbound] hinzu.
      * Wenn Sie Ihre Dateien mehrere Ordner unter den Pfad senden, geben Sie Schrägstriche zwischen den einzelnen Ordnern ein. Wenn Sie den Speicherort von [!DNL /inbound/subdirectory1/subdirectory2] erhalten, sollten Sie [!DNL inbound/subdirectory1/subdirectory2] in dieses Feld eingeben.
      * Wenn die Datei in dem Ordner abgelegt werden soll, der automatisch vom externen Server an den Server weitergeleitet wird, können Sie diesen Leerraum leer lassen. Geben Sie keinen Punkt ein (. ), Schrägstrich ( / ) oder alles andere.

* **[!DNL S3]**
   * [!DNL S3] ist das bevorzugte Transfer-Protokoll (over  [!DNL FTP] oder  [!DNL HTTP]).
      * **[!UICONTROL Bucket]**
         * Der Behältername sollte ohne Schrägstriche, Präfixe, Suffixe usw. aufgeführt werden. Wenn Sie die Adresse [!DNL s3://your-bucket] erhalten, sollten Sie [!DNL your-bucket] einfach diesem Feld hinzufügen.
      * **[!UICONTROL Directory]**
         * Lassen Sie dieses Feld leer, es sei denn, Sie erhalten einen Unterordner, in dem die Daten abgelegt werden sollen. Wenn Sie die Adresse [!DNL s3://your-bucket/your-subdirectory] erhalten, geben Sie [!DNL your-bucket] in das Feld [!UICONTROL Bucket] ein und [!DNL your-subdirectory] sollte in das Feld [!UICONTROL Directory] eingefügt werden. Fügen Sie keine vorherigen Schrägstriche hinzu.
         * Wenn Sie mehrere Ordner entlang des Pfades reisen müssen, sollten Sie nur Schrägstriche als Trennzeichen verwenden. An einem Ort von [!DNL s3://your-bucket/your-subdirectory1/your-subdirectory2] würde [!DNL your-bucket] im Feld [!UICONTROL Bucket] und [!DNL your-subdirectory1/your-subdirectory2] in das Feld [!UICONTROL Directory] eingegeben.
      * **[!UICONTROL Access / Secret Keys]**
         * Wenn [!DNL TechOps] einen Bucket erstellt und einem Berater Zugriff-/geheime Schlüssel zur Verfügung stellt, sind diese Anmeldeinformationen in der Regel `READ-ONLY`, die an den Client übergeben werden sollen. Diese Anmeldeinformationen sollten nicht in die Felder [!UICONTROL Access / Secret Key] eingegeben werden, da dies dazu führt, dass die Übertragung fehlschlägt (da diese Anmeldeinformationen schreibgeschützt und nicht schreibbar sind). Wenn [!DNL TechOps] einen Behälter erstellt und Anmeldeinformationen bereitstellt, sollte der Berater auch ein Schlüsselpaar für die Adobe anfordern - NICHT DEM CLIENT ZUZUGEBEN -, das das Schreiben von Dateien in diesen Behälter ermöglicht. Dieser Schlüssel sollte in diese Felder eingefügt werden.

* **[!DNL HTTP]**
   * **[!UICONTROL Domain]**
      * Geben Sie Präfixinformationen für [!DNL HTTP]-Einträge ein. Wenn Sie ein Konto [!DNL https://superduper.com] haben, geben Sie [!DNL https://superduper.com] in dieses Feld ein.
      * **[!UICONTROL URL Prefix]**
         * Wenn Sie ein [!DNL URL]-Präfix hinzufügen, lassen Sie den vorherigen Schrägstrich deaktiviert. Bei einer Adresse von [!DNL https://hello.com/r/x/y/z] sollte [!DNL https://hello.com] in das Feld [!UICONTROL Domain] eingegeben und [!DNL r/x/y/z] hier in das Feld [!UICONTROL URL Prefix] eingegeben werden.
         * Wenn kein [!UICONTROL URL Prefix] erforderlich ist, lassen Sie diesen Wert leer.
      * **[!UICONTROL Authentication - SSH Key]**
         * Geben Sie in dieses Feld den vollständigen `SSH PRIVATE`-Schlüsselwert ein, einschließlich Kopf- und Fußzeilen sowie Zeilenumbrüchen, um eine exakte Verschlüsselung/Key-Datenspeicherung sicherzustellen.

### Nicht genügend Zeit für die Generierung nach dem Auslaufen

Der Prozess wird zweimal täglich ausgeführt, und es werden mehrere Prozesse ausgeführt (Auslaufen, Veröffentlichen, An externe Standorte verschieben usw.) muss ausgeführt werden, bevor eine Datei an ihr endgültiges Ziel gesendet wird. Eine gute Faustregel ist, dass ein Ziel mindestens 24 Stunden vollständig konfiguriert werden sollte, bevor Sie erwarten können, dass Daten an einen externen Speicherort gesendet werden.

### Dateiaufteilungsgrößen zu groß

Wenn Sie Dateien an Zielorte auslagern, können Sie größere ausgehende Dateien in Dateiblöcke aufteilen. Achten Sie darauf, dass die einzelnen Dateiabschnitte 10 GB nicht überschreiten. Siehe auch [Name der ausgehenden Datendatei: Syntax und Beispiele](https://docs.adobe.com/help/en/audience-manager/user-guide/implemenation-integration-guides/receiving-audience-data/batch-outbound-data-transfers/outbound-file-name-contents.html).


## Einrichten Ihrer Ziele zum Exportieren von Experience Cloud-IDs, Kunden-IDs oder Audience Manager-IDs in ausgehenden Datendateien {#set-up-destinations-export}

Diese Seite zeigt Ihnen, wie Sie Ziele einrichten, um Daten zu exportieren, die vom ID-Typ, den Sie unter [!UICONTROL Outbound Data Files] eingeben möchten, abgegrenzt sind.

<!-- set-up-destinations-mcid-aamid.xml -->

Ziele ermöglichen es unseren Kunden, ihre Daten über eine beliebige Anzahl digitaler Kanal zu aktivieren. Sie können beispielsweise Daten zur Audience in andere [!DNL Adobe Experience Cloud]-Lösungen ([!DNL Target], [!DNL Campaign] usw.) exportieren. Oder sie können Daten an [!UICONTROL DSP]s, [!UICONTROL SSP]s oder eine beliebige Plattform senden, die in Audience Manager integriert ist. Wir führen eine Liste von Partnern, mit denen wir arbeiten, auf unserer [Integrations-Wiki-Seite](https://wiki.corp.adobe.com/display/MCPI).

>[!NOTE]
>
>Eine ausführliche Anleitung zum Erstellen von Zielen in der Admin-Benutzeroberfläche finden Sie im Artikel [Ziele für Firmen erstellen oder bearbeiten](companies/admin-manage-company-destinations.md#create-edit-company-destinations).

Ihre Kunden möchten je nach Ziel unterschiedliche ID-Typen exportieren. Das folgende Konfigurationstabelle zeigt die Optionen, die Sie auswählen sollten, um Profil-Informationen zu verschiedenen ID-Typen zu exportieren. Es wird empfohlen, auch auf den [ID-Index in Audience Manager](https://marketing.adobe.com/resources/help/en_US/aam/ids-in-aam.html) zu verweisen. Es sind drei wichtige Einstellungen zu beachten: die [!UICONTROL User ID Key], die [!UICONTROL Data Source Type] und die [!UICONTROL Format]. Wir führen alle unten auf.

* [!UICONTROL User ID Key]. Wechseln Sie in [!UICONTROL Admin UI] zu **[!UICONTROL Companies]**. Suchen Sie nach der Firma Ihres Kunden und klicken Sie darauf. Suchen Sie nach der Registerkarte **[!UICONTROL Destinations]** und drücken Sie **[!UICONTROL Add Destination]**. Wählen Sie im Arbeitsablauf **[!UICONTROL Add Destination]** die Option [!UICONTROL User ID Key]. Die [!UICONTROL User ID Key] filtert die eingehenden IDs aus der Zielgruppe-Datenquelle und lässt nur das Übergeben der IDs zu.

   ![](assets/user_id_key.PNG)

* [!UICONTROL Data Source Type]. Wählen Sie diese Option, wenn Sie ein Ziel in der Benutzeroberfläche des Audience Managers erstellen. Wählen Sie zunächst [!UICONTROL Inbound] und dann den gewünschten ID-Typ aus. Die Optionen sind:

   ![](assets/data_source_settings.PNG)

* [!UICONTROL Format]. Diese Option legt das Dateiformat fest, das exportiert werden soll. Wählen Sie im Arbeitsablauf **[!UICONTROL Add Destination]** unter **[!UICONTROL Batch Data]** das Format aus.

Um ein Format zu überprüfen, gehen Sie zu **[!UICONTROL Admin UI > Formats]** und suchen Sie nach dem [!UICONTROL Data Row]-Element. Dieses Element enthält ein Makro des Dateiformats, &lt;MCID> im Beispiel unten.

![](assets/data_row.PNG)

<table id="table_DAEE5BC75DCB4FC690C4BAE41F627DEC"> 
 <thead> 
  <tr> 
   <th colname="col01" class="entry"> Konfigurationsnummer </th> 
   <th colname="col1" class="entry"> <p>Benutzerschlüssel </p> </th> 
   <th colname="col2" class="entry"> <p>Datenquelle-Typ </p> </th> 
   <th colname="col3" class="entry"> <p>Format </p> </th> 
   <th colname="col4" class="entry"> <p>Exportierter ID-Typ </p> </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col01"> 1 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Experience Cloud ID </p> </td> 
   <td colname="col3"> <p>&lt;dp_uuid&gt; </p> </td> 
   <td colname="col4"> <p>Experience Cloud-ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 2 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Experience Cloud-ID </p> </td> 
   <td colname="col3"> <p>MCID </p> </td> 
   <td colname="col4"> <p>Audience Manager-UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 3 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Experience Cloud-ID </p> </td> 
   <td colname="col3"> <p>UUID </p> </td> 
   <td colname="col4"> <p>Experience Cloud-ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 4 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>&lt;dp_uuid&gt; </p> </td> 
   <td colname="col4"> <p>Audience Manager-UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 5 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>MCID </p> </td> 
   <td colname="col4"> <p>Experience Cloud-ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 6 </td> 
   <td colname="col1"> <p>Adobe Audience Manager (0) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>UUID </p> </td> 
   <td colname="col4"> <p>Audience Manager-UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 7 </td> 
   <td colname="col1"> <p>DPID (Jede Datenquelle, auf die die Firma Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Kunden-ID </p> </td> 
   <td colname="col3"> <p>&lt;dp_uuid&gt; </p> </td> 
   <td colname="col4"> <p>Kunden-ID (DPUUID) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 8 </td> 
   <td colname="col1"> <p>DPID (Jede Datenquelle, auf die die Firma Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Kunden-ID </p> </td> 
   <td colname="col3"> <p>MCID </p> </td> 
   <td colname="col4"> <p>Experience Cloud-ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 9 </td> 
   <td colname="col1"> <p>DPID (Jede Datenquelle, auf die die Firma Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Kunden-ID </p> </td> 
   <td colname="col3"> <p>UUID </p> </td> 
   <td colname="col4"> <p>Audience Manager-UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 10 </td> 
   <td colname="col1"> <p>DPID (Jede Datenquelle, auf die die Firma Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>&lt;dp_uuid&gt; </p> </td> 
   <td colname="col4"> <p>Audience Manager-UUID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 11 </td> 
   <td colname="col1"> <p>DPID (Jede Datenquelle, auf die die Firma Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>MCID </p> </td> 
   <td colname="col4"> <p>Experience Cloud-ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> 12 </td> 
   <td colname="col1"> <p>DPID (Jede Datenquelle, auf die die Firma Zugriff hat) </p> </td> 
   <td colname="col2"> <p>Audience Manager-ID </p> </td> 
   <td colname="col3"> <p>UUID </p> </td> 
   <td colname="col4"> <p>Audience Manager-UUID </p> </td> 
  </tr> 
 </tbody> 
</table>

## Nutzungsszenarios

Nehmen wir an, Sie verwenden Audience Manager und [!DNL Campaign]. Damit die Kundendaten in [!DNL Campaign] verarbeitet werden können, müssen Sie [!UICONTROL Experience Cloud IDs] exportieren. In diesem Fall sollten Sie die Konfigurationsnummer 3 verwenden.