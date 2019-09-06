---
description: Dinge, die Sie Ihren Kunden empfehlen sollten, sich bewusst zu sein, wann sie mit den Audience Manager-apis arbeiten.
seo-description: Dinge, die Sie Ihren Kunden empfehlen sollten, sich bewusst zu sein, wann sie mit den Audience Manager-apis arbeiten.
seo-title: API-Anforderungen und Empfehlungen
title: API-Anforderungen und Empfehlungen
uuid: eba 9 cf 92-f 0 c 8-4394-8532-0 de 9 a 2 e 7 b 103
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54

---


# API-Anforderungen und Empfehlungen {#api-requirements-and-recommendations}

Dinge, die Sie Ihren Kunden empfehlen sollten, sich bewusst zu sein, wann sie mit Audience Manager [!DNL API]arbeiten.

## Voraussetzungen {#requirements}

Beachten Sie Folgendes, wenn Sie [!DNL Audience Manager][!DNL API] mit Code arbeiten:

* **Anforderungsparameter:** Alle Anforderungsparameter sind erforderlich, falls nicht anders angegeben.
* **[!DNL JSON]Inhaltstyp:** Geben Sie an `content-type: application/json`*und* `accept: application/json` in Ihrem Code.

* **Anforderungen und Antworten:** Senden Sie Anforderungen als ein ordnungsgemäß formatiertes [!DNL JSON] Objekt. [!DNL Audience Manager] mit [!DNL JSON] formatierten Daten beantwortet. Serverantworten können angeforderte Daten, einen Status-Code oder beides enthalten.

* **Zugriff:** Ihr [!DNL Audience Manager] Berater stellt Ihnen eine Client-ID und einen Schlüssel zur Verfügung, mit dem Sie Anforderungen erstellen [!DNL API] können.

* **Dokumentation und Codebeispiele:** *Kursiv gedruckter Text* stellt eine Variable dar, die Sie beim Erstellen oder Empfangen [!DNL API] von Daten bereitstellen oder weitergeben. Ersetzen *Sie Text mit Kursivschrift* durch Ihren eigenen Code, Parameter oder andere erforderliche Informationen.

## Recommendations: Generische API-Benutzer erstellen {#recommendations}

Wir empfehlen, ein separates technisches Benutzerkonto für die Arbeit mit Audience Manager [!DNL API]zu erstellen. Dies ist ein generisches Konto, das nicht an einen bestimmten Benutzer in Ihrem Kundenunternehmen gebunden oder mit ihm verknüpft ist. Diese Art [!DNL API] von Benutzerkonto hilft dabei, zwei Dinge zu erreichen:

* Identifizieren Sie, welcher Dienst den [!DNL API] Dienst aufruft (z. B. Aufrufe einer Client-App, die unsere [!DNL API]s oder von Massenänderungen verwenden).
* Stellen Sie unterbrechungsfreien Zugriff auf [!DNL API]die s. Ein mit einem bestimmten Mitarbeiter verknüpftes Konto kann gelöscht werden, wenn sie das Unternehmen verlassen. Dadurch verhindern Sie, dass Ihre Kunden mit dem verfügbaren [!DNL API] Code arbeiten. Ein generisches Konto, das nicht an einen bestimmten Mitarbeiter gebunden ist, hilft dabei, dieses Problem zu vermeiden.

Nehmen wir als Beispiel an, dass Ihre Kunden viele Segmente auf einmal mit den [Massenverwaltungstools ändern](https://docs.adobe.com/content/help/en/audience-manager/user-guide/reference/bult-management-tools/bulk-management-intro.html)möchten. Dazu benötigen sie [!DNL API] Zugriff. Anstatt einem bestimmten Benutzer Berechtigungen hinzuzufügen, erstellen Sie ein nicht spezifisches [!DNL API] Benutzerkonto, das über die entsprechenden Anmeldeinformationen, Schlüssel und geheimen Schlüssel verfügt, um [!DNL API] Aufrufe durchzuführen. Dies ist auch nützlich, wenn der Kunde seine eigenen Anwendungen entwickelt, die die [!DNL Audience Manager][!DNL API]s verwenden.
