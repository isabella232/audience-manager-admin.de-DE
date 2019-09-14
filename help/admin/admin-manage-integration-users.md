---
description: Auf der Seite "Integrationsbenutzer"können Sie eine Liste der Benutzer in Ihrer Audience Manager-Konfiguration anzeigen. Sie können vorhandene Benutzer bearbeiten oder löschen oder neue Benutzer erstellen, sofern Ihnen die entsprechenden Benutzerrollen zugewiesen sind.
seo-description: Auf der Seite "Integrationsbenutzer"können Sie eine Liste der Benutzer in Ihrer Audience Manager-Konfiguration anzeigen. Sie können vorhandene Benutzer bearbeiten oder löschen oder neue Benutzer erstellen, sofern Ihnen die entsprechenden Benutzerrollen zugewiesen sind.
seo-title: Integrationsbenutzer
title: Integrationsbenutzer
uuid: 13dcb3fb-4561-409c-84da-943d0d390cf3
translation-type: tm+mt
source-git-commit: 10adb6b06160f5a5c4068483b407e5798fc10150

---


# Integrationsbenutzer {#integration-users}

Auf der [!UICONTROL Integration Users] Seite können Sie eine Liste der Benutzer in Ihrer Audience Manager-Konfiguration anzeigen. Sie können vorhandene Benutzer bearbeiten oder löschen oder neue Benutzer erstellen, sofern Ihnen die entsprechenden Benutzerrollen zugewiesen sind.

<!-- c_integration_users.xml -->

Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.
Verwenden Sie das [!UICONTROL Search] Feld oder die Paginierungssteuerelemente unten in der Liste, um den gewünschten Benutzer zu finden.

## Benutzer erstellen oder bearbeiten {#create-edit-user}

Verwenden Sie die [!UICONTROL Integration Users] Seite im Audience Manager- [!UICONTROL Admin] Tool, um einen neuen Benutzer zu erstellen oder das Konto eines vorhandenen Benutzers zu bearbeiten.

<!-- t_create_user.xml -->

>[!NOTE]
>
>Sie müssen die [!UICONTROL CREATE_USER] Rolle haben, um neue Benutzer zu erstellen. Sie müssen die [!UICONTROL EDIT_USER] Rolle haben, um vorhandene Benutzer zu bearbeiten.

1. Um einen neuen Benutzer zu erstellen, klicken Sie auf **[!UICONTROL Integration Users]** &gt; **[!UICONTROL Create a New User]**. To edit an existing user, click the desired user in the **[!UICONTROL Username]** column.
2. Füllen Sie die Felder aus:
   * **[!UICONTROL First Name]**: (Erforderlich) Geben Sie den Vornamen des Benutzers an.
   * **[!UICONTROL Last Name]**: (Erforderlich) Geben Sie den Nachnamen des Benutzers an.
   * **[!UICONTROL Username]**: (Erforderlich) Geben Sie den Benutzernamen des Benutzers an.
   * **[!UICONTROL Email Address]**: (Erforderlich) Geben Sie die E-Mail-Adresse des Benutzers an.
   * **[!UICONTROL Phone Number]**: Geben Sie die Telefonnummer des Benutzers an.
   * **[!UICONTROL IMS ID]**: Geben Sie die des Benutzers an [!UICONTROL Internet Messaging Service ID].
   * **[!UICONTROL User Roles]**: Wählen Sie die gewünschten Benutzerrollen aus:
      * **[!UICONTROL DEXADMIN]**: Bietet Administratorzugriff zum Ausführen von Aufgaben im Audience Manager- [!UICONTROL Admin] Tool. Wenn Sie diese Option nicht auswählen, können Sie einzelne Rollen auswählen. Mit diesen Rollen können Benutzer Aufgaben mithilfe von [!DNL API] Aufrufen ausführen, jedoch nicht im Admin-Tool.
      * **[!UICONTROL CREATE_USERS]**: Ermöglicht Benutzern das Erstellen neuer Benutzer mithilfe eines [!DNL API] Aufrufs.
      * **[!UICONTROL DELETE_USERS]**: Ermöglicht Benutzern das Löschen vorhandener Benutzer mithilfe eines [!DNL API] Aufrufs.
      * **[!UICONTROL EDIT_USERS]**: Ermöglicht Benutzern, bestehende Benutzer mithilfe eines [!DNL API] Aufrufs zu bearbeiten.
      * **[!UICONTROL VIEW_USERS]**: Ermöglicht Benutzern, andere Benutzer in Ihrer Audience Manager-Konfiguration mithilfe eines [!DNL API] Aufrufs anzuzeigen.
      * **[!UICONTROL CREATE_PARTNERS]**: Ermöglicht Benutzern das Erstellen von Audience Manager-Partnern mithilfe eines [!DNL API] Aufrufs.
      * **[!UICONTROL DELETE_PARTNERS]**: Ermöglicht Benutzern das Löschen von Audience Manager-Partnern durch einen [!DNL API] Aufruf.
      * **[!UICONTROL EDIT_PARTNERS]**: Ermöglicht Benutzern, Audience Manager-Partner mithilfe eines [!DNL API] Aufrufs zu bearbeiten.
      * **[!UICONTROL VIEW_PARNTERS]**: Ermöglicht Benutzern die Anzeige von Audience Manager-Partnern über einen [!DNL API] Aufruf.
   * **** Status: Wählen Sie **[!UICONTROL Active]** diese Option, um diesen Benutzer zu einem aktivierten Audience Manager-Benutzer zu machen.
3. Klicken Sie auf **[!UICONTROL Submit]**.

## Delete a User {#delete-user}

Verwenden Sie die [!UICONTROL Integration Users] Seite im Audience Manager- [!UICONTROL Admin] Tool, um einen vorhandenen Benutzer zu löschen.

<!-- t_delete_user.xml -->

>[!NOTE]
>
>Sie müssen die **[!UICONTROL DELETE_USER]** Rolle haben, um neue Benutzer zu erstellen.

1. Klicken Sie auf **[!UICONTROL Integration Users]**.
2. Klicken Sie ![](assets/icon_delete.png) in die **[!UICONTROL Actions]** Spalte des gewünschten Benutzers.
3. Klicken Sie auf **[!UICONTROL OK], um den Löschvorgang zu bestätigen.**