---
description: Die Beta-Umgebung dient zum Testen von Audience Manager-Implementierungen. In Beta vorgenommene Änderungen wirken sich nicht auf Produktionsdaten aus. Die Beta-Umgebung von Audience Manager ist eine eigenständige, eigenständige Version der Produktionsumgebung. Alle Daten, die Sie testen möchten, müssen in dieser Umgebung eingegeben und erfasst werden.
seo-description: Die Beta-Umgebung dient zum Testen von Audience Manager-Implementierungen. In Beta vorgenommene Änderungen wirken sich nicht auf Produktionsdaten aus. Die Beta-Umgebung von Audience Manager ist eine eigenständige, eigenständige Version der Produktionsumgebung. Alle Daten, die Sie testen möchten, müssen in dieser Umgebung eingegeben und erfasst werden.
seo-title: Beta-Umgebung
solution: Audience Manager
title: Beta-Umgebung
uuid: 6 a 253 f 4 e -96 e 7-4395-a 783-a 8 eb 213 b 7 daf
translation-type: tm+mt
source-git-commit: 7765dbf79c2fb6ca8c4b52fe8090c1fd11f9db27

---


# Beta-Umgebung {#beta-environment}

Die Beta-Umgebung dient zum Testen von Audience Manager-Implementierungen. In Beta vorgenommene Änderungen wirken sich nicht auf Produktionsdaten aus. Die Beta-Umgebung von Audience Manager ist eine eigenständige, eigenständige Version der Produktionsumgebung. Alle Daten, die Sie testen möchten, müssen in dieser Umgebung eingegeben und erfasst werden.

## Überblick {#overview}

<!-- beta_environment_admin.xml -->

| Dienst | URL/Hostname | Schritte zur Bereitstellung |
|--- |--- |--- |
| S3 |  | Siehe [Bereitstellen von Amazon S 3-Behältern](admin-beta-environment.md#provision-s3-buckets). |
| DCS | https &amp; amp; doppelpunkt; _/dcs-beta.demdex.net/.. | Von unserer Seite sind keine zusätzlichen Schritte erforderlich. Siehe [Zugriff auf das DCS in der Beta-Umgebung](admin-beta-environment.md#access-dcs-beta-environment). |
| Benutzeroberfläche | https &amp; amp; doppelpunkt; //bank-beta.demdex.com | Daten werden monatlich aus der Produktion in die Beta-Umgebung kopiert. Produktionsberechtigungen sind für Betaversion gültig. |
| API | https &amp; amp; doppelpunkt; _/api-beta.demdex.com/.. | Daten werden monatlich aus der Produktion in die Beta-Umgebung kopiert. Produktionsberechtigungen sind für Betaversion gültig. |

## Bereitstellen von Amazon S 3-Behältern {#provision-s3-buckets}

>[!NOTE]
>
>Wir bewegen uns von der Verwendung [!DNL FTP/SFTP]. Beachten Sie außerdem, dass ausgehende Datenübertragungen nicht für die Beta-Umgebung funktionieren.

So stellen Sie [!DNL S3] Behälter für eingehende Daten bereit:

1. Verwenden Sie die [**Techops-Hilfe für**](https://skms.adobe.com/) die SKMS-Anfrage.
1. Wechseln Sie in **[!UICONTROL Request TechOps Help]** der linken Navigationsleiste zu.
1. Geben Sie in **[!UICONTROL Request Search]** das Suchfeld in Audience Manager ein.
1. Blättern Sie in den Suchergebnissen nach unten und klicken Sie in **Audience Manager - S 3 Inbound/Outbound Account Provisioning**.
1. Füllen Sie die Felder im Bereitstellungsfenster aus und geben Sie **die Sandbox-Umgebung** in das **[!UICONTROL Environment]** Feld ein.

>[!NOTE]
>
>Wir bedauern die Verwendung [!DNL FTP/SFTP] und Verwendung [!UICONTROL Amazon S3]von. Die Gründe, weshalb wir die Verwendung von [!UICONTROL Amazon S3] empfehlen, sind in [Amazon S 3 aufgeführt: Info](https://docs.adobe.com/content/help/en/audience-manager/user-guide/reference/amazon-s3.html).

## Zugriff auf das DCS in der Beta-Umgebung {#access-dcs-beta-environment}

So greifen Sie auf die [!UICONTROL DCS] Beta-Umgebung zu:

1. Rufen Sie einen [!UICONTROL DCS] Aufruf mit dem [!DNL curl][Befehl](https://curl.haxx.se/docs/manpage.html)auf. [!DNL Curl] ist ein Tool, mit dem Daten von einem oder mehreren unterstützten Protokollen übertragen werden.

   Beispiel: `curl -v https://dcs-beta.demdex.net/event`

1. Stellen Sie sicher, dass Ihre Anforderung von der Beta-Seite [!UICONTROL DCS] bereitgestellt wurde, indem Sie nach "[!DNL sandbox]in der [!UICONTROL DCS] Antwort-Kopfzeile" suchen.

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