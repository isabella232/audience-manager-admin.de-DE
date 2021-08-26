---
description: Dinge, die Sie Ihren Kunden empfehlen sollten, sich dessen bewusst zu sein, wenn sie mit den Audience Manager-APIs arbeiten.
seo-description: Things you should encourage your clients to be aware of when they're working with the Audience Manager APIs.
seo-title: API Requirements and Recommendations
title: API-Anforderungen und -Empfehlungen
uuid: eba9cf92-f0c8-4394-8532-0de9a2e7b103
exl-id: 24f90732-31a6-436d-862b-e6871d279c7a
source-git-commit: 79415eba732c2a6d50f04124774664f788ccc78c
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 2%

---

# API-Anforderungen und -Empfehlungen {#api-requirements-and-recommendations}

Dinge, die Sie dazu anregen sollten, dass Ihre Kunden wissen, wann sie mit dem Audience Manager [!DNL API]s arbeiten.

## Anforderungen {#requirements}

Beachten Sie Folgendes beim Arbeiten mit [!DNL Audience Manager] [!DNL API]-Code:

* **Anforderungsparameter:** Alle Anforderungsparameter sind erforderlich, sofern nicht anders angegeben.
* **[!DNL JSON]Inhaltstyp:** Geben Sie  `content-type: application/json` ** `accept: application/json` und Ihren Code an.

* **Anforderungen und Antworten:** Anforderungen als ordnungsgemäß formatiertes  [!DNL JSON] Objekt senden. [!DNL Audience Manager] antwortet mit  [!DNL JSON] formatierten Daten. Serverantworten können angeforderte Daten, einen Statuscode oder beides enthalten.

* **Zugriff:** Ihr  [!DNL Audience Manager] Berater stellt Ihnen eine Client-ID und einen Schlüssel zur Verfügung, mit denen Sie  [!DNL API] Anfragen stellen können.

* **Dokumentation und Codebeispiele:** Text in  ** Kursivschrift stellt eine Variable dar, die Sie beim Erstellen oder Empfangen von  [!DNL API] Daten bereitstellen oder übergeben. Ersetzen Sie den Text *kursiv* durch Ihren eigenen Code, Ihre eigenen Parameter oder andere erforderliche Informationen.

## Recommendations: Erstellen eines generischen API-Benutzers {#recommendations}

Es wird empfohlen, ein eigenes technisches Benutzerkonto für die Arbeit mit dem Audience Manager [!DNL API]s zu erstellen. Dies ist ein generisches Konto, das nicht an einen bestimmten Benutzer in der Organisation Ihres Kunden gebunden ist oder mit diesem verknüpft ist. Dieser Typ von [!DNL API] Benutzerkonto hilft bei der Erreichung von zwei Aspekten:

* Ermitteln Sie, welcher Dienst die [!DNL API] aufruft (z. B. Aufrufe von einer Client-App, die unsere [!DNL API]s verwenden oder Massenänderungen vornehmen).
* Gewähren Sie unterbrechungsfreien Zugriff auf die [!DNL API]s. Ein an einen bestimmten Mitarbeiter gebundenes Konto kann gelöscht werden, wenn er das Unternehmen verlässt. Dadurch wird verhindert, dass Ihre Kunden mit dem verfügbaren [!DNL API]-Code arbeiten. Ein generisches Konto, das nicht an einen bestimmten Mitarbeiter gebunden ist, hilft, dieses Problem zu vermeiden.

Nehmen wir als Beispiel oder Anwendungsfall für diesen Kontotyp an, Ihre Kunden möchten mit den [Tools für die Massenverwaltung](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/bult-management-tools/bulk-management-intro.html) viele Segmente gleichzeitig ändern. Dazu benötigen sie [!DNL API] Zugriff. Anstatt einem bestimmten Benutzer Berechtigungen hinzuzufügen, erstellen Sie ein unspezifisches [!DNL API]-Benutzerkonto mit den entsprechenden Anmeldeinformationen, Schlüsseln und Geheimnissen, um [!DNL API]-Aufrufe durchzuführen. Dies ist auch dann nützlich, wenn die Kunden eigene Anwendungen entwickeln, die die [!DNL Audience Manager] [!DNL API]s verwenden.
