---
description: Einige Kunden möchten möglicherweise nicht ihren Amazon Simple Datenspeicherung Service (Amazon S3) oder geheime Schlüssel zur Adobe bereitstellen, um das Hochladen von Zieldaten in ihre Behälter zu genehmigen.
seo-description: Einige Kunden möchten möglicherweise nicht ihren Amazon Simple Datenspeicherung Service (Amazon S3) oder geheime Schlüssel zur Adobe bereitstellen, um das Hochladen von Zieldaten in ihre Behälter zu genehmigen.
seo-title: So autorisieren Sie den kontoübergreifenden Amazon S3-Behälterzugriff für Stapelziele
title: So autorisieren Sie den kontoübergreifenden Amazon S3-Behälterzugriff für Stapelziele
uuid: da2bcbda-a765-437a-bfe9-4355383a4730
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# So autorisieren Sie den kontoübergreifenden Amazon S3-Behälterzugriff für Stapelziele{#authorize-cross-account-bucket-batch}

Einige Kunden möchten möglicherweise ihre [!DNL Amazon S3]-Zugriffs- oder geheimen Schlüssel nicht zur Adobe bereitstellen, um das Hochladen von Zieldaten in ihre Behälter zu genehmigen.

Eine Alternative, die wir unseren Kunden Angebot geben können, ist [!UICONTROL Cross-Account Bucket Permissions] in [!DNL Amazon S3]. Dieser Vorgang wird in der [AWS-Dokumentation](https://docs.aws.amazon.com/AmazonS3/latest/dev/example-walkthroughs-managing-access-example2.html) beschrieben. Gehen Sie wie folgt vor, um diese Alternative in Audience Manager zu aktivieren:

1. Gehen Sie zu **[!UICONTROL Servers]** und wählen Sie **[!UICONTROL Create Server]**.
1. Wählen Sie **[!UICONTROL S3]** in der Dropdown-Maske **[!UICONTROL Protocol/Credentials]** aus.
1. Aktivieren Sie die Option **[!UICONTROL Use Internal Adobe Key]**.
1. Verwenden Sie den Konto- und Behälternamen Ihres Kunden in [!DNL Amazon S3].
1. Stellen Sie sicher, dass Ihr Kunde weiß das [!DNL Amazon S3]-Konto `975822914085` auf seinem [!DNL S3]-Behälter auflistet.

>[!NOTE]
>
>Unser ausgehende Herausgeber stellt sicher, dass die Berechtigungsstufe `bucket-owner-full-control` für hochgeladene Daten festgelegt ist, damit Ihr Kunde Eigentümer dieser Daten sein kann.
