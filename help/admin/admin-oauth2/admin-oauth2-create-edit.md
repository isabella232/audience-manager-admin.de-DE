---
description: Auf der Seite "oauth 2-Kunden" können Sie eine Liste der oauth 2-Clients in Ihrer Audience Manager-Konfiguration anzeigen. Sie können bestehende Clients bearbeiten oder löschen oder neue Clients erstellen, sofern Sie über die entsprechenden Benutzerrollen verfügen.
seo-description: Auf der Seite "oauth 2-Kunden" können Sie eine Liste der oauth 2-Clients in Ihrer Audience Manager-Konfiguration anzeigen. Sie können bestehende Clients bearbeiten oder löschen oder neue Clients erstellen, sofern Sie über die entsprechenden Benutzerrollen verfügen.
seo-title: Oauth 2-Clients
title: Oauth 2-Clients
uuid: 3 e 654053-fb 2 f -4 d 8 f-a 53 c-b 5 c 3 b 8 dbdaaa
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54

---


# Oauth 2-Clients {#oauth-clients}

Verwenden Sie die [!UICONTROL OAuth2 Clients] Seite, um eine Liste der [!UICONTROL OAuth2] Kunden in Ihrer [!DNL Audience Manager] Konfiguration anzuzeigen. Sie können bestehende Clients bearbeiten oder löschen oder neue Clients erstellen, sofern Sie über die entsprechenden Benutzerrollen verfügen.

## Überblick {#overview}

<!-- c_oauth.xml -->

>[!NOTE]
>
>Stellen Sie sicher, dass Ihr Kunde die [oauth 2](https://docs.adobe.com/content/help/en/audience-manager/user-guide/api-and-sdk-code/rest-apis/aam-api-getting-started.html#oauth) -Dokumentation in [! Benutzerhandbuch zu DNL Audience Manager.

[!DNL OAuth2] ist ein offener Standard für die Autorisierung, um geschützten delegierten Zugriff auf [!DNL Audience Manager] Ressourcen im Auftrag eines Ressourceneigentümers bereitzustellen.

![](assets/oauth.png)

Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.

Verwenden Sie das [!UICONTROL Search] Feld oder die Seitenumbruchsteuerelemente unten in der Liste, um den gewünschten Client zu finden.

## Oauth 2-Client erstellen oder bearbeiten {#create-edit-client}

<!-- t_create_edit_auth.xml -->

Verwenden Sie die [!UICONTROL OAuth2 Clients] Seite im Audience Manager [!UICONTROL Admin] -Tool, um einen neuen [!UICONTROL Oauth2] Client zu erstellen oder einen vorhandenen Client zu bearbeiten.

1. Klicken Sie auf &gt;, um einen neuen [!UICONTROL OAuth2] Client **[!UICONTROL OAuth2 Clients]** zu erstellen **[!UICONTROL Add OAuth2 Client]**. Um einen vorhandenen [!UICONTROL OAuth2] Client zu bearbeiten, klicken Sie in der **[!UICONTROL Client ID]** Spalte auf den gewünschten Client.
1. Geben Sie den gewünschten Namen für diesen [!UICONTROL OAuth2] Client an. Beachten Sie, dass dies nur ein Name für den Datensatz ist.
1. Geben Sie die E-Mail-Adresse [!UICONTROL OAuth2] des Kunden an. Es gibt eine Beschränkung auf eine E-Mail-Adresse.
1. Wählen Sie aus der **[!UICONTROL Partner]** Dropdownliste den gewünschten Partner aus.
1. Geben Sie in das **[!UICONTROL Client ID]** Feld die gewünschte ID ein. Dies ist der Wert, der beim Senden [!DNL API] von Anforderungen verwendet wird. Das Präfix wird automatisch gefüllt, wenn Sie mit der Eingabe beginnen, nachdem Sie eine [!UICONTROL Partner] aus der Dropdown-Liste im vorherigen Schritt ausgewählt haben. Das richtige Format ist &lt; *`partner subdomain`*&gt; - &lt; *`Audience Manager username`*&gt;.
1. Aktivieren oder deaktivieren Sie das **[!UICONTROL Restrict to Partner Users]** Kontrollkästchen, falls gewünscht. Wenn dieses Kontrollkästchen aktiviert ist, muss der Benutzer ein [!DNL Audience Manager] Benutzer sein, der für den ausgewählten Partner aufgelistet ist. Wir empfehlen, dass Sie diese Option auswählen.
1. Aktivieren oder deaktivieren Sie im **[!UICONTROL Scope]** Abschnitt die Kontrollkästchen **[!UICONTROL Read]** und **[!UICONTROL Write]** aktivieren Sie die Kontrollkästchen.
1. Wählen Sie im **[!UICONTROL Grant Type]** Abschnitt die gewünschten Möglichkeiten zur Autorisierung aus. Es wird empfohlen, die Standardeinstellungen [!UICONTROL Password] und [!UICONTROL Refresh-token] -optionen zu verwenden.

   * **[!UICONTROL Implicit]**: Wenn Sie diese Option auswählen, wird das [!UICONTROL Redirect URI] Feld aktiviert. Dem Benutzer wird nach Authentifizierung ein automatisches Zugriffstoken zugewiesen und es wird sofort an die Umleitung [!DNL URI]gesendet.
   * **[!UICONTROL Authorization Code]**: Wenn Sie diese Option auswählen, wird das [!UICONTROL Redirect URI] Feld aktiviert. Der Benutzer wird nach Authentifizierung an den Client zurückgegeben und wird dann an die Umleitung [!DNL URI]gesendet.
   * **[!UICONTROL Password]**: Der Benutzer wird mit einem vom Benutzer eingegebenen Kennwort authentifiziert und nicht über einen automatischen Validierungsversuch über einen Autorisierungsserver.
   * **[!UICONTROL Refresh_token]**: Wird verwendet, um ein abgelaufenes Zugriffstoken über einen längeren Zeitraum zu aktualisieren.

1. Geben Sie im **[!UICONTROL Redirect URI]** Feld den [!DNL URI]gewünschten Wert an. Diese Option ist nur aktiviert, wenn Sie die gewünschten Typen **[!UICONTROL Implicit]****[!UICONTROL Authorization_code]** auswählen. Mit dem **[!UICONTROL Redirect URI]** Feld können Sie einen kommagetrennten Wert der zulässigen [!DNL URI] Werte angeben. Dies ist der [!DNL URI] Benutzer eines Clients, nachdem er den Client für den [!DNL API] Zugriff genehmigt hat.
1. Geben Sie die gewünschte Ablaufzeit (in Sekunden) für den Zugriff und die Aktualisierung des Token an.

   * **[!UICONTROL Access Token Expiration Time]**: Die Anzahl der Sekunden, die ein Zugriffstoken nach der Ausgabe gültig ist. Kann null sein, um die Plattformstandardeinstellung (12 Stunden) zu verwenden. Es kann auch -1 sein, um anzuzeigen, dass das Zugriffstoken nicht abläuft.
   * **[!UICONTROL Refresh Token Expiration Time]**: Die Anzahl der Sekunden, die ein Aktualisierungstoken nach der Ausgabe gültig ist. Kann null sein, um die Plattformstandardeinstellung (30 Tage) zu verwenden.

1. Klicken Sie auf **[!UICONTROL Save]**.

Klicken Sie zum Löschen eines [!UICONTROL OAuth2] Clients **[!UICONTROL OAuth2 Clients]** auf und klicken ![](assets/icon_delete.png) Sie dann in die **[!UICONTROL Actions]** Spalte für den gewünschten Client.

>[!MORE_ LIKE_ THIS]
>
>* [API-Anforderungen und Empfehlungen](../admin-oauth2/aam-admin-api-requirements.md)

