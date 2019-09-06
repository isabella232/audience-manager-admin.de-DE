---
description: Verwenden Sie die Seite "Unternehmen" im Audience Manager-Verwaltungswerkzeug, um ein neues Unternehmen zu erstellen.
seo-description: Verwenden Sie die Seite "Unternehmen" im Audience Manager-Verwaltungswerkzeug, um ein neues Unternehmen zu erstellen.
seo-title: Erstellen eines Unternehmensprofils
title: Erstellen eines Unternehmensprofils
uuid: 55 de 18 f 8-883 d -43 fe-b 37 f-e 8805 bb 92 f 7 a
translation-type: tm+mt
source-git-commit: 71bf4cec222428686c1eab0998f66887db06da68

---


# Erstellen eines Unternehmensprofils {#create-a-company-profile}

Verwenden Sie die [!UICONTROL Companies] Seite im Audience Manager-Verwaltungswerkzeug, um ein neues Unternehmen zu erstellen.

<!-- t_create_company.xml -->

>[!NOTE]
>
>Sie müssen über die **[!UICONTROL DEXADMIN]** Rolle verfügen, um neue Unternehmen zu erstellen.

1. Click **[!UICONTROL Companies]** &gt; **[!UICONTROL Add Company]**.
1. Füllen Sie die Felder aus:

   * **[!UICONTROL Name]**: (Erforderlich) Geben Sie den Namen des Unternehmens an.
   * **[!UICONTROL Description]**: (Erforderlich) Geben Sie beschreibende Informationen über das Unternehmen an, z. B. Branche oder seinen vollständigen Namen.
   * **[!UICONTROL Subdomain]**: (Erforderlich) Geben Sie die Subdomäne des Unternehmens an. Der eingegebene Text wird als Subdomäne des Ereignisaufrufs angezeigt. Dies kann nicht geändert werden. Es muss eine Zeichenfolge aus [!DNL URL]-gültigen Zeichen sein.

      Wenn Ihr Unternehmen beispielsweise benannt [!DNL AcmeCorp]wurde, lautet [!DNL acmecorp]die Subdomäne.

      Audience Manager verwendet die Subdomäne für das [!UICONTROL Data Collection Server]([!UICONTROL DCS]). Im vorherigen Beispiel, wenn Ihr Unternehmen [!DNL URL][!UICONTROL DCS][!DNL acmecorp.demdex.net]in der Vergangenheit ist.

   * **[!UICONTROL Lifecyle]**: Geben Sie die gewünschte Stufe für das Unternehmen an:
      * **[!UICONTROL Active]**: Geben Sie an, dass das Unternehmen ein aktiver Audience Manager-Client sein soll. Ein [!UICONTROL Active] Konto bedeutet einen zahlenden Kunden, nicht nur für Beratung, sondern für die Zielgruppen-Manager-SKU.
      * **[!UICONTROL Demo]**: Legen Sie fest, dass das Unternehmen nur zu Demozwecken dient. Berichtsdaten werden automatisch verfälscht.
      * **[!UICONTROL Prospect]**: Geben Sie an, dass das Unternehmen ein Audience Manager-Client ist, z. B. ein Unternehmen, das kostenlos [!DNL POC] oder ein Konto für eine Demo-Demo eingerichtet wird.
      * **[!UICONTROL Test]**: Geben Sie an, dass das Unternehmen nur internen Testzwecken dient.
   * **[!UICONTROL Account Types]**: Geben Sie den vollständigen Satz an Kontotypen für dieses Unternehmen an. Keine Kontotypen schließen sich gegenseitig aus.
      * **[!UICONTROL Full AAM]**: Geben Sie an, dass das Unternehmen über ein vollständiges Adobe Audience Manager-Konto verfügt und Benutzer über die Anmeldung verfügen.
      * **[!UICONTROL MMP]**: Geben Sie an, dass das Unternehmen für die Verwendung der Funktion [!UICONTROL Master Marketing Profile] ([!UICONTROL MMP]) aktiviert wurde. Die Funktion [!UICONTROL MMP] ermöglicht das Freigeben von Zielgruppen über die Experience Cloud mit einem [!UICONTROL Experience Cloud ID] ([!DNL MCID]), das jedem Besucher zugewiesen und dann von Audience Manager verwendet wird. Wenn Sie diesen Kontotyp auswählen, wird ebenfalls automatisch ausgewählt [!UICONTROL Experience Cloud ID Service] .

         Weitere Informationen finden Sie unter [Audiences Services - Master-Marketing-Profil](https://marketing.adobe.com/resources/help/en_US/mcloud/audience_library.html).
   * **[!UICONTROL Data Source]**: Geben Sie an, dass das Unternehmen ein Drittanbieter-Datenprovider in Audience Manager ist.
   * **[!UICONTROL Targeting Partner]**: Geben Sie an, dass das Unternehmen als Targeting-Plattform für Audience Manager-Kunden fungiert.
   * **[!UICONTROL Visitor ID Service]**: Geben Sie an, dass das Unternehmen aktiviert [!UICONTROL Experience Cloud Visitor ID Service]wurde.

      Die Bereitstellung [!UICONTROL Experience Cloud Visitor ID Service] stellt eine universale Besucher-ID für die Experience Cloud-Lösungen bereit. For more information, see the [Experience Cloud Visitor ID Service user guide](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-overview.html).

   * **[!UICONTROL Agency]**: Geben Sie an, dass das Unternehmen über ein [!UICONTROL Agency] Konto verfügt.



1. Klicken Sie auf **[!UICONTROL Create]**. Fahren Sie mit den Anweisungen unter [Unternehmensprofil bearbeiten fort](../companies/admin-manage-company-profiles.md#edit-company-profile).

   ![Schrittergebnis](assets/add_company.png)

## Bearbeiten eines Unternehmensprofils {#edit-company-profile}

Bearbeiten Sie das Profil eines Unternehmens, einschließlich Name, Beschreibung, Subdomäne, Lebenszyklus und mehr.

<!-- t_edit_company_profile.xml -->

1. Klicken **[!UICONTROL Companies]** Sie auf und suchen Sie dann das gewünschte Unternehmen, um dessen [!UICONTROL Profile] Seite anzuzeigen.

   Verwenden Sie das [!UICONTROL Search] Feld oder die Seitenumbruchsteuerelemente unten in der Liste, um das gewünschte Unternehmen zu finden. Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.

   ![Schrittergebnis](assets/profile_company.png)

1. Bearbeiten Sie die Felder je nach Bedarf:

   * **[!UICONTROL Name]**: Bearbeiten Sie den Namen des Unternehmens. Dies ist ein erforderliches Feld.
   * **[!UICONTROL Description]**: Bearbeiten Sie die Beschreibung des Unternehmens. Dies ist ein erforderliches Feld.
   * **[!UICONTROL Subdomain]**: (Erforderlich) Geben Sie die Subdomäne des Unternehmens an. Der eingegebene Text wird als Subdomäne des Ereignisaufrufs angezeigt. Dies kann nicht geändert werden. Es muss eine Zeichenfolge aus [!DNL URL]-gültigen Zeichen sein.

      Wenn Ihr Unternehmen beispielsweise benannt [!DNL AcmeCorp]wurde, lautet [!DNL acmecorp]die Subdomäne.

      Audience Manager verwendet die Subdomäne für das [!UICONTROL Data Collection Server] ([!UICONTROL DCS]). Im vorherigen Beispiel, wenn Ihr Unternehmen [!DNL URL][!UICONTROL DCS][!DNL acmecorp.demdex.net]in der Vergangenheit ist.

   * **[!UICONTROL imsOrgld]**: ([!UICONTROL Identity Management System Organization ID]) Mit dieser ID können Sie Ihr Unternehmen mit der Adobe Experience Cloud verbinden.
   * **[!UICONTROL Lifecyle]**: Geben Sie die gewünschte Stufe für das Unternehmen an:
      * **[!UICONTROL Active]**: Geben Sie an, dass das Unternehmen ein aktiver Audience Manager-Client sein soll. Ein aktives Konto bedeutet einen zahlenden Kunden, nicht nur für Beratung, sondern für die Zielgruppen-Manager-SKU.
      * **[!UICONTROL Demo]**: Legen Sie fest, dass das Unternehmen nur zu Demozwecken dient. Berichtsdaten werden automatisch verfälscht.
      * **[!UICONTROL Prospect]**: Geben Sie an, dass das Unternehmen ein Audience Manager-Client ist, z. B. ein Unternehmen, das kostenlos [!DNL POC] oder ein Konto für eine Demo-Demo eingerichtet wird.
      * **[!UICONTROL Test]**: Geben Sie an, dass das Unternehmen nur internen Testzwecken dient.
   * **[!UICONTROL Account Types]**: Geben Sie den vollständigen Satz an Kontotypen für dieses Unternehmen an. Keine Kontotypen schließen sich gegenseitig aus.
      * **[!UICONTROL Full AAM]**: Geben Sie an, dass das Unternehmen über ein vollständiges Adobe Audience Manager-Konto verfügt und Benutzer über die Anmeldung verfügen.
      * **[!UICONTROL MMP]**: Geben Sie an, dass das Unternehmen für die Verwendung der Master-Marketing-Profil ([!UICONTROL MMP])-Funktionen aktiviert wurde.

         Wenn Sie diesen Kontotyp auswählen, **[!UICONTROL Visitor ID Service]** wird ebenfalls automatisch ausgewählt.
Weitere Informationen finden Sie unter [Audiences Services - Master-Marketing-Profil](https://marketing.adobe.com/resources/help/en_US/mcloud/audience_library.html).
   * **[!UICONTROL Data Source]**: Geben Sie an, dass das Unternehmen ein Drittanbieter-Datenprovider in Audience Manager ist.
   * **[!UICONTROL Targeting Partner]**: Geben Sie an, dass das Unternehmen als Targeting-Plattform für Audience Manager-Kunden fungiert.
   * **[!UICONTROL Visitor ID Service]**: Geben Sie an, dass das Unternehmen für die Verwendung des Experience Cloud Besucher-ID-Service aktiviert wurde.

      Der Experience Cloud-Besucher-ID-Dienst stellt eine universale Besucher-ID für alle Experience Cloud-Lösungen bereit. For more information, see the [Experience Cloud Visitor ID Service user guide](https://microsite.omniture.com/t2/help/en_US/mcvid/mcvid_service.html).

   * **[!UICONTROL Agency]**: Geben Sie an, dass das Unternehmen über ein Agenturkonto verfügt.
   * **[!UICONTROL Features]**: Wählen Sie die gewünschten Optionen aus:
      * **[!UICONTROL Password Expiration]**: Legt alle Benutzerkennwörter innerhalb dieses Unternehmens nach 90 Tagen ab, um die Sicherheit von Audience Manager zu erhöhen.
      * **[!UICONTROL Reporting]**: Aktiviert die Audience Manager-Berichterstellung für dieses Unternehmen.
      * **[!UICONTROL Role Based Access Controls]**: Aktivieren Sie rollenbasierte Zugriffssteuerungsmöglichkeiten für dieses Unternehmen. Mit rollenbasierten Zugriffssteuerungselementen können Sie Benutzergruppen mit unterschiedlichen Zugriffsrechten erstellen. Einzelne Benutzer innerhalb dieser Gruppen können dann nur auf bestimmte Funktionen in Audience Manager zugreifen.


1. Klicken Sie auf **[!UICONTROL Submit Updates]**.

## Ein Unternehmensprofil löschen {#delete-company-profile}

Verwenden Sie die [!UICONTROL Companies] Seite im Audience Manager [!UICONTROL Admin] -Tool, um ein vorhandenes Unternehmen zu löschen.

<!-- t_delete_company.xml -->

>[!NOTE]
>
>Sie müssen über die [!UICONTROL DEXADMIN] Rolle verfügen, um bestehende Unternehmen zu löschen.

1. Klicken **[!UICONTROL Companies]** Sie auf, um ein vorhandenes Unternehmen zu löschen.

   ![Schrittergebnis](assets/companies.png)

1. Klicken ![](assets/icon_delete.png) Sie in die **[!UICONTROL Actions]** Spalte des gewünschten Unternehmens.
1. Klicken Sie auf **[!UICONTROL OK], um den Löschvorgang zu bestätigen.**
