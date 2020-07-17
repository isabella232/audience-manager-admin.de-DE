---
description: Verwenden Sie die Seite "Server"im Audience Manager-Admin-Tool, um einen neuen FTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-description: Verwenden Sie die Seite "Server"im Audience Manager-Admin-Tool, um einen neuen FTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-title: Erstellen und Bearbeiten von FTP-Servern
title: Erstellen und Bearbeiten von FTP-Servern
uuid: 9273abb2-963d-4d83-bf5a-b3817f0b90e6
translation-type: tm+mt
source-git-commit: 78d694670e7abdc18938c5be729ad499e2647825
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 5%

---


# Erstellen und Bearbeiten von FTP-Servern {#create-or-edit-an-ftp-server}

Verwenden Sie die [!UICONTROL Servers] Seite im Audience Manager-Admin-Tool, um einen neuen FTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.

>[!NOTE]
>
>Sie müssen die [!UICONTROL DEXADMIN] Rolle haben, um neue Server zu erstellen oder vorhandene Server zu bearbeiten.

1. Um einen neuen Server zu erstellen, klicken Sie auf **[!UICONTROL Servers]** > **[!UICONTROL Create Server]**. Um einen vorhandenen Server zu bearbeiten, klicken Sie auf den gewünschten Server in der **[!UICONTROL Label]** Spalte.
1. Geben Sie die gewünschte Bezeichnung für diesen Server an.
1. Wählen Sie in der **[!UICONTROL Protocol]** Dropdown-Liste das gewünschte Protokoll aus: **FTP**.

   >[!NOTE]
   >
   >Als Best Practice empfehlen wir die Verwendung [!DNL Amazon S3] als Methode zum Abrufen von Dateien und zum Senden von Dateien an Partner. [!DNL Amazon S3] bietet eine einfache Web-Services-Oberfläche, die verwendet werden kann, um eine beliebige Menge von Daten zu speichern und abzurufen, jederzeit und überall im Web. Weitere Informationen finden Sie unter [Info zu Amazon S3](https://docs.adobe.com/content/help/en/audience-manager/user-guide/reference/amazon-s3.html) im *Audience Manager-Benutzerhandbuch*.

1. Füllen Sie die Felder aus:

   * **[!UICONTROL Type]:**Wählen Sie den gewünschten Verschlüsselungstyp aus:**[!UICONTROL SFTP]**oder **[!UICONTROL FTPs/TLS]**.
   * **[!UICONTROL Domain]:**Geben Sie die gewünschte Domäne (den Host) für diesen Server an.
   * **[!UICONTROL Port]:**Geben Sie den gewünschten Anschluss für diesen Server an. Für jeden Verschlüsselungstyp wird der Standardanschluss angezeigt. Sie können den Standardanschluss bei Bedarf ändern.
   * **[!UICONTROL Remote Path]:**Geben Sie den gewünschten Remote-Pfad für diesen Server an. Wenn Sie dieses Feld leer lassen, platziert Audience Manager die Dateien im Standardverzeichnis.
   * **[!UICONTROL .tmp File Rename on Completion]:**Aktivieren Sie diese Option, um die`.tmp`Datei nach Abschluss des Vorgangs umzubenennen.
   * **[!UICONTROL Filename Suffix]:**Geben Sie den Text an, der an die Dateien angehängt werden soll.
   * **[!UICONTROL Moved to When Finished]:**Geben Sie den Pfad zu dem Speicherort an, an den die Übertragungsdatei nach Abschluss des Vorgangs verschoben werden soll.
   * **[!UICONTROL Authentication]:**Geben Sie die gewünschte Serverauthentifizierungsmethode an:**[!UICONTROL Username/Password]**oder **[!UICONTROL SSH Key]**.

   >[!NOTE]
   >
   >Vergessen Sie nicht, Ihre Liste der zulässigen IPs [!DNL FTP] [!DNL IP] um unsere Adresse zu erweitern: **52 44 29 204**.

1. Zur **[!UICONTROL SSH Key]** Authentifizierung:
   >[!NOTE]
   >
   >Stellen Sie beim Konfigurieren der SSH-Schlüsselauthentifizierung sicher, dass Sie stets die öffentlichen und privaten Schlüssel nur im OpenSSH-Format generieren.
   1. Generieren Sie das Public / Private Key Paar von einem beliebigen [!DNL Linux] oder [!DNL Mac] Computer.
   1. Weisen Sie den **öffentlichen Schlüssel** dem Client zu, um ihn auf dem [!DNL SFTP] Server zu aktualisieren. Sie müssen den gesamten Text des öffentlichen Schlüssels auf ihrem Server einschließen, einschließlich `-----BEGIN RSA PRIVATE KEY-----` und `-----END RSA PRIVATE KEY-----` . Im Gegenzug müssen sie den Benutzernamen angeben, unter dem sie den Schlüssel installieren.
   1. Aktualisieren Sie das Feld &quot;Benutzername&quot;mit dem vom Client bereitgestellten Feld und das Schlüsselfeld mit dem **privaten Schlüssel**.
1. Klicken Sie auf **[!UICONTROL Create]** , wenn Sie einen neuen Server erstellen, oder klicken Sie auf **[!UICONTROL Update]** , wenn Sie einen vorhandenen Server bearbeiten.
