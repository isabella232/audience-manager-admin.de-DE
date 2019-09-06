---
description: Auf der Seite "Integrationsbenutzer" können Sie eine Liste der Benutzer in Ihrer Audience Manager-Konfiguration anzeigen. Sie können bestehende Benutzer bearbeiten oder löschen oder neue Benutzer erstellen, sofern Sie über die entsprechenden Benutzerrollen verfügen.
seo-description: Auf der Seite "Integrationsbenutzer" können Sie eine Liste der Benutzer in Ihrer Audience Manager-Konfiguration anzeigen. Sie können bestehende Benutzer bearbeiten oder löschen oder neue Benutzer erstellen, sofern Sie über die entsprechenden Benutzerrollen verfügen.
seo-title: Integrationsbenutzer
title: Integrationsbenutzer
uuid: 13 dcb 3 fb -4561-409 c -84 da -943 d 0 d 390 cf 3
translation-type: tm+mt
source-git-commit: 10adb6b06160f5a5c4068483b407e5798fc10150

---


# Integrationsbenutzer {#integration-users}

Verwenden Sie die [!UICONTROL Integration Users] Seite, um eine Liste der Benutzer in Ihrer Audience Manager-Konfiguration anzuzeigen. Sie können bestehende Benutzer bearbeiten oder löschen oder neue Benutzer erstellen, sofern Sie über die entsprechenden Benutzerrollen verfügen.

<!-- c_integration_users.xml -->

Sie können jede Spalte in auf- oder absteigender Reihenfolge sortieren, indem Sie auf die Kopfzeile der gewünschten Spalte klicken.
Verwenden Sie das [!UICONTROL Search] Feld oder die Seitenumbruchsteuerelemente unten in der Liste, um den gewünschten Benutzer zu finden.

## Benutzer erstellen oder bearbeiten {#create-edit-user}

Verwenden Sie die [!UICONTROL Integration Users] Seite im Audience Manager [!UICONTROL Admin] -Tool, um einen neuen Benutzer zu erstellen oder um das Konto eines vorhandenen Benutzers zu bearbeiten.

<!-- t_create_user.xml -->

>[!NOTE]
>
>Sie müssen über die [!UICONTROL CREATE_USER] Rolle verfügen, um neue Benutzer zu erstellen. Sie müssen über die [!UICONTROL EDIT_USER] Rolle verfügen, um bestehende Benutzer zu bearbeiten.

1. Klicken Sie **[!UICONTROL Integration Users]** auf &gt; **[!UICONTROL Create a New User]**, um einen neuen Benutzer zu erstellen. To edit an existing user, click the desired user in the **[!UICONTROL Username]** column.
2. Füllen Sie die Felder aus:
   * **[!UICONTROL First Name]**: (Erforderlich) Geben Sie den Vornamen des Benutzers an.
   * **[!UICONTROL Last Name]**: (Erforderlich) Geben Sie den Nachnamen des Benutzers an.
   * **[!UICONTROL Username]**: (Erforderlich) Geben Sie den Benutzernamen des Benutzers an.
   * **[!UICONTROL Email Address]**: (Erforderlich) Geben Sie die E-Email-Adresse des Benutzers an.
   * **[!UICONTROL Phone Number]**: Geben Sie die Telefonnummer des Benutzers an.
   * **[!UICONTROL IMS ID]**: Geben [!UICONTROL Internet Messaging Service ID]Sie den Benutzer an.
   * **[!UICONTROL User Roles]**: Wählen Sie die gewünschten Benutzerrollen aus:
      * **[!UICONTROL DEXADMIN]**: Bietet Administratorzugriff, um Aufgaben im Audience Manager [!UICONTROL Admin] -Tool auszuführen. Wenn Sie diese Option nicht auswählen, können Sie einzelne Rollen auswählen. Mit diesen Rollen können Benutzer Aufgaben mithilfe [!DNL API] von Aufrufen durchführen, nicht jedoch im Admin-Tool.
      * **[!UICONTROL CREATE_USERS]**: Ermöglicht Benutzern, neue Benutzer mithilfe eines [!DNL API] Aufrufs zu erstellen.
      * **[!UICONTROL DELETE_USERS]**: Ermöglicht Benutzern, vorhandene Benutzer mit einem [!DNL API] Aufruf zu löschen.
      * **[!UICONTROL EDIT_USERS]**: Ermöglicht Benutzern das Bearbeiten vorhandener Benutzer, die einen [!DNL API] Aufruf verwenden.
      * **[!UICONTROL VIEW_USERS]**: Ermöglicht Benutzern, andere Benutzer in Ihrer Audience Manager-Konfiguration mithilfe eines [!DNL API] Aufrufs anzuzeigen.
      * **[!UICONTROL CREATE_PARTNERS]**: Ermöglicht Benutzern, Audience Manager-Partner mithilfe eines [!DNL API] Aufrufs zu erstellen.
      * **[!UICONTROL DELETE_PARTNERS]**: Hiermit können Benutzer Audience Manager-Partner mithilfe eines [!DNL API] Aufrufs löschen.
      * **[!UICONTROL EDIT_PARTNERS]**: Ermöglicht Benutzern, Audience Manager-Partner mithilfe eines [!DNL API] Aufrufs zu bearbeiten.
      * **[!UICONTROL VIEW_PARNTERS]**: Ermöglicht Benutzern das Anzeigen von Audience Manager-Partnern mit einem [!DNL API] Aufruf.
   * **Status:** Wählen **[!UICONTROL Active]** Sie diese Option, um diesen Benutzer zu einem aktivierten Audience Manager-Benutzer zu machen.
3. Klicken Sie auf **[!UICONTROL Submit]**.

## Delete a User {#delete-user}

Verwenden Sie die [!UICONTROL Integration Users] Seite im Audience Manager [!UICONTROL Admin] -Tool, um einen vorhandenen Benutzer zu löschen.

<!-- t_delete_user.xml -->

>[!NOTE]
>
>Sie müssen über die **[!UICONTROL DELETE_USER]** Rolle verfügen, um neue Benutzer zu erstellen.

1. Klicken Sie auf **[!UICONTROL Integration Users]**.
2. Klicken ![](assets/icon_delete.png) Sie in die **[!UICONTROL Actions]** Spalte des gewünschten Benutzers.
3. Klicken Sie auf **[!UICONTROL OK], um den Löschvorgang zu bestätigen.**