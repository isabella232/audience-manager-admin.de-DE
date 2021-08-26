---
description: Die Gerätediagrammoptionen stehen Unternehmen zur Verfügung, die an der Adobe Experience Cloud-Gerätekooperation teilnehmen. Wenn ein Kunde auch eine Vertragsbeziehung mit einem Gerätediagramm-Drittanbieter unterhält, der in Audience Manager integriert ist, werden in diesem Abschnitt Optionen für dieses Gerätediagramm angezeigt. Diese Optionen finden Sie unter Unternehmen > Firmenname > Profil > Gerätediagrammoptionen.
seo-description: The Device Graph Options are available to companies that participate in the Adobe Experience Cloud Device Co-op. If a customer also has a contractual relationship with a third-party device graph provider that is integrated with Audience Manager, this section will show options for that device graph. These options are located in Companies > company name > Profile > Device Graph Options.
seo-title: Device Graph Options for Companies
title: Gerätediagrammoptionen für Firmen
uuid: a8ced843-710c-4a8f-a0d7-ea89d010a7a5
exl-id: 2502f3d2-b43c-410c-acb6-03c2a2ba2c1d
source-git-commit: 1f4dbf8f7b36e64c3015b98ef90b6726d0e7495a
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 3%

---

# Gerätediagrammoptionen für Firmen {#device-graph-options-for-companies}

Die [!UICONTROL Device Graph Options] stehen Unternehmen zur Verfügung, die am [!DNL Adobe Experience Cloud Device Co-op] teilnehmen. Wenn ein Kunde auch eine Vertragsbeziehung mit einem Gerätediagramm-Drittanbieter unterhält, der in Audience Manager integriert ist, werden in diesem Abschnitt Optionen für dieses Gerätediagramm angezeigt. Diese Optionen befinden sich unter [!UICONTROL Companies] > Firmenname > [!UICONTROL Profile] > [!UICONTROL Device Graph Options].

![](assets/adminUIdataSource.png)

In dieser Abbildung werden allgemeine Namen für die Gerätediagrammoptionen von Drittanbietern verwendet. In der Produktion stammen diese Namen vom Gerätediagramm-Provider und können von dem hier gezeigten variieren. Beispielsweise sind die [!DNL LiveRamp]-Optionen in der Regel (aber nicht immer):

* Mit &quot;[!DNL LiveRamp]&quot;
* Enthält einen Vornamen, der variiert
* Ende mit &quot;[!UICONTROL - Household]&quot;oder &quot;[!UICONTROL -Person]&quot;

## Definierte Gerätediagrammoptionen {#device-graph-options-defined}

Die hier ausgewählten Gerätediagrammoptionen zeigen [!UICONTROL Device Options] den [!DNL Audience Manager]-Kunden verfügbare Optionen an oder blenden sie aus, wenn sie eine [!UICONTROL Profile Merge Rule] erstellen.

### Co-op-Gerätediagramm {#co-op-graph}

Kunden, die an der [Adobe Experience Cloud Device Co-op](https://experienceleague.adobe.com/docs/device-co-op/using/about/overview.html?lang=en) teilnehmen, verwenden diese Optionen, um eine [!UICONTROL Profile Merge Rule] mit [deterministischen und probabilistischen Daten](https://experienceleague.adobe.com/docs/device-co-op/using/device-graph/links.html?lang=en) zu erstellen. Der [!DNL Corporate Provisioning Team] aktiviert und deaktiviert diese Option über einen Back-End-Aufruf [!DNL API]. Sie können diese Felder im [!DNL Admin UI] nicht aktivieren oder löschen. Außerdem schließen sich die Optionen **[!UICONTROL Co-op Device Graph]** und **[!UICONTROL Company Device Graph]** gegenseitig aus. Kunden können uns bitten, das eine oder das andere zu aktivieren, aber nicht beides. Wenn diese Option aktiviert ist, wird das **[!UICONTROL Co-op Device Graph]**-Steuerelement in den [!UICONTROL Device Options]-Einstellungen für [!UICONTROL Profile Merge Rule] verfügbar gemacht.

![](assets/adminUI1.png)

### Gerätediagramm für Unternehmen {#company-graph}

Diese Option richtet sich an [!DNL Analytics] -Kunden, die die Metrik [!UICONTROL People] in ihrer Report Suite [!DNL Analytics] verwenden. Der [!DNL Corporate Provisioning Team] aktiviert und deaktiviert diese Option über einen Back-End-Aufruf [!DNL API]. Sie können diese Felder im [!DNL Admin UI] nicht aktivieren oder löschen. Außerdem schließen sich die Optionen **[!UICONTROL Company Device Graph]** und **[!UICONTROL Co-op Device Graph]** gegenseitig aus. Kunden können uns bitten, das eine oder das andere zu aktivieren, aber nicht beides. Wenn aktiviert:

* Dieses Gerätediagramm verwendet deterministische Daten, die zu dem Unternehmen gehören, das Sie konfigurieren (keine probabilistischen Daten).
* [!DNL Audience Manager] erstellt automatisch einen  [!UICONTROL Data Source] benannten  `*`Partnernamen`*-Company Device Graph-Person`. Auf der Detailseite [!UICONTROL Data Source] können [!DNL Audience Manager] Kunden den Partnernamen und die Beschreibung ändern und [Datenexportkontrollen](https://experienceleague.adobe.com/docs/device-co-op/using/device-graph/links.html?lang=en) auf diese Datenquelle anwenden.
* [!DNL Audience Manager] -Kunden  *sehen* keine neue Einstellung im  [!UICONTROL Device Options] Abschnitt für  [!UICONTROL Profile Merge Rule].

### LiveRamp-Gerätediagramm (Person oder Haushalt) {#liveramp-device-graph}

Diese Kontrollkästchen sind in [!DNL Admin UI] aktiviert, wenn ein Partner ein [!UICONTROL Data Source] erstellt und **[!UICONTROL Use as an Authenticated Profile]** und/oder **[!UICONTROL Use as a Device Graph]** auswählt. Die Namen für diese Einstellungen werden vom Gerätediagramm-Anbieter eines Drittanbieters (z. B. [!DNL LiveRamp], [!DNL TapAd] usw.) bestimmt. Wenn diese Option aktiviert ist, bedeutet dies, dass das Unternehmen, das Sie konfigurieren, die von diesen Gerätediagrammen bereitgestellten Daten verwenden wird.

![](assets/adminUI2.png)

>[!MORELIKETHIS]
>
>* [Für Profilzusammenführungsrichtlinien definierte Optionen](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/profile-merge-rules/merge-rule-definitions.html?lang=en)
>* [Datenquelleneinstellungen und Menüoptionen](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-sources/datasources-list-and-settings.html?lang=en)

