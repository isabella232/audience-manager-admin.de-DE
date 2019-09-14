---
description: Verwenden Sie die Seite "Unternehmen"im Audience Manager Admin-Tool, um ein neues Unternehmen zu erstellen.
seo-description: Verwenden Sie die Seite "Unternehmen"im Audience Manager Admin-Tool, um ein neues Unternehmen zu erstellen.
seo-title: Unternehmensprofil erstellen
title: Unternehmensprofil erstellen
uuid: 55de18f8-883d-43fe-b37f-e8805bb92f7a
translation-type: tm+mt
source-git-commit: 71bf4cec222428686c1eab0998f66887db06da68

---


# Unternehmensprofil erstellen {#create-a-company-profile}

Verwenden Sie die [!UICONTROL Companies] Seite im Audience Manager Admin-Tool, um ein neues Unternehmen zu erstellen.

<!-- t_create_company.xml -->

>[!NOTE]
>
>Sie müssen die **[!UICONTROL DEXADMIN]** Rolle haben, um neue Unternehmen zu gründen.

1. Click **[!UICONTROL Companies]** &gt; **[!UICONTROL Add Company]**.
1. Füllen Sie die Felder aus:

   * **[!UICONTROL Name]**: (Erforderlich) Geben Sie den Namen des Unternehmens an.
   * **[!UICONTROL Description]**: (Erforderlich) Geben Sie beschreibende Informationen über das Unternehmen an, z. B. die Branche oder den vollständigen Namen.
   * **[!UICONTROL Subdomain]**: (Erforderlich) Geben Sie die Subdomäne des Unternehmens an. Der von Ihnen eingegebene Text wird als Subdomäne des Ereignisaufrufs angezeigt. Das kann man nicht ändern. Es muss sich um eine Zeichenfolge mit [!DNL URL]gültigen Zeichen handeln.

      Wenn Ihr Unternehmen z. B. benannt wurde [!DNL AcmeCorp], wäre die Subdomäne [!DNL acmecorp].

      Audience Manager verwendet die Subdomäne für [!UICONTROL Data Collection Server]([!UICONTROL DCS]). Im vorherigen Beispiel wäre es, wenn Ihr Unternehmen voll [!DNL URL] in [!UICONTROL DCS] wäre [!DNL acmecorp.demdex.net].

   * **[!UICONTROL Lifecyle]**: Geben Sie die gewünschte Phase für das Unternehmen an:
      * **[!UICONTROL Active]**: Geben Sie an, dass das Unternehmen ein aktiver Audience Manager-Client sein soll. Ein [!UICONTROL Active] Konto bedeutet einen zahlenden Kunden, nicht nur für Beratung, sondern auch für die Audience Manager-SKU.
      * **[!UICONTROL Demo]**: Geben Sie an, dass das Unternehmen nur zu Demozwecken dient. Berichtsdaten werden automatisch gefälscht.
      * **[!UICONTROL Prospect]**: Geben Sie an, dass es sich bei dem Unternehmen um einen potenziellen Audience Manager-Client handelt, z. B. um ein Unternehmen, das für eine Verkaufsdemo eine kostenlose [!DNL POC] Kontoeinrichtung erhält.
      * **[!UICONTROL Test]**: Geben Sie an, dass das Unternehmen nur für interne Testzwecke verwendet wird.
   * **[!UICONTROL Account Types]**: Geben Sie den vollständigen Satz an Kontotypen für dieses Unternehmen an. Kein Kontotyp schließt sich gegenseitig mit anderen Typen aus.
      * **[!UICONTROL Full AAM]**: Geben Sie an, dass das Unternehmen über ein vollständiges Adobe Audience Manager-Konto verfügt und die Benutzer Zugriff auf die Anmeldung haben.
      * **[!UICONTROL MMP]**: Geben Sie an, dass das Unternehmen die [!UICONTROL Master Marketing Profile] ([!UICONTROL MMP]) Funktionen verwenden darf. Auf diese Weise [!UICONTROL MMP] können Zielgruppen über die Experience Cloud gemeinsam genutzt werden. Dazu wird ein [!UICONTROL Experience Cloud ID] ([!DNL MCID]) verwendet, der jedem Besucher zugewiesen und dann von Audience Manager verwendet wird. Wenn Sie diesen Kontotyp auswählen, [!UICONTROL Experience Cloud ID Service] wird auch die Option automatisch ausgewählt.

         Weitere Informationen finden Sie unter [Audiences Services - Master-Marketing-Profil](https://marketing.adobe.com/resources/help/en_US/mcloud/audience_library.html).
   * **[!UICONTROL Data Source]**: Geben Sie an, dass das Unternehmen ein Drittanbieter für Daten in Audience Manager ist.
   * **[!UICONTROL Targeting Partner]**: Geben Sie an, dass das Unternehmen als Targeting-Plattform für Audience Manager-Kunden fungiert.
   * **[!UICONTROL Visitor ID Service]**: Geben Sie an, dass das Unternehmen für die Verwendung der Variablen [!UICONTROL Experience Cloud Visitor ID Service]aktiviert wurde.

      Die [!UICONTROL Experience Cloud Visitor ID Service] stellt eine universelle Besucher-ID für alle Experience Cloud-Lösungen bereit. For more information, see the [Experience Cloud Visitor ID Service user guide](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-overview.html).

   * **[!UICONTROL Agency]**: Geben Sie an, dass das Unternehmen über ein [!UICONTROL Agency] Konto verfügt.



1. Klicken Sie auf **[!UICONTROL Create]**. Fahren Sie mit den Anweisungen unter Unternehmensprofil [bearbeiten](../companies/admin-manage-company-profiles.md#edit-company-profile)fort.

   ![Schritt-Ergebnis](assets/add_company.png)

## Unternehmensprofil bearbeiten {#edit-company-profile}

Bearbeiten Sie das Profil eines Unternehmens, einschließlich Name, Beschreibung, Subdomäne, Lebenszyklus und mehr.

<!-- t_edit_company_profile.xml -->

1. Klicken Sie auf **[!UICONTROL Companies]**, suchen Sie das gewünschte Unternehmen und klicken Sie darauf, um die zugehörige [!UICONTROL Profile] Seite anzuzeigen.

   Verwenden Sie das [!UICONTROL Search] Feld oder die Paginierungssteuerelemente unten in der Liste, um das gewünschte Unternehmen zu finden. Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.

   ![Schritt-Ergebnis](assets/profile_company.png)

1. Bearbeiten Sie die Felder je nach Bedarf:

   * **[!UICONTROL Name]**: Bearbeiten Sie den Namen des Unternehmens. Dies ist ein erforderliches Feld.
   * **[!UICONTROL Description]**: Bearbeiten Sie die Beschreibung des Unternehmens. Dies ist ein erforderliches Feld.
   * **[!UICONTROL Subdomain]**: (Erforderlich) Geben Sie die Subdomäne des Unternehmens an. Der von Ihnen eingegebene Text wird als Subdomäne des Ereignisaufrufs angezeigt. Das kann man nicht ändern. Es muss sich um eine Zeichenfolge mit [!DNL URL]gültigen Zeichen handeln.

      Wenn Ihr Unternehmen z. B. benannt wurde [!DNL AcmeCorp], wäre die Subdomäne [!DNL acmecorp].

      Audience Manager verwendet die Subdomäne für [!UICONTROL Data Collection Server] ([!UICONTROL DCS]). Im vorherigen Beispiel wäre es, wenn Ihr Unternehmen voll [!DNL URL] in [!UICONTROL DCS] wäre [!DNL acmecorp.demdex.net].

   * **[!UICONTROL imsOrgld]**: ([!UICONTROL Identity Management System Organization ID]) Mit dieser ID können Sie Ihr Unternehmen mit der Adobe Experience Cloud verbinden.
   * **[!UICONTROL Lifecyle]**: Geben Sie die gewünschte Phase für das Unternehmen an:
      * **[!UICONTROL Active]**: Geben Sie an, dass das Unternehmen ein aktiver Audience Manager-Client sein soll. Ein Aktives Konto bedeutet einen zahlenden Kunden, nicht nur für Beratung, sondern auch für die Audience Manager-SKU.
      * **[!UICONTROL Demo]**: Geben Sie an, dass das Unternehmen nur zu Demozwecken dient. Berichtsdaten werden automatisch gefälscht.
      * **[!UICONTROL Prospect]**: Geben Sie an, dass es sich bei dem Unternehmen um einen potenziellen Audience Manager-Client handelt, z. B. um ein Unternehmen, das für eine Verkaufsdemo eine kostenlose [!DNL POC] Kontoeinrichtung erhält.
      * **[!UICONTROL Test]**: Geben Sie an, dass das Unternehmen nur für interne Testzwecke verwendet wird.
   * **[!UICONTROL Account Types]**: Geben Sie den vollständigen Satz an Kontotypen für dieses Unternehmen an. Kein Kontotyp schließt sich gegenseitig mit anderen Typen aus.
      * **[!UICONTROL Full AAM]**: Geben Sie an, dass das Unternehmen über ein vollständiges Adobe Audience Manager-Konto verfügt und die Benutzer Zugriff auf die Anmeldung haben.
      * **[!UICONTROL MMP]**: Geben Sie an, dass das Unternehmen die Funktionen des Master-Marketing-Profils ([!UICONTROL MMP]) verwenden darf.

         Wenn Sie diesen Kontotyp auswählen, **[!UICONTROL Visitor ID Service]** wird auch automatisch ausgewählt.
Weitere Informationen finden Sie unter [Audiences Services - Master-Marketing-Profil](https://marketing.adobe.com/resources/help/en_US/mcloud/audience_library.html).
   * **[!UICONTROL Data Source]**: Geben Sie an, dass das Unternehmen ein Drittanbieter für Daten in Audience Manager ist.
   * **[!UICONTROL Targeting Partner]**: Geben Sie an, dass das Unternehmen als Targeting-Plattform für Audience Manager-Kunden fungiert.
   * **[!UICONTROL Visitor ID Service]**: Geben Sie an, dass das Unternehmen den Experience Cloud-Besucher-ID-Dienst verwenden darf.

      Der Experience Cloud-Besucher-ID-Dienst stellt eine universale Besucher-ID für alle Experience Cloud-Lösungen bereit. For more information, see the [Experience Cloud Visitor ID Service user guide](https://microsite.omniture.com/t2/help/en_US/mcvid/mcvid_service.html).

   * **[!UICONTROL Agency]**: Geben Sie an, dass das Unternehmen über ein Agenturkonto verfügen soll.
   * **[!UICONTROL Features]**: Wählen Sie die gewünschten Optionen aus:
      * **[!UICONTROL Password Expiration]**: Legt fest, dass alle Benutzerkennwörter in diesem Unternehmen nach 90 Tagen ablaufen, um die Sicherheit von Audience Manager zu erhöhen.
      * **[!UICONTROL Reporting]**: Aktiviert Audience Manager-Berichte für dieses Unternehmen.
      * **[!UICONTROL Role Based Access Controls]**: Aktivieren Sie rollenbasierte Zugriffssteuerung für dieses Unternehmen. Mit rollenbasierten Zugriffssteuerelementen können Sie Benutzergruppen mit unterschiedlichen Zugriffsberechtigungen erstellen. Einzelne Benutzer innerhalb dieser Gruppen können dann nur auf bestimmte Funktionen in Audience Manager zugreifen.


1. Klicken Sie auf **[!UICONTROL Submit Updates]**.

## Unternehmensprofil löschen {#delete-company-profile}

Verwenden Sie die [!UICONTROL Companies] Seite im Audience Manager- [!UICONTROL Admin] Tool, um ein vorhandenes Unternehmen zu löschen.

<!-- t_delete_company.xml -->

>[!NOTE]
>
>Sie müssen die [!UICONTROL DEXADMIN] Rolle haben, um bestehende Unternehmen zu löschen.

1. Klicken Sie zum Löschen eines vorhandenen Unternehmens auf **[!UICONTROL Companies]**.

   ![Schritt-Ergebnis](assets/companies.png)

1. Klicken Sie ![](assets/icon_delete.png) in die **[!UICONTROL Actions]** Spalte des gewünschten Unternehmens.
1. Klicken Sie auf **[!UICONTROL OK], um den Löschvorgang zu bestätigen.**
