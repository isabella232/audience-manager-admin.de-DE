---
description: 'Verwenden Sie beim Debugging von Kundenproblemen zuerst die Prüfprotokollierung. '
seo-description: 'Verwenden Sie beim Debugging von Kundenproblemen zuerst die Prüfprotokollierung. '
seo-title: Prüfprotokollierung
title: Prüfprotokollierung
uuid: null
translation-type: tm+mt
source-git-commit: 190ba5c1215782e46c8e544c10679d451fbed134

---


# Prüfprotokollierung {#audit-logging}

Verwenden Sie [!UICONTROL  Audit Logging] als Erstes, wenn Sie Kundenprobleme debuggen möchten.

> [!NOTE]
>
>[!UICONTROL Audit Logging] befindet sich derzeit in der Entwicklung und kann geändert werden. Bitte protokollieren Sie alle Probleme, mit denen Sie konfrontiert sind [!DNL JIRA] ([!DNL UI] Team)

![Prüfprotokollierungsansicht](assets/audit-logging-img.png)

Wählen Sie in der Dropdown-Auswahl **Prüfungstyp** eine der folgenden Optionen:

* [!UICONTROL Partner]
* [!UICONTROL User]
* [!UICONTROL Group]
* [!UICONTROL Datasource Summary]
* [!UICONTROL General Datasource]
* [!UICONTROL Merge Rule Datasource]
* [!UICONTROL Data Feed]
* [!UICONTROL Data Feed Subscription]
* [!UICONTROL Trait Summary]
* [!UICONTROL Trait Rule]
* [!UICONTROL Segment Summary]
* [!UICONTROL Destination Summary]
* [!UICONTROL Server to Server Destination]
* [!UICONTROL Derived Signal]
* [!UICONTROL Model]
* [!UICONTROL Segment Test Group]

Die **Objekt-ID** ist die ID des gesuchten Elements. Die nachstehende Tabelle zeigt, welche ID in jedem Fall der Objekt-ID entspricht:

| Prüfungstyp | Objekt-ID |
---------|----------|
| [!UICONTROL Partner] | Partner-ID - PID |
| [!UICONTROL User] | Benutzer-ID |
| [!UICONTROL Group] | B3 |
| [!UICONTROL Datasource Summary] | Datenquellen-ID |
| [!UICONTROL General Datasource] | Datenquellen-ID |
| [!UICONTROL Merge Rule Datasource] | Datenquellen-ID |
| [!UICONTROL Data Feed] | Datenfeed-ID |
| [!UICONTROL Data Feed Subscription] | Datenfeed-ID |
| [!UICONTROL Trait Summary] | SID (Eigenschaft) |
| [!UICONTROL Trait Rule] | SID (Eigenschaft) |
| [!UICONTROL Segment Summary] |  |
| [!UICONTROL Destination Summary] |  |
| [!UICONTROL Server-to-Server Destination] | Keine |
| [!UICONTROL Derived Signal] | Keine |
| [!UICONTROL Model] | Keine |
| [!UICONTROL Segment Test Group] | Keine |

Verwenden Sie [!UICONTROL Start Date] ([!DNL UTC]) und [!UICONTROL End Date] ([!DNL UTC]), um das Zeitintervall der Protokolle einzugrenzen.