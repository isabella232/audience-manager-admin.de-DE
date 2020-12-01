---
description: Sie sollten Ihre Kunden darauf hinweisen, dass sie wissen, wann sie mit den Audience Manager-APIs arbeiten.
seo-description: Sie sollten Ihre Kunden darauf hinweisen, dass sie wissen, wann sie mit den Audience Manager-APIs arbeiten.
seo-title: API-Anforderungen und -Empfehlungen
title: API-Anforderungen und -Empfehlungen
uuid: eba9cf92-f0c8-4394-8532-0de9a2e7b103
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 3%

---


# API-Anforderungen und -Empfehlungen {#api-requirements-and-recommendations}

Dinge, die Sie Ihren Kunden empfehlen sollten, sich bewusst zu sein, wenn sie mit dem Audience Manager [!DNL API]s arbeiten.

## Anforderungen {#requirements}

Beachten Sie Folgendes, wenn Sie mit [!DNL Audience Manager] [!DNL API]-Code arbeiten:

* **Anforderungsparameter:** Alle Anforderungsparameter sind erforderlich, sofern nicht anders angegeben.
* **[!DNL JSON]Inhaltstyp:** Geben Sie  `content-type: application/json` ** `accept: application/json` Ihren Code an.

* **Anforderungen und Antworten:** Senden von Anforderungen als korrekt formatiertes  [!DNL JSON] Objekt. [!DNL Audience Manager] antwortet mit  [!DNL JSON] formatierten Daten. Serverantworten können angeforderte Daten, einen Statuscode oder beides enthalten.

* **Zugriff:** Ihr  [!DNL Audience Manager] Berater stellt Ihnen eine Client-ID und einen Schlüssel zur Verfügung, mit denen Sie  [!DNL API] Anforderungen stellen können.

* **Dokumentations- und Codebeispiele:** Text in  ** Kursivschrift stellt eine Variable dar, die Sie beim Herstellen oder Empfangen von  [!DNL API] Daten angeben oder weitergeben. Ersetzen Sie den Text *kursiv* durch Ihren eigenen Code, Ihre eigenen Parameter oder andere erforderliche Informationen.

## Recommendations: Generischen API-Benutzer {#recommendations} erstellen

Es wird empfohlen, ein separates technisches Benutzerkonto für die Arbeit mit dem Audience Manager [!DNL API]s zu erstellen. Hierbei handelt es sich um ein generisches Konto, das nicht an einen bestimmten Benutzer im Unternehmen Ihres Kunden gebunden ist oder mit diesem verknüpft ist. Dieser Typ von [!DNL API]-Benutzerkonto hilft dabei, zwei Dinge zu erreichen:

* Identifizieren Sie, welchen Dienst [!DNL API] aufruft (z. B. Aufrufe von einer Client-App, die unsere [!DNL API]s verwenden, oder Aufrufe von Massenänderungen).
* Stellen Sie unterbrechungsfreien Zugriff auf die [!DNL API]s bereit. Ein Konto, das an einen bestimmten Mitarbeiter gebunden ist, kann gelöscht werden, wenn er die Firma verlässt. Dadurch wird verhindert, dass Ihre Kunden mit dem verfügbaren [!DNL API]-Code arbeiten. Ein generisches Konto, das nicht an einen bestimmten Mitarbeiter gebunden ist, hilft, dieses Problem zu vermeiden.

Als Beispiel oder Anwendungsfall für diesen Kontotyp sollten Ihre Kunden mit den [Massenverwaltungswerkzeugen](https://docs.adobe.com/content/help/en/audience-manager/user-guide/reference/bult-management-tools/bulk-management-intro.html) viele Segmente gleichzeitig ändern. Dazu benötigen sie [!DNL API] Zugriff. Anstatt einem bestimmten Benutzer Berechtigungen hinzuzufügen, erstellen Sie ein unspezifisches [!DNL API]-Benutzerkonto, das über die entsprechenden Anmeldeinformationen, den entsprechenden Schlüssel und das geheime Schlüssel zum Durchführen von [!DNL API]-Aufrufen verfügt. Dies ist auch dann nützlich, wenn der Client eigene Anwendungen entwickelt, die [!DNL Audience Manager] [!DNL API]s verwenden.
