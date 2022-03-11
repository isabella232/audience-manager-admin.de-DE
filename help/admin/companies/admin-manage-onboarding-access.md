---
description: Um das versehentliche Einbinden von Dateien und Daten in Zieldatenquellen anderer Partner oder Kunden zu verhindern, hat Audience Manager eine Zuordnungsanforderung zwischen Partner-ID (PID) und den Datenquellen anderer Partner hinzugefügt.
title: Onboarding-Zugriff für Zweitanbieterdaten verwalten
source-git-commit: 6c88979f876909bc32b5238605cb4a352e327a00
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Onboarding-Zugriff für Daten von Zweitanbietern verwalten {#manage-onboarding-access-for-second-party-data}

Um das versehentliche Einbinden von Dateien und Daten in Zieldatenquellen anderer Partner zu verhindern, hat der Audience Manager eine Zuordnungsanforderung zwischen Partner-ID (PID) und Datenquellen (DPID) anderer Partner hinzugefügt. Weitere Informationen zu PID und DPID finden Sie im Abschnitt [Index der Audience Manager-IDs](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/ids-in-aam.html).

Wenn ein Audience Manager-Partner oder -Kunde zu Zwecken der Datenfreigabe von Zweitanbietern Dateien in eine Zieldatenquelle aufnehmen möchte, deren Eigentümer er nicht ist, muss er eine Zuordnung zwischen seiner Partner-ID (PID) und dieser spezifischen Datenquelle (DPID) anfordern. Wenn die Zuordnung fehlt, werden die Dateien nicht vom eingehenden Datenauftrag verarbeitet und die Daten werden nicht in Audience Manager integriert.

Um dieses Mapping zu erstellen, senden Sie ein Jira-Ticket an das Audience Manager Engineering-Team. Beispiel für ein Jira-Ticket anzeigen [here](https://jira.corp.adobe.com/browse/AAM-60353). Sie müssen keine Zuordnungen für bestehende Datenfreigabe-Beziehungen anfordern.
