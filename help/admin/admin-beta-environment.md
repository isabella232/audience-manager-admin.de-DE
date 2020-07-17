---
description: Die Beta-Umgebung dient zum Testen von Audience Manager-Implementierungen. Änderungen, die in der Beta-Version vorgenommen werden, wirken sich nicht auf Produktionsdaten aus. Die Audience Manager Beta-Umgebung ist eine kleinere, eigenständige Version der Umgebung. Alle Daten, die Sie testen möchten, müssen in diese Umgebung eingegeben und gesammelt werden.
seo-description: Die Beta-Umgebung dient zum Testen von Audience Manager-Implementierungen. Änderungen, die in der Beta-Version vorgenommen werden, wirken sich nicht auf Produktionsdaten aus. Die Audience Manager Beta-Umgebung ist eine kleinere, eigenständige Version der Umgebung. Alle Daten, die Sie testen möchten, müssen in diese Umgebung eingegeben und gesammelt werden.
seo-title: Beta-Umgebung
solution: Audience Manager
title: Beta-Umgebung
uuid: 6a253f4e-96e7-4395-a783-a8eb213b7daf
translation-type: tm+mt
source-git-commit: 7765dbf79c2fb6ca8c4b52fe8090c1fd11f9db27
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 3%

---


# Beta-Umgebung {#beta-environment}

Die Beta-Umgebung dient zum Testen von Audience Manager-Implementierungen. Änderungen, die in der Beta-Version vorgenommen werden, wirken sich nicht auf Produktionsdaten aus. Die Audience Manager Beta-Umgebung ist eine kleinere, eigenständige Version der Umgebung. Alle Daten, die Sie testen möchten, müssen in diese Umgebung eingegeben und gesammelt werden.

## Überblick {#overview}

<!-- beta_environment_admin.xml -->

| Diensleistung | URL/Hostname | Schritte zur Bereitstellung |
|--- |--- |--- |
| S3 |  | Siehe [Bereitstellung von Amazon S3-Behältern](admin-beta-environment.md#provision-s3-buckets). |
| DCS | https&amp;colon;//dcs-beta.demdex.net/... | Keine zusätzlichen Schritte von unserer Seite aus erforderlich. Siehe [Zugriff auf den DCS in der Beta-Umgebung](admin-beta-environment.md#access-dcs-beta-environment). |
| Benutzeroberfläche | https&amp;colon;//bank-beta.demdex.com | Die Daten werden monatlich von der Produktion in die Beta-Umgebung kopiert. Produktionsberechtigungen sind für Beta gültig. |
| API | https&amp;colon;//api-beta.demdex.com/... | Die Daten werden monatlich von der Produktion in die Beta-Umgebung kopiert. Produktionsberechtigungen sind für Beta gültig. |

## Bereitstellung von Amazon S3-Buckets {#provision-s3-buckets}

>[!NOTE]
>
>Wir bewegen uns davon ab, [!DNL FTP/SFTP]zu nutzen. Beachten Sie auch, dass ausgehende Datenübertragungen für die Beta-Umgebung nicht funktionieren.

So stellen Sie [!DNL S3] Behälter für eingehende Daten bereit:

1. Verwenden Sie die [**SKMS Request TechOps-Hilfe **](https://skms.adobe.com/).
1. Gehen Sie zur **[!UICONTROL Request TechOps Help]** linken Navigationsleiste.
1. Geben Sie **[!UICONTROL Request Search]** in das Suchfeld Audience Manager ein.
1. Blättern Sie nach unten in den Suchergebnissen und klicken Sie auf **Audience Manager - S3 Inbound/Outbound Account Provisioning**.
1. Füllen Sie die Felder im Bereitstellungsfenster aus und geben Sie **Sandbox-Umgebung** in das **[!UICONTROL Environment]** Feld ein.

>[!NOTE]
>
>Wir halten die Verwendung von [!DNL FTP/SFTP] und fördern die Verwendung von [!UICONTROL Amazon S3]. Die Gründe, warum wir die Verwendung von [!UICONTROL Amazon S3] sind in [Amazon S3:Info](https://docs.adobe.com/content/help/en/audience-manager/user-guide/reference/amazon-s3.html)aufgeführt.

## Zugriff auf den DCS in der Beta-Umgebung {#access-dcs-beta-environment}

So greifen Sie auf die [!UICONTROL DCS] Beta-Umgebung zu:

1. Führen Sie einen [!UICONTROL DCS] Aufruf mithilfe des [!DNL curl] Befehls [](https://curl.haxx.se/docs/manpage.html)durch. [!DNL Curl] ist ein Tool zum Übertragen von Daten von oder auf einen Server unter Verwendung eines von vielen unterstützten Protokollen.

   Beispiel: `curl -v https://dcs-beta.demdex.net/event`

1. Stellen Sie sicher, dass Ihre Anfrage von der Beta-Version bearbeitet wurde, [!UICONTROL DCS] indem Sie nach &quot;[!DNL sandbox]&quot;in der [!UICONTROL DCS] Antwort-Kopfzeile suchen.

   Beispiel:

   ```
   curl -v http://dcs-beta.demdex.net/?event
   [...]
   < DCS: va6-sandbox-dcs-3.sandbox.demdex.com <release_number>
   [...]
   ```

<!--
1. Determine the load balancer's endpoint IP addresses.

   Run the `dig` [command](https://en.wikipedia.org/wiki/Dig_(command)) to determine the IP address of the nearest load balancer. The `dig` command queries the Domain Name System and returns the name and IP addresses of the Audience Manager [!UICONTROL Data Collection Servers (DCS)].

   ```
   dig dcs-beta.demdex.net
   ...
   dcs-sandbox-1754093861.us-east-1.elb.amazonaws.com. 60 IN A 52.87.15.51
   dcs-sandbox-1754093861.us-east-1.elb.amazonaws.com. 60 IN A 50.16.150.8
   dcs-sandbox-1754093861.us-east-1.elb.amazonaws.com. 60 IN A 52.2.228.100
   ```

1. Using one of the addresses in the above table, add a static DNS entry in the [!DNL `/etc/hosts`] file.

   On Windows, modify [!DNL `c:\WINDOWS\system32\drivers\etc\hosts`].

   For example:

[!DNL `52.87.15.51 samplepartner.demdex.net`]

   >[!NOTE]
   >
   >The addresses change occasionally, so you must keep your [!DNL /etc/hosts] file up to date.

   Additionally, if you need to set up ID synchronization, you must add a similar entry for [!DNL dpm.demdex.net.]

[!DNL `52.87.15.51 dpm.demdex.net`] [!DNL]. 

1. Make a [!UICONTROL DCS] call, using the `curl` [command](https://curl.haxx.se/docs/manpage.html). Curl is a tool to transfer data from or to a server, using one of many supported protocols.

   For example:

[!DNL `https://<domain>/event?product=camera`] 

1. Verify that your request was served by the beta [!UICONTROL DCS] by looking for "sandbox" in the [!UICONTROL DCS] response header.

   For example:

   ```
   curl -v https://dcs-beta.demdex.net/?event
   [...]
   < DCS: va6-sandbox-dcs-3.sandbox.demdex.com <release_number>
   [...]
   ```
-->