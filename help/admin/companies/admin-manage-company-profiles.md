---
description: Verwenden Sie die Seite "Unternehmen"im Audience Manager-Admin-Tool, um ein neues Unternehmen zu erstellen.
seo-description: Verwenden Sie die Seite "Unternehmen"im Audience Manager-Admin-Tool, um ein neues Unternehmen zu erstellen.
seo-title: Erstellen eines Firmenprofils
title: Erstellen eines Firmenprofils
uuid: 55de18f8-883d-43fe-b37f-e8805bb92f7a
exl-id: 80bb8a89-0207-4645-ac42-e73cd10561de
source-git-commit: f5d74995f0664cf63e68b46f1f3c608f34df0e80
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 5%

---

# Erstellen eines Firmenprofils {#create-a-company-profile}

Verwenden Sie die Seite [!UICONTROL Companies] im Audience Manager Admin-Tool, um ein neues Unternehmen zu erstellen.

<!-- t_create_company.xml -->

>[!NOTE]
>
>Sie müssen über die Rolle **[!UICONTROL DEXADMIN]** verfügen, um neue Unternehmen erstellen zu können.

1. Klicken **[!UICONTROL Companies]** > **[!UICONTROL Add Company]**.
1. Füllen Sie die Felder aus:

   * **[!UICONTROL Name]**: (Erforderlich) Geben Sie den Namen des Unternehmens an.
   * **[!UICONTROL Description]**: (Erforderlich) Geben Sie beschreibende Informationen über das Unternehmen an, z. B. die Branche oder seinen vollständigen Namen.
   * **[!UICONTROL Subdomain]**: (Erforderlich) Geben Sie die Subdomäne des Unternehmens an. Der Text, den Sie eingeben, wird als Subdomäne des Ereignisaufrufs angezeigt. Das kann nicht geändert werden. Es muss sich um eine Zeichenfolge von [!DNL URL]-gültigen Zeichen handeln.

      Wenn Ihr Unternehmen beispielsweise [!DNL AcmeCorp] heißt, lautet die Subdomäne [!DNL acmecorp].

      Audience Manager verwendet die Subdomäne für [!UICONTROL Data Collection Server] (DCS). Wenn im vorherigen Beispiel [!DNL URL] in [!UICONTROL DCS] vollständig von Ihrem Unternehmen ist, wäre [!DNL acmecorp.demdex.net].

   * **[!UICONTROL Lifecyle]**: Geben Sie die gewünschte Phase für das Unternehmen an:
      * **[!UICONTROL Active]**: Geben Sie an, dass das Unternehmen ein aktiver Audience Manager-Client sein wird. Ein [!UICONTROL Active]-Konto bedeutet einen zahlenden Kunden, nicht nur für die Beratung, sondern für die Audience Manager-SKU.
      * **[!UICONTROL Demo]**: Geben Sie an, dass das Unternehmen nur zu Demozwecken dient. Berichtsdaten werden automatisch gefälscht.
      * **[!UICONTROL Prospect]**: Geben Sie an, dass es sich bei dem Unternehmen um einen potenziellen Audience Manager-Client handelt, z. B. wenn einem Unternehmen eine kostenlose Kontoeinrichtung  [!DNL POC] oder eine Kontoeinrichtung für eine Verkaufsdemo zugewiesen wird.
      * **[!UICONTROL Test]**: Geben Sie an, dass das Unternehmen nur zu internen Testzwecken dient.
   * **[!UICONTROL Account Types]**: Geben Sie die vollständigen Kontotypen für dieses Unternehmen an. Kein Kontotyp schließt sich bei anderen Typen gegenseitig aus.
      * **[!UICONTROL Full AAM]**: Geben Sie an, dass das Unternehmen über ein vollständiges Adobe Audience Manager-Konto verfügt und die Benutzer Zugriff auf die Anmeldung haben.
      * **[!UICONTROL MMP]**: Geben Sie an, dass das Unternehmen für die Verwendung der  [!UICONTROL Master Marketing Profile] ([!UICONTROL MMP])-Funktionen aktiviert wurde. Der [!UICONTROL MMP] ermöglicht die Freigabe von Zielgruppen über das Experience Cloud mithilfe eines [!UICONTROL Experience Cloud ID] ([!DNL MCID]) , das jedem Besucher zugewiesen und dann vom Audience Manager verwendet wird. Wenn Sie diesen Kontotyp auswählen, wird auch [!UICONTROL Experience Cloud ID Service] automatisch ausgewählt.

         Weitere Informationen finden Sie unter [Zielgruppendienste - Übergeordnetes Marketingprofil](https://marketing.adobe.com/resources/help/en_US/mcloud/audience_library.html).
   * **[!UICONTROL Data Source]**: Geben Sie an, dass das Unternehmen ein Drittanbieter von Daten in Audience Manager ist.
   * **[!UICONTROL Targeting Partner]**: Geben Sie an, dass das Unternehmen als Targeting-Plattform für Audience Manager fungiert.
   * **[!UICONTROL Visitor ID Service]**: Geben Sie an, dass das Unternehmen für die Verwendung der  [!UICONTROL Experience Cloud Visitor ID Service]aktiviert wurde.

      [!UICONTROL Experience Cloud Visitor ID Service] stellt eine universelle Besucher-ID für alle Experience Cloud-Lösungen bereit. Weitere Informationen finden Sie im Benutzerhandbuch zum Experience Cloud-Besucher-ID-Dienst](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-overview.html).[

   * **[!UICONTROL Agency]**: Geben Sie an, dass das Unternehmen über ein  [!UICONTROL Agency] Konto verfügen soll.



1. Klicken **[!UICONTROL Create]**. Fahren Sie mit den Anweisungen unter [Ein Firmenprofil bearbeiten](../companies/admin-manage-company-profiles.md#edit-company-profile) fort.

   ![Schrittergebnis](assets/add_company.png)

## Bearbeiten von Firmenprofilen {#edit-company-profile}

Bearbeiten Sie das Profil eines Unternehmens, einschließlich Name, Beschreibung, Subdomäne, Lebenszyklus und mehr.

<!-- t_edit_company_profile.xml -->

1. Klicken Sie auf **[!UICONTROL Companies]**, suchen Sie das gewünschte Unternehmen und klicken Sie auf das gewünschte Unternehmen, um dessen Seite [!UICONTROL Profile] anzuzeigen.

   Verwenden Sie das Feld [!UICONTROL Search] oder die Paginierungssteuerelemente am unteren Rand der Liste, um das gewünschte Unternehmen zu finden. Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.

   ![Schrittergebnis](assets/profile_company.png)

1. Bearbeiten Sie die Felder je nach Bedarf:

   * **[!UICONTROL Name]**: Bearbeiten Sie den Namen des Unternehmens. Dies ist ein erforderliches Feld.
   * **[!UICONTROL Description]**: Bearbeiten Sie die Beschreibung des Unternehmens. Dies ist ein erforderliches Feld.
   * **[!UICONTROL Subdomain]**: (Erforderlich) Geben Sie die Subdomäne des Unternehmens an. Der Text, den Sie eingeben, wird als Subdomäne des Ereignisaufrufs angezeigt. Das kann nicht geändert werden. Es muss sich um eine Zeichenfolge von [!DNL URL]-gültigen Zeichen handeln.

      Wenn Ihr Unternehmen beispielsweise [!DNL AcmeCorp] heißt, lautet die Subdomäne [!DNL acmecorp].

      Audience Manager verwendet die Subdomäne für [!UICONTROL Data Collection Server] (DCS). Wenn im vorherigen Beispiel [!DNL URL] in [!UICONTROL DCS] vollständig von Ihrem Unternehmen ist, wäre [!DNL acmecorp.demdex.net].

   * **[!UICONTROL imsOrgld]**: ([!UICONTROL Identity Management System Organization ID]) Mit dieser Kennung können Sie Ihr Unternehmen mit der Adobe Experience Cloud verbinden.
   * **[!UICONTROL Lifecyle]**: Geben Sie die gewünschte Phase für das Unternehmen an:
      * **[!UICONTROL Active]**: Geben Sie an, dass das Unternehmen ein aktiver Audience Manager-Client sein wird. Ein aktives Konto bedeutet einen zahlenden Kunden, nicht nur für Beratung, sondern für die Audience Manager-SKU.
      * **[!UICONTROL Demo]**: Geben Sie an, dass das Unternehmen nur zu Demozwecken dient. Berichtsdaten werden automatisch gefälscht.
      * **[!UICONTROL Prospect]**: Geben Sie an, dass es sich bei dem Unternehmen um einen potenziellen Audience Manager-Client handelt, z. B. wenn einem Unternehmen eine kostenlose Kontoeinrichtung  [!DNL POC] oder eine Kontoeinrichtung für eine Verkaufsdemo zugewiesen wird.
      * **[!UICONTROL Test]**: Geben Sie an, dass das Unternehmen nur zu internen Testzwecken dient.
   * **[!UICONTROL Account Types]**: Geben Sie die vollständigen Kontotypen für dieses Unternehmen an. Kein Kontotyp schließt sich bei anderen Typen gegenseitig aus.
      * **[!UICONTROL Full AAM]**: Geben Sie an, dass das Unternehmen über ein vollständiges Adobe Audience Manager-Konto verfügt und die Benutzer Zugriff auf die Anmeldung haben.
      * **[!UICONTROL MMP]**: Geben Sie an, dass das Unternehmen für die Verwendung der Funktionen des Übergeordneten Marketing-Profils ([!UICONTROL MMP]) aktiviert wurde.

         Wenn Sie diesen Kontotyp auswählen, wird auch **[!UICONTROL Visitor ID Service]** automatisch ausgewählt.
Weitere Informationen finden Sie unter [Zielgruppendienste - Übergeordnetes Marketingprofil](https://marketing.adobe.com/resources/help/en_US/mcloud/audience_library.html).
   * **[!UICONTROL Data Source]**: Geben Sie an, dass das Unternehmen ein Drittanbieter von Daten in Audience Manager ist.
   * **[!UICONTROL Targeting Partner]**: Geben Sie an, dass das Unternehmen als Targeting-Plattform für Audience Manager fungiert.
   * **[!UICONTROL Visitor ID Service]**: Geben Sie an, dass das Unternehmen für die Verwendung des Experience Cloud-Besucher-ID-Diensts aktiviert wurde.

      Der Experience Cloud-Besucher-ID-Dienst stellt eine universale Besucher-ID für alle Experience Cloud-Lösungen bereit. Weitere Informationen finden Sie im Benutzerhandbuch zum Experience Cloud-Besucher-ID-Dienst](https://microsite.omniture.com/t2/help/en_US/mcvid/mcvid_service.html).[

   * **[!UICONTROL Agency]**: Geben Sie an, dass das Unternehmen über ein Agenturkonto verfügen wird.
   * **[!UICONTROL Features]**: Wählen Sie die gewünschten Optionen aus:
      * **[!UICONTROL Password Expiration]**: Legt fest, dass alle Benutzerkennwörter in diesem Unternehmen nach 90 Tagen ablaufen, um die Sicherheit der Audience Manager zu erhöhen.
      * **[!UICONTROL Reporting]**: Ermöglicht die Berichterstellung der Audience Manager für dieses Unternehmen.
      * **[!UICONTROL Role Based Access Controls]**: Aktivieren Sie rollenbasierte Zugriffskontrollen für dieses Unternehmen. Mit rollenbasierten Zugriffssteuerungen können Sie Benutzergruppen mit unterschiedlichen Zugriffsberechtigungen erstellen. Einzelanwender innerhalb dieser Gruppen können dann nur auf bestimmte Funktionen in Audience Manager zugreifen.


1. Klicken **[!UICONTROL Submit Updates]**.

## Löschen eines Firmenprofils {#delete-company-profile}

Verwenden Sie die Seite [!UICONTROL Companies] im Tool Audience Manager [!UICONTROL Admin], um ein bestehendes Unternehmen zu löschen.

<!-- t_delete_company.xml -->

>[!NOTE]
>
>Sie müssen über die Rolle [!UICONTROL DEXADMIN] verfügen, um vorhandene Unternehmen zu löschen.

1. Um ein vorhandenes Unternehmen zu löschen, klicken Sie auf **[!UICONTROL Companies]**.

   ![Schrittergebnis](assets/companies.png)

1. Klicken Sie in der Spalte **[!UICONTROL Actions]** des gewünschten Unternehmens auf ![](assets/icon_delete.png) .
1. Klicken Sie auf **[!UICONTROL OK]**, um den Löschvorgang zu bestätigen.
