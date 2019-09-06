---
description: Verwenden Sie die Seite Server im Audience Manager-Verwaltungswerkzeug, um einen neuen HTTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-description: Verwenden Sie die Seite Server im Audience Manager-Verwaltungswerkzeug, um einen neuen HTTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.
seo-title: HTTP-Server erstellen oder bearbeiten
title: HTTP-Server erstellen oder bearbeiten
uuid: 1 ef 0 e 751-e 239-4 dc 6-a 4 f 6-73 cc 05686807
translation-type: tm+mt
source-git-commit: 57d7a92265e565b6c411e4cfa5c579e40eb837b3

---


# HTTP-Server erstellen oder bearbeiten {#create-or-edit-an-http-server}

Verwenden Sie die [!UICONTROL Servers] Seite im Audience Manager-Verwaltungswerkzeug, um einen neuen HTTP-Server zu erstellen oder einen vorhandenen Server zu bearbeiten.

>[!NOTE]
>
>Sie müssen über die [!UICONTROL DEXADMIN] Rolle verfügen, um neue Server zu erstellen oder bestehende Server zu bearbeiten.

1. Um einen neuen Server zu erstellen, gehen Sie zu **[!UICONTROL Servers]** &gt; **[!UICONTROL Create Server]**. To edit an existing server, click the desired server in the **[!UICONTROL Label]** column.
1. Geben Sie die gewünschte Beschriftung für diesen Server an.
1. Wählen Sie aus der **[!UICONTROL Protocol]** Dropdownliste das gewünschte Protokoll aus: [!DNL HTTP].
1. Füllen Sie die Felder aus:

   * **[!UICONTROL Domain]:** Geben Sie die gewünschte Domäne (Host) für diesen Server an.
   * **[!UICONTROL Port]:** Geben Sie den gewünschten Anschluss für diesen Server an. Der Standardanschluss wird für jeden Verschlüsselungstyp angezeigt. Sie können den Standardanschluss ändern, falls erforderlich.
   * **[!UICONTROL Maximum Users Per Request]:** Geben Sie die maximale Anzahl von Benutzern pro Anforderung für diesen Server an.
   * **[!UICONTROL URL Prefix]:** Geben Sie das [!DNL URL] für diesen Server zu verwendende Präfix an.
   * **[!UICONTROL Authentication URL]:** Geben Sie die [!UICONTROL Authentication URL] für diesen `HTTP` Server an.
   * **[!UICONTROL Authentication]:** Geben Sie die gewünschte Authentifizierungsmethode an: **[!UICONTROL None]**, **[!UICONTROL Username/Password]** oder **[!UICONTROL SSH Key]**.
   * **[!UICONTROL HTTP Signature Header]:** Der Name der [!DNL HTTP] Kopfzeile, die vom Kunden bereitgestellt wird, der den [!DNL HTTP] Signaturschlüssel enthält. Der Standardwert ist [!UICONTROL X-Signature]wie im folgenden Beispiel dargestellt:

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

   * **[!UICONTROL HTTP Signature Key]:** Der Schlüssel, der zum Signieren der [!DNL HTTP] Anforderung vom Kunden verwendet wird.
   * **[!UICONTROL Show Signature Key]:** Schalten Sie ein, ob die Unterschrift im Browser angezeigt werden soll oder nicht.
   * **[!UICONTROL HTTP Signature Encryption Method]:** Geben Sie die Methode an, die wir zum Verschlüsseln der Signatur verwenden. Verwenden [!UICONTROL SHA1] Sie dies, wenn der Kunde nicht anderweitig bevorzugt wird.
   >[!NOTE]
   >
   >Wenn Sie [die oauth 2.0-Authentifizierung für Echtzeit-Datenübertragungen](https://docs.adobe.com/help/en/audience-manager/user-guide/implemenation-integration-guides/receiving-audience-data/real-time-outbound-transfers/oauth-in-outbound-transfers.html) für einen Partner aktivieren möchten, füllen Sie die Felder wie in der folgenden Tabelle aus. *Die kursiv gedruckten Felder* müssen genau wie in der Tabelle ausgefüllt werden.

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
   | [!UICONTROL Password] | your_ password_ here |
   | [!UICONTROL HTTP Signature Header] | [!UICONTROL Leave this field blank] |
   | [!UICONTROL HTTP Signature Key] | [!UICONTROL Leave this field blank] |
   | [!UICONTROL HTTP Signature Encryption Method] | [!UICONTROL None] |

1. Klicken **[!UICONTROL Create]** Sie auf, wenn Sie einen neuen Server erstellen, oder klicken **[!UICONTROL Update]** Sie auf, wenn Sie einen vorhandenen Server bearbeiten.