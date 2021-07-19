---
description: Verwenden Sie die Seite "Server"im Audience Manager Admin-Tool, um einen neuen FTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-description: Verwenden Sie die Seite "Server"im Audience Manager Admin-Tool, um einen neuen FTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-title: Erstellen und Bearbeiten von FTP-Servern
title: Erstellen und Bearbeiten von FTP-Servern
uuid: 9273abb2-963d-4d83-bf5a-b3817f0b90e6
exl-id: 9eae4ecf-ccde-483a-ae53-1cbac033d8d6
source-git-commit: f5d74995f0664cf63e68b46f1f3c608f34df0e80
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 5%

---

# Erstellen und Bearbeiten von FTP-Servern {#create-or-edit-an-ftp-server}

Verwenden Sie die Seite [!UICONTROL Servers] im Audience Manager Admin-Tool, um einen neuen FTP-Server zu erstellen oder einen bestehenden Server zu bearbeiten.

>[!NOTE]
>
>Sie müssen über die Rolle [!UICONTROL DEXADMIN] verfügen, um neue Server zu erstellen oder vorhandene Server zu bearbeiten.

1. Um einen neuen Server zu erstellen, klicken Sie auf **[!UICONTROL Servers]** > **[!UICONTROL Create Server]**. Um einen vorhandenen Server zu bearbeiten, klicken Sie in der Spalte **[!UICONTROL Label]** auf den gewünschten Server.
1. Geben Sie die gewünschte Bezeichnung für diesen Server an.
1. Wählen Sie aus der Dropdownliste **[!UICONTROL Protocol]** das gewünschte Protokoll aus: **FTP**.

   >[!NOTE]
   >
   >Als Best Practice empfehlen wir die Verwendung von [!DNL Amazon S3] als Methode zum Abrufen von Dateien von und zum Bereitstellen von Dateien an Partner. [!DNL Amazon S3] bietet eine einfache Web-Services-Oberfläche, die verwendet werden kann, um eine beliebige Menge von Daten jederzeit von überall aus im Internet zu speichern und abzurufen. Weitere Informationen finden Sie unter [Über Amazon S3](https://docs.adobe.com/content/help/en/audience-manager/user-guide/reference/amazon-s3.html) im *Audience Manager-Benutzerhandbuch*.

1. Füllen Sie die Felder aus:

   * **[!UICONTROL Type]:**  Wählen Sie den gewünschten Verschlüsselungstyp aus:  **[!UICONTROL SFTP]** oder  **[!UICONTROL FTPs/TLS]**.
   * **[!UICONTROL Domain]:** Geben Sie die gewünschte Domäne (den Host) für diesen Server an.
   * **[!UICONTROL Port]:** Geben Sie den gewünschten Anschluss für diesen Server an. Für jeden Verschlüsselungstyp wird der Standardanschluss angezeigt. Sie können bei Bedarf den Standardanschluss ändern.
   * **[!UICONTROL Remote Path]:** Geben Sie den gewünschten Remote-Pfad für diesen Server an. Wenn Sie dieses Feld leer lassen, platziert Audience Manager die Dateien im Standardverzeichnis.
   * **[!UICONTROL .tmp File Rename on Completion]:** Aktivieren Sie diese Option, um die  `.tmp` Datei nach Abschluss umzubenennen.
   * **[!UICONTROL Filename Suffix]:** Geben Sie den Text an, der an die Dateiübertragung angehängt werden soll.
   * **[!UICONTROL Moved to When Finished]:** Geben Sie den Pfad zu dem Speicherort an, an den die Übertragungsdatei nach Abschluss verschoben werden soll.
   * **[!UICONTROL Authentication]:**  Geben Sie die gewünschte Server-Authentifizierungsmethode an:  **[!UICONTROL Username/Password]** oder  **[!UICONTROL SSH Key]**.

   >[!NOTE]
   >
   >Denken Sie daran, Ihre Ausgangs-IPs [!DNL FTP] [!DNL IP] Ihrer Liste der zulässigen IPs hinzuzufügen: **52.44.29.204**.

1. Für **[!UICONTROL SSH Key]**-Authentifizierung:
   >[!NOTE]
   >
   >Stellen Sie beim Konfigurieren der SSH-Schlüsselauthentifizierung sicher, dass Sie immer die öffentlichen und privaten Schlüssel nur im OpenSSH-Format generieren.
   1. Generieren Sie das Paar aus öffentlichem/privatem Schlüssel von einem beliebigen [!DNL Linux]- oder [!DNL Mac]-Computer aus.
   1. Geben Sie den **öffentlichen Schlüssel** dem Client zur Aktualisierung auf seinem [!DNL SFTP]-Server. Sie müssen den gesamten Text aus dem öffentlichen Schlüssel auf ihrem Server enthalten, einschließlich `-----BEGIN RSA PRIVATE KEY-----` und `-----END RSA PRIVATE KEY-----` . Im Gegenzug müssen sie den Benutzernamen angeben, unter dem sie den Schlüssel installieren.
   1. Aktualisieren Sie das Feld Benutzername mit dem vom Client bereitgestellten Feld und das Schlüsselfeld mit dem privaten Schlüssel **a1/>.**
1. Klicken Sie auf **[!UICONTROL Create]**, wenn Sie einen neuen Server erstellen, oder auf **[!UICONTROL Update]** , wenn Sie einen vorhandenen Server bearbeiten.
