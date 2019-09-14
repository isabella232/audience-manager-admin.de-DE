---
description: Sie sollten Ihre Kunden auffordern, sich im Klaren zu sein, wenn sie mit den Audience Manager-APIs arbeiten.
seo-description: Sie sollten Ihre Kunden auffordern, sich im Klaren zu sein, wenn sie mit den Audience Manager-APIs arbeiten.
seo-title: API-Anforderungen und Empfehlungen
title: API-Anforderungen und Empfehlungen
uuid: eba9cf92-f0c8-4394-8532-0de9a2e7b103
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54

---


# API-Anforderungen und Empfehlungen {#api-requirements-and-recommendations}

Sie sollten Ihre Kunden dazu anhalten, sich darüber im Klaren zu sein, wann sie mit Audience Manager [!DNL API]arbeiten.

## Voraussetzungen {#requirements}

Beachten Sie beim Arbeiten mit [!DNL Audience Manager][!DNL API] Code Folgendes:

* **** Abfrageparameter: Sofern nicht anders angegeben, sind alle Anforderungsparameter erforderlich.
* **[!DNL JSON]** Inhaltstyp: Geben Sie `content-type: application/json` und *geben Sie Ihren Code ein* `accept: application/json`.

* **** Anforderungen und Antworten: Senden von Anforderungen als korrekt formatiertes [!DNL JSON] Objekt [!DNL Audience Manager] antwortet mit [!DNL JSON] formatierten Daten. Serverantworten können angeforderte Daten, einen Statuscode oder beides enthalten.

* **** Zugriff: Ihr [!DNL Audience Manager] Berater stellt Ihnen eine Client-ID und einen Schlüssel zur Verfügung, mit denen Sie [!DNL API] Anforderungen stellen können.

* **** Dokumentation und Codebeispiele: Text in *Kursivschrift* stellt eine Variable dar, die Sie beim Herstellen oder Empfangen von [!DNL API] Daten angeben oder übermitteln. Ersetzen Sie *kursiv gedruckten* Text durch Ihren eigenen Code, Ihre eigenen Parameter oder andere erforderliche Informationen.

## Empfehlungen: Erstellen eines generischen API-Benutzers {#recommendations}

Es wird empfohlen, ein separates technisches Benutzerkonto für die Arbeit mit Audience Manager [!DNL API]zu erstellen. Hierbei handelt es sich um ein generisches Konto, das nicht an einen bestimmten Benutzer im Unternehmen Ihres Kunden gebunden ist oder mit diesem verknüpft ist. Mit diesem [!DNL API] Benutzerkonto können Sie zwei Dinge erreichen:

* Identifizieren Sie, welcher Dienst die Anwendung aufruft [!DNL API] (z. B. Aufrufe von einer Client-App, die unsere [!DNL API]s verwenden, oder Aufrufe von Massenänderungen).
* Gewähren Sie ununterbrochenen Zugriff auf die [!DNL API]s. Ein Konto, das an einen bestimmten Mitarbeiter gebunden ist, kann gelöscht werden, wenn er das Unternehmen verlässt. Dadurch wird verhindert, dass Ihre Kunden mit dem verfügbaren [!DNL API] Code arbeiten. Ein generisches Konto, das nicht an einen bestimmten Mitarbeiter gebunden ist, hilft, dieses Problem zu vermeiden.

Als Beispiel oder Anwendungsfall für diese Art von Konto, nehmen wir an, dass Ihre Kunden mit den [Massenverwaltungstools](https://docs.adobe.com/content/help/en/audience-manager/user-guide/reference/bult-management-tools/bulk-management-intro.html)viele Segmente gleichzeitig ändern möchten. Dazu benötigen sie [!DNL API] Zugriff. Anstatt einem bestimmten Benutzer Berechtigungen hinzuzufügen, erstellen Sie ein unspezifisches [!DNL API] Benutzerkonto, das über die entsprechenden Anmeldeinformationen, den entsprechenden Schlüssel und das geheime Schlüssel zum [!DNL API] Aufrufen verfügt. Dies ist auch dann nützlich, wenn Kunden eigene Anwendungen entwickeln, die die [!DNL Audience Manager] [!DNL API]s verwenden.
