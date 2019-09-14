---
description: Einige Kunden möchten Adobe möglicherweise nicht den Zugriff auf den Amazon Simple Storage Service (Amazon S3) oder geheime Schlüssel zur Autorisierung des Uploads von Zieldaten in ihre Behälter bereitstellen.
seo-description: Einige Kunden möchten Adobe möglicherweise nicht den Zugriff auf den Amazon Simple Storage Service (Amazon S3) oder geheime Schlüssel zur Autorisierung des Uploads von Zieldaten in ihre Behälter bereitstellen.
seo-title: So autorisieren Sie den kontoübergreifenden Zugriff auf Amazon S3-Behälter für Stapelziele
title: So autorisieren Sie den kontoübergreifenden Zugriff auf Amazon S3-Behälter für Stapelziele
uuid: da2bcbda-a765-437a-bfe9-4355383a4730
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54

---


# So autorisieren Sie den kontoübergreifenden Zugriff auf Amazon S3-Behälter für Stapelziele{#authorize-cross-account-bucket-batch}

Einige Kunden möchten Adobe möglicherweise keine [!DNL Amazon S3] Zugriffs- oder geheimen Schlüssel zur Autorisierung des Uploads von Zieldaten in ihre Behälter bereitstellen.

Eine Alternative, die wir unseren Kunden bieten können, ist [!UICONTROL Cross-Account Bucket Permissions] in [!DNL Amazon S3]. Dieser Vorgang wird in der [AWS-Dokumentation](https://docs.aws.amazon.com/AmazonS3/latest/dev/example-walkthroughs-managing-access-example2.html)beschrieben. Gehen Sie wie folgt vor, um diese Alternative in Audience Manager zu aktivieren:

1. Gehen Sie zu **[!UICONTROL Servers]** und wählen Sie **[!UICONTROL Create Server]**.
1. Wählen Sie **[!UICONTROL S3]** in der **[!UICONTROL Protocol/Credentials]** Dropdownmaske aus.
1. Aktivieren Sie die **[!UICONTROL Use Internal Adobe Key]** Option.
1. Verwenden Sie den Konto- und Behälternamen Ihres Kunden in [!DNL Amazon S3].
1. Achten Sie darauf, dass Ihr Kunde das [!DNL Amazon S3] Konto `975822914085` auf seinem [!DNL S3] Bucket auf "Weiß"auflistet.

>[!NOTE]
>
>Unser ausgehende Herausgeber stellt sicher, dass die Berechtigungsebene für hochgeladene Daten festgelegt `bucket-owner-full-control` wird, damit Ihr Kunde diese Daten besitzen kann.
