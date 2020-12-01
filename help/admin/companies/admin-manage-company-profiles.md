---
description: Verwenden Sie die Seite "Firmen"im Audience Manager-Admin-Tool, um eine neue Firma zu erstellen.
seo-description: Verwenden Sie die Seite "Firmen"im Audience Manager-Admin-Tool, um eine neue Firma zu erstellen.
seo-title: Erstellen eines Firmenprofils
title: Erstellen eines Firmenprofils
uuid: 55de18f8-883d-43fe-b37f-e8805bb92f7a
translation-type: tm+mt
source-git-commit: 69b733ae869b3dded76f0264e395f0157b445148
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 5%

---


# Erstellen eines Firmenprofils {#create-a-company-profile}

Verwenden Sie die Seite [!UICONTROL Companies] im Audience Manager Admin Tool, um eine neue Firma zu erstellen.

<!-- t_create_company.xml -->

>[!NOTE]
>
>Sie müssen über die **[!UICONTROL DEXADMIN]**-Rolle verfügen, um neue Firmen zu erstellen.

1. Klicken **[!UICONTROL Companies]** > **[!UICONTROL Add Company]**.
1. Füllen Sie die Felder aus:

   * **[!UICONTROL Name]**: (Erforderlich) Geben Sie den Namen der Firma an.
   * **[!UICONTROL Description]**: (Erforderlich) Geben Sie beschreibende Informationen über die Firma ein, z. B. die Branche oder den vollständigen Namen.
   * **[!UICONTROL Subdomain]**: (Erforderlich) Geben Sie die Subdomäne der Firma an. Der von Ihnen eingegebene Text wird als Subdomäne des Ereignis-Aufrufs angezeigt. Das kann man nicht ändern. Es muss sich um eine Zeichenfolge von [!DNL URL]-gültigen Zeichen handeln.

      Wenn Ihre Firma beispielsweise [!DNL AcmeCorp] heißt, wäre die Subdomäne [!DNL acmecorp].

      Audience Manager verwendet die Subdomäne für [!UICONTROL Data Collection Server] (DCS). Wenn im vorherigen Beispiel die vollständige [!DNL URL] Ihrer Firma in [!UICONTROL DCS] [!DNL acmecorp.demdex.net] lautet.

   * **[!UICONTROL Lifecyle]**: Geben Sie die gewünschte Phase für die Firma an:
      * **[!UICONTROL Active]**: Geben Sie an, dass die Firma ein aktiver Audience Manager-Client sein soll. Ein [!UICONTROL Active]-Konto bedeutet einen zahlenden Kunden, nicht nur für Beratung, sondern für den Audience Manager SKU.
      * **[!UICONTROL Demo]**: Geben Sie an, dass die Firma nur zu Demozwecken verwendet werden soll. Berichte-Daten werden automatisch gefälscht.
      * **[!UICONTROL Prospect]**: Geben Sie an, dass es sich bei der Firma um einen potenziellen Audience Manager-Client handelt, z. B. um eine kostenlose Firma  [!DNL POC] oder eine Kontoeinrichtung für eine Verkaufsdemo.
      * **[!UICONTROL Test]**: Geben Sie an, dass die Firma nur zu internen Testzwecken verwendet werden soll.
   * **[!UICONTROL Account Types]**: Geben Sie den vollständigen Satz von Kontotypen für diese Firma an. Kein Kontotyp schließt sich gegenseitig mit anderen Typen aus.
      * **[!UICONTROL Full AAM]**: Geben Sie an, dass die Firma über ein vollständiges Adobe Audience Manager-Konto verfügt und die Benutzer Zugriff auf die Anmeldung haben.
      * **[!UICONTROL MMP]**: Geben Sie an, dass die Firma für die Verwendung der  [!UICONTROL Master Marketing Profile] ([!UICONTROL MMP])-Funktionen aktiviert wurde. Das [!UICONTROL MMP] ermöglicht die Freigabe von Audiencen über das Experience Cloud mit einem [!UICONTROL Experience Cloud ID] ([!DNL MCID]), das jedem Besucher zugewiesen und dann vom Audience Manager verwendet wird. Wenn Sie diesen Kontotyp auswählen, wird auch [!UICONTROL Experience Cloud ID Service] automatisch ausgewählt.

         Weitere Informationen finden Sie unter [Audiencen Services - Übergeordnet Marketing Profil](https://marketing.adobe.com/resources/help/en_US/mcloud/audience_library.html).
   * **[!UICONTROL Data Source]**: Geben Sie an, dass die Firma ein Drittanbieter für Daten in Audience Manager ist.
   * **[!UICONTROL Targeting Partner]**: Geben Sie an, dass die Firma als Targeting-Plattform für Audience Manager fungiert.
   * **[!UICONTROL Visitor ID Service]**: Geben Sie an, dass die Firma für die Verwendung der  [!UICONTROL Experience Cloud Visitor ID Service]Variable aktiviert wurde.

      Das [!UICONTROL Experience Cloud Visitor ID Service] stellt eine universelle Besucher-ID für alle Experience Cloud-Lösungen bereit. Weitere Informationen finden Sie im Benutzerhandbuch [Experience Cloud-Besucher-ID-Dienst](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-overview.html).

   * **[!UICONTROL Agency]**: Geben Sie an, dass die Firma über ein  [!UICONTROL Agency] Konto verfügt.



1. Klicken **[!UICONTROL Create]**. Fahren Sie mit den Anweisungen unter [Firma-Profil bearbeiten](../companies/admin-manage-company-profiles.md#edit-company-profile) fort.

   ![Schritt-Ergebnis](assets/add_company.png)

## Bearbeiten von Firmenprofilen {#edit-company-profile}

Bearbeiten Sie das Profil einer Firma, einschließlich Name, Beschreibung, Subdomäne, Lebenszyklus usw.

<!-- t_edit_company_profile.xml -->

1. Klicken Sie auf **[!UICONTROL Companies]**, suchen Sie die gewünschte Firma und klicken Sie darauf, um deren [!UICONTROL Profile]-Seite anzuzeigen.

   Verwenden Sie das Feld [!UICONTROL Search] oder die Paginierungssteuerelemente am unteren Rand der Liste, um die gewünschte Firma zu finden. Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.

   ![Schritt-Ergebnis](assets/profile_company.png)

1. Bearbeiten Sie die Felder je nach Bedarf:

   * **[!UICONTROL Name]**: Bearbeiten Sie den Namen der Firma. Dies ist ein erforderliches Feld.
   * **[!UICONTROL Description]**: Bearbeiten Sie die Beschreibung der Firma. Dies ist ein erforderliches Feld.
   * **[!UICONTROL Subdomain]**: (Erforderlich) Geben Sie die Subdomäne der Firma an. Der von Ihnen eingegebene Text wird als Subdomäne des Ereignis-Aufrufs angezeigt. Das kann man nicht ändern. Es muss sich um eine Zeichenfolge von [!DNL URL]-gültigen Zeichen handeln.

      Wenn Ihre Firma beispielsweise [!DNL AcmeCorp] heißt, wäre die Subdomäne [!DNL acmecorp].

      Audience Manager verwendet die Subdomäne für [!UICONTROL Data Collection Server] (DCS). Wenn im vorherigen Beispiel die vollständige [!DNL URL] Ihrer Firma in [!UICONTROL DCS] [!DNL acmecorp.demdex.net] lautet.

   * **[!UICONTROL imsOrgld]**: ([!UICONTROL Identity Management System Organization ID]) Mit dieser ID können Sie Ihre Firma mit dem Adobe Experience Cloud verbinden.
   * **[!UICONTROL Lifecyle]**: Geben Sie die gewünschte Phase für die Firma an:
      * **[!UICONTROL Active]**: Geben Sie an, dass die Firma ein aktiver Audience Manager-Client sein soll. Ein Aktives Konto bedeutet einen zahlenden Kunden, nicht nur für Beratung, sondern für den Audience Manager-SKU.
      * **[!UICONTROL Demo]**: Geben Sie an, dass die Firma nur zu Demozwecken verwendet werden soll. Berichte-Daten werden automatisch gefälscht.
      * **[!UICONTROL Prospect]**: Geben Sie an, dass es sich bei der Firma um einen potenziellen Audience Manager-Client handelt, z. B. um eine kostenlose Firma  [!DNL POC] oder eine Kontoeinrichtung für eine Verkaufsdemo.
      * **[!UICONTROL Test]**: Geben Sie an, dass die Firma nur zu internen Testzwecken verwendet werden soll.
   * **[!UICONTROL Account Types]**: Geben Sie den vollständigen Satz von Kontotypen für diese Firma an. Kein Kontotyp schließt sich gegenseitig mit anderen Typen aus.
      * **[!UICONTROL Full AAM]**: Geben Sie an, dass die Firma über ein vollständiges Adobe Audience Manager-Konto verfügt und die Benutzer Zugriff auf die Anmeldung haben.
      * **[!UICONTROL MMP]**: Geben Sie an, dass die Firma für die Verwendung der Übergeordnet Marketing Profil ([!UICONTROL MMP])-Funktionen aktiviert wurde.

         Wenn Sie diesen Kontotyp auswählen, wird auch **[!UICONTROL Visitor ID Service]** automatisch ausgewählt.
Weitere Informationen finden Sie unter [Audiencen Services - Übergeordnet Marketing Profil](https://marketing.adobe.com/resources/help/en_US/mcloud/audience_library.html).
   * **[!UICONTROL Data Source]**: Geben Sie an, dass die Firma ein Drittanbieter für Daten in Audience Manager ist.
   * **[!UICONTROL Targeting Partner]**: Geben Sie an, dass die Firma als Targeting-Plattform für Audience Manager fungiert.
   * **[!UICONTROL Visitor ID Service]**: Geben Sie an, dass die Firma für die Verwendung des Experience Cloud-Besucher-ID-Diensts aktiviert wurde.

      Der Experience Cloud-Besucher-ID-Dienst stellt eine universale Besucher-ID für alle Experience Cloud-Lösungen bereit. Weitere Informationen finden Sie im Benutzerhandbuch [Experience Cloud-Besucher-ID-Dienst](https://microsite.omniture.com/t2/help/en_US/mcvid/mcvid_service.html).

   * **[!UICONTROL Agency]**: Geben Sie an, dass die Firma über ein Agenturkonto verfügt.
   * **[!UICONTROL Features]**: Wählen Sie die gewünschten Optionen aus:
      * **[!UICONTROL Password Expiration]**: Legt fest, dass alle Benutzerkennwörter innerhalb dieser Firma nach 90 Tagen ablaufen, um die Sicherheit der Audience Manager zu erhöhen.
      * **[!UICONTROL Reporting]**: Aktiviert Audience Manager Berichte für diese Firma.
      * **[!UICONTROL Role Based Access Controls]**: Aktivieren Sie rollenbasierte Zugriffskontrollen für diese Firma. Mithilfe rollenbasierter Zugriffskontrollen können Sie Benutzergruppen mit unterschiedlichen Zugriffsberechtigungen erstellen. Einzelne Benutzer innerhalb dieser Gruppen können dann nur auf bestimmte Funktionen in Audience Manager zugreifen.


1. Klicken **[!UICONTROL Submit Updates]**.

## Löschen eines Firma-Profils {#delete-company-profile}

Verwenden Sie die Seite [!UICONTROL Companies] im Audience Manager [!UICONTROL Admin], um eine vorhandene Firma zu löschen.

<!-- t_delete_company.xml -->

>[!NOTE]
>
>Sie müssen über die [!UICONTROL DEXADMIN]-Rolle verfügen, um vorhandene Firmen zu löschen.

1. Um eine vorhandene Firma zu löschen, klicken Sie auf **[!UICONTROL Companies]**.

   ![Schritt-Ergebnis](assets/companies.png)

1. Klicken Sie in der Spalte **[!UICONTROL Actions]** der gewünschten Firma auf ![](assets/icon_delete.png).
1. Klicken Sie auf **[!UICONTROL OK]**, um den Löschvorgang zu bestätigen.
