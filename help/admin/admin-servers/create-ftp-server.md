---
description: Verwenden Sie die Seite Server im Audience Manager-Verwaltungswerkzeug, um einen neuen FTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-description: Verwenden Sie die Seite Server im Audience Manager-Verwaltungswerkzeug, um einen neuen FTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-title: FTP-Server erstellen oder bearbeiten
title: FTP-Server erstellen oder bearbeiten
uuid: 9273 abb 2-963 d -4 d 83-bf 5 a-b 3817 f 0 b 90 e 6
translation-type: tm+mt
source-git-commit: 57d7a92265e565b6c411e4cfa5c579e40eb837b3

---


# FTP-Server erstellen oder bearbeiten {#create-or-edit-an-ftp-server}

Verwenden Sie die [!UICONTROL Servers] Seite im Audience Manager-Verwaltungswerkzeug, um einen neuen FTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.

>[!NOTE]
>
>Sie müssen über die [!UICONTROL DEXADMIN] Rolle verfügen, um neue Server zu erstellen oder bestehende Server zu bearbeiten.

1. Klicken Sie **[!UICONTROL Servers]** auf &gt; **[!UICONTROL Create Server]**, um einen neuen Server zu erstellen. To edit an existing server, click the desired server in the **[!UICONTROL Label]** column.
1. Geben Sie die gewünschte Beschriftung für diesen Server an.
1. Wählen Sie aus der **[!UICONTROL Protocol]** Dropdownliste das gewünschte Protokoll aus: **FTP**.

   >[!NOTE]
   >
   >Wir empfehlen, als [!DNL Amazon S3] Methode zum Abrufen von Dateien und zur Auslieferung von Dateien an Partner zu empfehlen. [!DNL Amazon S3] bietet eine einfache Benutzeroberfläche für Webdienste, die verwendet werden kann, um beliebige Datenmengen jederzeit und jederzeit im Internet zu speichern und abzurufen. Weitere Informationen finden Sie unter [Info zu Amazon S 3](https://docs.adobe.com/content/help/en/audience-manager/user-guide/reference/amazon-s3.html) im *Audience Manager-Benutzerhandbuch*.

1. Füllen Sie die Felder aus:

   * **[!UICONTROL Type]:** Wählen Sie den gewünschten Verschlüsselungstyp aus: **[!UICONTROL SFTP]** oder **[!UICONTROL FTPs/TLS]**.
   * **[!UICONTROL Domain]:** Geben Sie die gewünschte Domäne (Host) für diesen Server an.
   * **[!UICONTROL Port]:** Geben Sie den gewünschten Anschluss für diesen Server an. Der Standardanschluss wird für jeden Verschlüsselungstyp angezeigt. Sie können bei Bedarf den Standardanschluss ändern.
   * **[!UICONTROL Remote Path]:** Geben Sie den gewünschten Remote-Pfad für diesen Server an. Wenn Sie dieses Feld leer lassen, legt Audience Manager die Dateien im Standardordner ab.
   * **[!UICONTROL .tmp File Rename on Completion]:** Aktivieren Sie diese Option, um die `.tmp` Datei beim Abschluss umzubenennen.
   * **[!UICONTROL Filename Suffix]:** Geben Sie den Text an, der an die Übertragung der Dateien angehängt werden soll.
   * **[!UICONTROL Moved to When Finished]:** Geben Sie den Pfad an der Stelle an, an der die Übertragungsdatei nach Abschluss verschoben werden soll.
   * **[!UICONTROL Authentication]:** Geben Sie die gewünschte Serverauthentifizierungsmethode an: **[!UICONTROL Username/Password]** oder **[!UICONTROL SSH Key]**.
   >[!NOTE]
   >
   >Denken Sie daran, unser Geschäft zu Whitelist [!DNL FTP][!DNL IP]zu machen: **52.44.29.204**.

1. Zur **[!UICONTROL SSH Key]** Authentifizierung:
   1. Generieren Sie das öffentliche/private Schlüsselpaar von einem beliebigen [!DNL Linux] oder [!DNL Mac] einem Computer.
   1. Geben Sie dem Kunden den **öffentlichen Schlüssel** zur Aktualisierung auf seinem [!DNL SFTP] Server. Sie müssen den gesamten Text aus dem öffentlichen Schlüssel auf ihrem Server einschließlich `-----BEGIN RSA PRIVATE KEY-----` und `-----END RSA PRIVATE KEY-----` . Im Gegenzug müssen sie den Benutzernamen angeben, unter dem sie den Schlüssel installieren.
   1. Aktualisieren Sie das Feld Benutzername mit dem vom Client bereitgestellten Feld und dem Schlüsselfeld mit **dem privaten Schlüssel**.
1. Klicken **[!UICONTROL Create]** Sie auf, wenn Sie einen neuen Server erstellen, oder klicken **[!UICONTROL Update]** Sie auf, wenn Sie einen vorhandenen Server bearbeiten.
