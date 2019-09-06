---
description: Einige Kunden möchten ihren Amazon Simple Storage Service (Amazon S 3) oder geheimen Schlüssel nicht für Adobe bereitstellen, um die Zieldaten in ihre Behälter hochzuladen.
seo-description: Einige Kunden möchten ihren Amazon Simple Storage Service (Amazon S 3) oder geheimen Schlüssel nicht für Adobe bereitstellen, um die Zieldaten in ihre Behälter hochzuladen.
seo-title: So autorisieren Sie Cross-Account Amazon S 3-Behälterzugriff für Stapelziele
title: So autorisieren Sie Cross-Account Amazon S 3-Behälterzugriff für Stapelziele
uuid: da 2 bcbda-a 765-437 a-bfe 9-4355383 a 4730
translation-type: tm+mt
source-git-commit: be661580da839ce6332a0ad827dec08e854abe54

---


# So autorisieren Sie Cross-Account Amazon S 3-Behälterzugriff für Stapelziele{#authorize-cross-account-bucket-batch}

Einige Kunden möchten ihren [!DNL Amazon S3] Zugriff oder ihre Geheimschlüssel nicht an Adobe bereitstellen, um die Zieldaten in ihre Behälter hochzuladen.

Eine Alternative, die unsere Kunden bieten können, ist [!UICONTROL Cross-Account Bucket Permissions][!DNL Amazon S3]in. Dieser Vorgang wird in der [AWS-Dokumentation beschrieben](https://docs.aws.amazon.com/AmazonS3/latest/dev/example-walkthroughs-managing-access-example2.html). Gehen Sie wie folgt vor, um diese Alternative in Audience Manager zu aktivieren:

1. Wechseln **[!UICONTROL Servers]** Sie zu und wählen **[!UICONTROL Create Server]** Sie diese aus.
1. Wählen **[!UICONTROL S3]** Sie in der **[!UICONTROL Protocol/Credentials]** Dropdown-Maske aus.
1. Aktivieren **[!UICONTROL Use Internal Adobe Key]** Sie die Option.
1. Verwenden [!DNL Amazon S3]Sie das Konto und den Behälternamen Ihres Kunden.
1. Stellen Sie sicher, dass Ihr Kunde das [!DNL Amazon S3] Konto `975822914085` in seinem [!DNL S3] Behälter auflistet.

>[!NOTE]
>
>Unser ausgehender Herausgeber stellt sicher, dass die Zugriffsebene `bucket-owner-full-control` für hochgeladene Daten festgelegt ist, damit Ihr Kunde diese Daten selbst nutzen kann.
