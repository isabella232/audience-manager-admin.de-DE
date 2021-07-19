---
description: Verwenden Sie die Seite OAuth2-Clients , um eine Liste der OAuth2-Clients in Ihrer Audience Manager-Konfiguration anzuzeigen. Sie können vorhandene Clients bearbeiten oder löschen oder neue Clients erstellen, sofern Ihnen die entsprechenden Benutzerrollen zugewiesen sind.
seo-description: Verwenden Sie die Seite OAuth2-Clients , um eine Liste der OAuth2-Clients in Ihrer Audience Manager-Konfiguration anzuzeigen. Sie können vorhandene Clients bearbeiten oder löschen oder neue Clients erstellen, sofern Ihnen die entsprechenden Benutzerrollen zugewiesen sind.
seo-title: OAuth2-Clients
title: OAuth2-Clients
uuid: 3e654053-fb2f-4d8f-a53c-b5c3b8dbdaaa
exl-id: 993eae04-02e8-4554-a6fe-cf599053bfc9
source-git-commit: f5d74995f0664cf63e68b46f1f3c608f34df0e80
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 2%

---

# OAuth2-Clients {#oauth-clients}

Verwenden Sie die Seite [!UICONTROL OAuth2 Clients] , um eine Liste der [!UICONTROL OAuth2]-Clients in Ihrer [!DNL Audience Manager]-Konfiguration anzuzeigen. Sie können vorhandene Clients bearbeiten oder löschen oder neue Clients erstellen, sofern Ihnen die entsprechenden Benutzerrollen zugewiesen sind.

## Überblick {#overview}

<!-- c_oauth.xml -->

>[!NOTE]
>
>Stellen Sie sicher, dass Ihr Kunde die [OAuth2](https://docs.adobe.com/content/help/en/audience-manager/user-guide/api-and-sdk-code/rest-apis/aam-api-getting-started.html#oauth) -Dokumentation im Audience Manager-Benutzerhandbuch liest.

[!DNL OAuth2] ist ein offener Standard für die Autorisierung, um einen gesicherten delegierten Zugriff auf  [!DNL Audience Manager] Ressourcen im Namen eines Ressourceneigentümers bereitzustellen.

![](assets/oauth.png)

Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.

Verwenden Sie das Feld [!UICONTROL Search] oder die Paginierungssteuerelemente unten in der Liste, um den gewünschten Client zu finden.

## Erstellen oder Bearbeiten eines OAuth2-Clients {#create-edit-client}

<!-- t_create_edit_auth.xml -->

Verwenden Sie die Seite [!UICONTROL OAuth2 Clients] im Audience Manager [!UICONTROL Admin] , um einen neuen [!UICONTROL Oauth2]-Client zu erstellen oder einen vorhandenen Client zu bearbeiten.

1. Um einen neuen [!UICONTROL OAuth2]-Client zu erstellen, klicken Sie auf **[!UICONTROL OAuth2 Clients]** > **[!UICONTROL Add OAuth2 Client]**. Um einen vorhandenen [!UICONTROL OAuth2]-Client zu bearbeiten, klicken Sie in der Spalte **[!UICONTROL Client ID]** auf den gewünschten Client.
1. Geben Sie den gewünschten Namen für diesen [!UICONTROL OAuth2]-Client an. Beachten Sie, dass dies nur ein Name für den Datensatz ist.
1. Geben Sie die E-Mail-Adresse des Kunden an. [!UICONTROL OAuth2] Es gibt eine Grenze von einer E-Mail-Adresse.
1. Wählen Sie aus der Dropdownliste **[!UICONTROL Partner]** den gewünschten Partner aus.
1. Geben Sie im Feld **[!UICONTROL Client ID]** die gewünschte ID an. Dies ist der Wert, der beim Senden von [!DNL API]-Anfragen verwendet wird. Das Präfix wird automatisch ausgefüllt, wenn Sie mit der Eingabe beginnen, nachdem Sie in der Dropdown-Liste im vorherigen Schritt ein [!UICONTROL Partner] ausgewählt haben. Das richtige Format ist &lt; *`partner subdomain`* - &lt; *`Audience Manager username`*>.
1. Aktivieren bzw. deaktivieren Sie das Kontrollkästchen **[!UICONTROL Restrict to Partner Users]** nach Bedarf. Wenn dieses Kontrollkästchen aktiviert ist, muss der Benutzer ein [!DNL Audience Manager] Benutzer sein, der für den ausgewählten Partner aufgelistet ist. Es hat sich bewährt, diese Option zu wählen.
1. Aktivieren bzw. deaktivieren Sie im Abschnitt **[!UICONTROL Scope]** die Kontrollkästchen **[!UICONTROL Read]** und **[!UICONTROL Write]** nach Bedarf.
1. Wählen Sie im Abschnitt **[!UICONTROL Grant Type]** die gewünschten Autorisierungsmöglichkeiten aus. Es wird empfohlen, die Standardeinstellungen der Optionen [!UICONTROL Password] und [!UICONTROL Refresh-token] zu verwenden.

   * **[!UICONTROL Implicit]**: Wenn Sie diese Option auswählen, ist das  [!UICONTROL Redirect URI] Feld aktiviert. Der Benutzer erhält nach der Authentifizierung ein automatisches Zugriffstoken und wird sofort an die Umleitung [!DNL URI] gesendet.
   * **[!UICONTROL Authorization Code]**: Wenn Sie diese Option auswählen, ist das  [!UICONTROL Redirect URI] Feld aktiviert. Der Benutzer wird nach der Authentifizierung an den Client zurückgegeben und dann an die Weiterleitung [!DNL URI] gesendet.
   * **[!UICONTROL Password]**: Der Benutzer wird mit einem vom Benutzer eingegebenen Kennwort authentifiziert und nicht mit einem automatischen Validierungsversuch über einen Autorisierungsserver.
   * **[!UICONTROL Refresh_token]**: Wird verwendet, um ein abgelaufenes Zugriffstoken über einen längeren Zeitraum zu aktualisieren.

1. Geben Sie im Feld **[!UICONTROL Redirect URI]** den gewünschten [!DNL URI] an. Diese Option ist nur aktiviert, wenn Sie die Grant-Typen **[!UICONTROL Implicit]** und **[!UICONTROL Authorization_code]** auswählen. Mit dem Feld **[!UICONTROL Redirect URI]** können Sie einen kommagetrennten Wert akzeptabler [!DNL URI]-Werte angeben. Dies ist das [!DNL URI], zu dem ein Benutzer eines Clients umgeleitet wird, nachdem er den Client für den Zugriff auf [!DNL API] genehmigt hat.
1. Geben Sie die gewünschte Ablaufzeit (in Sekunden) für den Ablauf des Zugriffs- und Aktualisierungstokens an.

   * **[!UICONTROL Access Token Expiration Time]**: Die Anzahl der Sekunden, die ein Zugriffstoken nach der Ausstellung gültig ist. Kann null sein, um den Plattformstandard zu verwenden (12 Stunden). Kann auch -1 sein, um anzugeben, dass das Zugriffstoken nicht abläuft.
   * **[!UICONTROL Refresh Token Expiration Time]**: Die Anzahl der Sekunden, die ein Aktualisierungstoken nach der Ausgabe gültig ist. Kann null sein, um den Plattformstandard zu verwenden (30 Tage).

1. Klicken **[!UICONTROL Save]**.

Um einen [!UICONTROL OAuth2]-Client zu löschen, klicken Sie auf **[!UICONTROL OAuth2 Clients]** und dann in der Spalte **[!UICONTROL Actions]** auf ![](assets/icon_delete.png) für den gewünschten Client.

>[!MORELIKETHIS]
>
>* [API-Anforderungen und -Empfehlungen](../admin-oauth2/aam-admin-api-requirements.md)

