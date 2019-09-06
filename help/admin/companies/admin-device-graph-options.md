---
description: Die Gerätediagrammoptionen sind für Unternehmen verfügbar, die an der Adobe Experience Cloud Device Co-op teilnehmen. Wenn ein Kunde außerdem über eine vertragliche Beziehung mit einem Drittanbieter-Diagrammanbieter verfügt, der in Audience Manager integriert ist, zeigt dieser Abschnitt Optionen für dieses Gerätediagramm an. Diese Optionen finden Sie unter Unternehmen > Firmenname > Profil > Gerätediagrammoptionen.
seo-description: Die Gerätediagrammoptionen sind für Unternehmen verfügbar, die an der Adobe Experience Cloud Device Co-op teilnehmen. Wenn ein Kunde außerdem über eine vertragliche Beziehung mit einem Drittanbieter-Diagrammanbieter verfügt, der in Audience Manager integriert ist, zeigt dieser Abschnitt Optionen für dieses Gerätediagramm an. Diese Optionen finden Sie unter Unternehmen > Firmenname > Profil > Gerätediagrammoptionen.
seo-title: Gerätediagrammoptionen für Unternehmen
title: Gerätediagrammoptionen für Unternehmen
uuid: a 8 sed 433-710 c -4 a 8 f-a 0 d 7-ea 89 d 010 a 7 a 5
translation-type: tm+mt
source-git-commit: 10adb6b06160f5a5c4068483b407e5798fc10150

---


# Gerätediagrammoptionen für Unternehmen {#device-graph-options-for-companies}

Sie [!UICONTROL Device Graph Options] sind für Unternehmen verfügbar, die an [!DNL Adobe Experience Cloud Device Co-op]der Seite teilnehmen. Wenn ein Kunde außerdem über eine vertragliche Beziehung mit einem Drittanbieter-Diagrammanbieter verfügt, der in Audience Manager integriert ist, zeigt dieser Abschnitt Optionen für dieses Gerätediagramm an. Diese Optionen befinden sich unter [!UICONTROL Companies] &gt; Firmenname &gt; [!UICONTROL Profile] &gt; [!UICONTROL Device Graph Options].

![](assets/adminUIdataSource.png)

Diese Abbildung verwendet allgemeine Namen für die Optionen des Drittanbietergeräts. In der Produktion stammen diese Namen vom Gerätediagrammanbieter und können von den hier gezeigten unterschieden werden. Beispielsweise werden die [!DNL LiveRamp] Optionen in der Regel angezeigt (nicht immer):

* Mit "[!DNL LiveRamp]"
* Enthält einen mittleren Namen, der variabel ist
* Beenden mit "[!UICONTROL - Household]oder «[!UICONTROL -Person]

## Gerätediagrammoptionen definiert {#device-graph-options-defined}

Die hier ausgewählten Gerätediagrammoptionen stellen [!UICONTROL Device Options] die Auswahlmöglichkeiten ein oder blenden sie ein, wenn sie einen [!DNL Audience Manager][!UICONTROL Profile Merge Rule]Kunden erstellen.

### Co-op Device Graph {#co-op-graph}

Kunden, die an der [Adobe Experience Cloud-Gerätekooperation teilnehmen,](https://marketing.adobe.com/resources/help/en_US/mcdc/) verwenden diese Optionen, um eine [!UICONTROL Profile Merge Rule] mit [deterministischen und wahrscheinlichen Daten zu erstellen](https://marketing.adobe.com/resources/help/en_US/mcdc/mcdc-links.html). Die [!DNL Corporate Provisioning Team] Option aktiviert und deaktiviert diese Option über einen Back-End [!DNL API] -Aufruf. Sie können diese Kontrollkästchen nicht in [!DNL Admin UI]der Außerdem schließen sich die **[!UICONTROL Co-op Device Graph]** Optionen und **[!UICONTROL Company Device Graph]** Optionen gegenseitig aus. Kunden können uns fragen, ob sie eine oder eine andere aktivieren, aber nicht beide. Wenn diese Option aktiviert ist, stellt sie die **[!UICONTROL Co-op Device Graph]** Steuerung in den [!UICONTROL Device Options] Einstellungen für einen [!UICONTROL Profile Merge Rule]bereit.

![](assets/adminUI1.png)

### Firmengerätediagramm {#company-graph}

Diese Option richtet [!DNL Analytics] sich an Kunden, die die [!UICONTROL People] Metrik in ihrer [!DNL Analytics] Report Suite verwenden. Die [!DNL Corporate Provisioning Team] Option aktiviert und deaktiviert diese Option über einen Back-End [!DNL API] -Aufruf. Sie können diese Kontrollkästchen nicht in [!DNL Admin UI]der Außerdem schließen sich die **[!UICONTROL Company Device Graph]** Optionen und **[!UICONTROL Co-op Device Graph]** Optionen gegenseitig aus. Kunden können uns fragen, ob sie eine oder eine andere aktivieren, aber nicht beide. Wenn aktiviert:

* Dieses Gerätediagramm verwendet deterministische Daten, die dem Unternehmen gehören, das Sie konfigurieren (keine probabilistischen Daten).
* [!DNL Audience Manager] erstellt automatisch einen [!UICONTROL Data Source] benannten `*`Partnernamen`*-Company Device Graph-Person`. Auf der [!UICONTROL Data Source] Detailseite können [!DNL Audience Manager] Kunden den Namen, die Beschreibung und die Anwendung [von Datenexportsteuerelementen](https://marketing.adobe.com/resources/help/en_US/aam/c_dec.html) auf diese Datenquelle ändern.
* [!DNL Audience Manager] Kunden *sehen keine* neue Einstellung im [!UICONTROL Device Options] Abschnitt für einen [!UICONTROL Profile Merge Rule].

### Liveramp Device Graph (Person oder Haushalt) {#liveramp-device-graph}

Diese Kontrollkästchen sind aktiviert, wenn [!DNL Admin UI] ein Partner ein und [!UICONTROL Data Source] auswählt **[!UICONTROL Use as an Authenticated Profile]** und/oder **[!UICONTROL Use as a Device Graph]** Die Namen dieser Einstellungen werden vom Gerätediagramm des Drittanbieters bestimmt (z. [!DNL LiveRamp]B. [!DNL TapAd]usw.). Wenn diese Option aktiviert ist, wird das Unternehmen, das Sie konfigurieren, die von diesen Gerätediagrammen bereitgestellten Daten verwenden.

![](assets/adminUI2.png)

>[!MORE_ LIKE_ THIS]
>
>* [Regeloptionen für Profilzusammenführung definiert](https://marketing.adobe.com/resources/help/en_US/aam/merge-rule-definitions.html)
>* [Datenquelleneinstellungen und Menüoptionen](https://marketing.adobe.com/resources/help/en_US/aam/datasource-settings-definitions.html)

