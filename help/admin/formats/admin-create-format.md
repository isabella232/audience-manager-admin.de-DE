---
description: Verwenden Sie die Seite "Formate"im Audience Manager-Admin-Tool, um ein neues Format zu erstellen oder ein vorhandenes Format zu bearbeiten.
seo-description: Verwenden Sie die Seite "Formate"im Audience Manager-Admin-Tool, um ein neues Format zu erstellen oder ein vorhandenes Format zu bearbeiten.
seo-title: Erstellen oder Bearbeiten von Formaten
title: Erstellen oder Bearbeiten von Formaten
uuid: ca1b1feb-bcd3-4a41-b1e8-80565f6c23ae
translation-type: tm+mt
source-git-commit: 71bf4cec222428686c1eab0998f66887db06da68
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 5%

---


# Erstellen oder Bearbeiten von Formaten {#create-or-edit-a-format}

Verwenden Sie die [!UICONTROL Formats] Seite im Audience Manager Admin Tool, um ein neues Format zu erstellen oder ein vorhandenes Format zu bearbeiten.

<!-- t_create_format.xml -->

>[!TIP]
>
>Bei der Auswahl eines Formats für Ihre Daten im Ausland sollten Sie möglichst ein vorhandenes Format wiederverwenden. Die Verwendung eines bereits bewährten Formats stellt sicher, dass Ihre ausgehenden Daten erfolgreich generiert werden. Um genau zu sehen, wie ein vorhandenes Format formatiert ist, klicken Sie auf die [!UICONTROL Formats] Option in der Menüleiste und suchen Sie nach dem Format nach Namen oder ID-Nummer. Falsche Formate oder Makros, die in Formaten verwendet werden, liefern eine falsch formatierte Ausgabe oder verhindern, dass Informationen vollständig ausgegeben werden.

1. Um ein neues Format zu erstellen, klicken Sie auf **[!UICONTROL Formats]** > **[!UICONTROL Add Format]**. Um ein vorhandenes Format zu bearbeiten, klicken Sie auf das gewünschte Format in der **[!UICONTROL Name]** Spalte.

   ![](assets/create_format.png)

1. Füllen Sie die Felder aus:
   * **Name:** (Erforderlich) Geben Sie einen beschreibenden Namen für das Format ein.
   * **Typ:** (Erforderlich) Wählen Sie das gewünschte Format aus:
      * **[!UICONTROL File]**: Sendet Daten über [!DNL FTP] Dateien.
      * **[!UICONTROL HTTP]**: Umfasst Daten in einem [!DNL JSON] Wrapper.

1. (Bedingt) Wenn Sie diese Option wählen, füllen Sie **[!UICONTROL File]** die Felder aus:

   >[!NOTE]
   >
   >Eine Liste der verfügbaren Makros finden Sie unter [Dateiformatmakros](../formats/file-formats.md#concept_A867101505074418A58DE325949E5089) und [HTTP-Formatmakros](../formats/web-formats.md#reference_C392124A5F3F42E49F8AADDBA601ADFE).

   * **[!UICONTROL File Name]:**Geben Sie den Dateinamen für die Datenübertragungsdatei an.
   * **Kopfzeile:** Geben Sie den Text ein, der in der ersten Zeile der Datenübertragungsdatei angezeigt wird.
   * **[!UICONTROL Data Row]:**Geben Sie den Text an, der in jeder ausgehenden Zeile der Datei angezeigt wird.
   * **[!UICONTROL Maximum File Size (In MB)]:**Geben Sie die maximale Dateigröße für Datenübertragungsdateien an. Komprimierte Dateien müssen kleiner als 100 MB sein. Die Größe der unkomprimierten Datei ist nicht begrenzt.
   * **[!UICONTROL Compression]:**Wählen Sie den gewünschten Komprimierungstyp aus: gz oder zip für Ihre Datendateien. Zum Versand[!UICONTROL AWS S3]müssen Sie .gz- oder unkomprimierte Dateien verwenden.
   * **[!UICONTROL .info Receipt]:**Gibt an, dass eine ([!DNL .info]) Übertragungssteuerungsdatei generiert wird. Die[!DNL .info]Datei enthält Metadateninformationen zu Dateiübertragungen, damit die Partner überprüfen können, ob die Dateiübertragungen von Audience Manager korrekt verarbeitet wurden. Weitere Informationen finden Sie unter[Transfer-Control-Dateien für Protokolldateitransfers](https://marketing.adobe.com/resources/help/en_US/aam/c_s2s_add_transfer_control_files.html).
   * **[!UICONTROL MD5 Checksum Receipt]:**Gibt an, dass ein[!DNL MD5]Prüfsummenbeleg generiert wird. Der[!DNL MD5]Prüfsummenbeleg, damit die Partner überprüfen können, ob der Audience Manager die gesamte Übertragung ordnungsgemäß durchgeführt hat.

1. (Bedingt) Wenn Sie diese Option wählen, füllen Sie **[!UICONTROL HTTP]** die Felder aus:

   * **[!UICONTROL Method]:**Wählen Sie die[!DNL API]Methode, die Sie für den Transfervorgang verwenden möchten:
      * **[!UICONTROL POST]:**Wählen Sie bei Auswahl[!DNL POST]den Inhaltstyp ([!DNL XML]oder[!DNL JSON]) und geben Sie dann den Anforderungstext an.
      * **[!UICONTROL GET]:**Geben Sie bei Auswahl[!DNL GET]die Parameter für die Abfrage an.

1. Klicken Sie auf **[!UICONTROL Create]** , wenn Sie ein neues Format erstellen, oder klicken Sie auf **[!UICONTROL Save Updates]** , wenn Sie ein vorhandenes Format bearbeiten.

## Löschen eines Formats {#delete-format}

1. Klicken **[!UICONTROL Formats]**.
2. Klicken Sie ![](assets/icon_delete.png) in die **[!UICONTROL Actions]** Spalte des gewünschten Formats.
3. Klicken Sie auf **[!UICONTROL OK]**, um den Löschvorgang zu bestätigen.
