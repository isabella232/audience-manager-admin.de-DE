---
description: Verwenden Sie die Seite "Server"im Audience Manager-Admin-Tool, um einen neuen HTTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-description: Verwenden Sie die Seite "Server"im Audience Manager-Admin-Tool, um einen neuen HTTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-title: Erstellen und Bearbeiten von HTTP-Servern
title: Erstellen und Bearbeiten von HTTP-Servern
uuid: 1ef0e751-e239-4dc6-a4f6-73cc05686807
translation-type: tm+mt
source-git-commit: 57d7a92265e565b6c411e4cfa5c579e40eb837b3
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 7%

---


# Erstellen und Bearbeiten von HTTP-Servern {#create-or-edit-an-http-server}

Verwenden Sie die [!UICONTROL Servers] Seite im Audience Manager-Admin-Tool, um einen neuen HTTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.

>[!NOTE]
>
>Sie müssen die [!UICONTROL DEXADMIN] Rolle haben, um neue Server zu erstellen oder vorhandene Server zu bearbeiten.

1. Um einen neuen Server zu erstellen, gehen Sie zu **[!UICONTROL Servers]** > **[!UICONTROL Create Server]**. Um einen vorhandenen Server zu bearbeiten, klicken Sie auf den gewünschten Server in der **[!UICONTROL Label]** Spalte.
1. Geben Sie die gewünschte Bezeichnung für diesen Server an.
1. Wählen Sie in der **[!UICONTROL Protocol]** Dropdown-Liste das gewünschte Protokoll aus: [!DNL HTTP].
1. Füllen Sie die Felder aus:

   * **[!UICONTROL Domain]:**Geben Sie die gewünschte Domäne (den Host) für diesen Server an.
   * **[!UICONTROL Port]:**Geben Sie den gewünschten Anschluss für diesen Server an. Für jeden Verschlüsselungstyp wird der Standardanschluss angezeigt. Sie können den Standardanschluss bei Bedarf ändern
   * **[!UICONTROL Maximum Users Per Request]:**Geben Sie die maximale Anzahl von Benutzern pro Anforderung an, die für diesen Server zulässig ist.
   * **[!UICONTROL URL Prefix]:**Geben Sie das für diesen Server zu verwendende[!DNL URL]Präfix an.
   * **[!UICONTROL Authentication URL]:**Geben Sie die[!UICONTROL Authentication URL]für diesen`HTTP`Server an.
   * **[!UICONTROL Authentication]:**Geben Sie die gewünschte Authentifizierungsmethode an:**[!UICONTROL None]**,**[!UICONTROL Username/Password]**oder **[!UICONTROL SSH Key]**.
   * **[!UICONTROL HTTP Signature Header]:**Der Name der vom Kunden bereitgestellten[!DNL HTTP]Kopfzeile, die den[!DNL HTTP]Signaturschlüssel enthält. Der Standardwert ist[!UICONTROL X-Signature]wie im folgenden Beispiel dargestellt:

      ```
      * Connected to partner.website.com (127.0.0.1) port 80 (#0)
      > POST /webpage HTTP/1.1
      > Host: partner.host.com
      > Accept: */*
      > Content-Type: application/json
      > Content-Length: 20
      > X-Signature: wxa2ByMWhhP328EvHQsVlOD5jTc=
      POST message content
      ```

   * **[!UICONTROL HTTP Signature Key]:**Der Schlüssel, der zum Unterschreiben der[!DNL HTTP]Anforderung verwendet wird, vom Kunden bereitgestellt.
   * **[!UICONTROL Show Signature Key]:**Schalten Sie ein/aus, ob die Unterschrift im Browser angezeigt werden soll.
   * **[!UICONTROL HTTP Signature Encryption Method]:**Geben Sie die Methode zum Verschlüsseln der Signatur an. Verwenden Sie diese Option,[!UICONTROL SHA1]sofern der Kunde nichts anderes vorzieht.

   >[!NOTE]
   >
   >Wenn Sie die [OAuth 2.0-Authentifizierung für Echtzeit-Datenübertragungen](https://docs.adobe.com/help/en/audience-manager/user-guide/implemenation-integration-guides/receiving-audience-data/real-time-outbound-transfers/oauth-in-outbound-transfers.html) für einen Partner aktivieren möchten, füllen Sie die folgenden Felder aus. Die kursiv *gedruckten* Felder müssen genau wie in der Tabelle ausgefüllt werden.

   | Name | Wert |
   |---|---|
   | [!UICONTROL Label] | [!UICONTROL Server with OAuth 2.0 enabled] |
   | [!UICONTROL Protocol] | [!UICONTROL HTTP] |
   | [!UICONTROL Domain] | [!UICONTROL api.partner.com] |
   | [!UICONTROL Port] | [!UICONTROL 443] |
   | [!UICONTROL Maximum Users per Request] | [!UICONTROL 10] |
   | [!UICONTROL URL Prefix] | [!UICONTROL /segments/aam] |
   | [!UICONTROL Authentication URL] | [!UICONTROL api.partner.com/oauth2/token] |
   | [!UICONTROL Authentication] | [!UICONTROL Username/Password] |
   | [!UICONTROL Username] | [!UICONTROL *Genehmigung *] |
   | [!UICONTROL Password] | your_password_here |
   | [!UICONTROL HTTP Signature Header] | [!UICONTROL Leave this field blank] |
   | [!UICONTROL HTTP Signature Key] | [!UICONTROL Leave this field blank] |
   | [!UICONTROL HTTP Signature Encryption Method] | [!UICONTROL None] |

1. Klicken Sie auf **[!UICONTROL Create]** , wenn Sie einen neuen Server erstellen, oder klicken Sie auf **[!UICONTROL Update]** , wenn Sie einen vorhandenen Server bearbeiten.