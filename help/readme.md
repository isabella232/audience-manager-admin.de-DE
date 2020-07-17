---
source-git-commit: b76aa4a35a5216aabd60d07352a7c4bd2b3e6e32
workflow-type: tm+mt
translation-type: tm+mt
source-wordcount: '329'
ht-degree: 2%

---
# Anleitung

**Note: This page (or any readme.md page) will not publish to the customer facing documentation**

## Inhaltsverzeichnis

+ `TOC.md` im Stammverzeichnis des Benutzerhandbuchs finden Sie die Organisation der Themen, die im Handbuch für diese Lösung enthalten sind.
+ Jedes Benutzerhandbuch verfügt über eine eigene, eindeutige Benutzeroberfläche `TOC.md`, in der Sie nach Bedarf alle Seiten/Themen bestellen können.
+ Die erste Seite aller Benutzerhandbücher ist `overview.md`.

## Benutzerhandbuch

+ Die Einführung in das Benutzerhandbuch heißt `overview.md`
+ Jedes Thema im Benutzerhandbuch hat einen eigenen Ordner.
   + Wenn ein Thema im Handbuch *Implementierung* aufgeführt ist, ist der entsprechende Ordner `/implementation`
+ Alle Bild-Assets werden im Stammverzeichnis `/assets` des Benutzerhandbuchs gespeichert.
   + Alle Bilder im `/assets` Ordner werden lokalisiert.
   + Alle Bilder im `/no-localize` Verzeichnis werden nicht lokalisiert (es gibt eine Überraschung!). Auf diese Weise kann sichergestellt werden, dass bestimmte Assets in lokalen Versionen nicht unnötig reproduziert werden.

## Metrikdaten auf Benutzerhandbuchebene

+ Metadaten, die das Benutzerhandbuch beschreiben, werden im `TOC.md`Ordner gespeichert. Dazu gehören:
   + product - Name des Produkts/der Funktion.
   + Cloud - Cloud, zu der dieses Produkt gehört.
   + Audience - Audience oder Archetyp, auf den der Guide abzielt.
   + user-guide - Name des Benutzerhandbuchs.

## Metadaten auf Seitenniveau

+ Metadaten, die zur Beschreibung eines Dokuments erforderlich sind, werden als Teil jeder einzelnen Seite gespeichert. Dazu gehören:
   + title - Titel der Seite.
   + description - description of page.
   + seo-title - seo alternative title.
   + seo-description - alternativer Titel für SEO Zwecke.
   + short-title - (optionales Feld).
   + index - ja/nein - wird die Seite von der Suchplattform von Adobe indiziert.
   + translate - ja / nein - wird diese Seite lokalisiert.
   + version - wird hauptsächlich für AEM und Kampagne verwendet, um die Produktversion zu kennzeichnen.
   + private-feature-pack - wird primär für AEM verwendet.
   + beta - ist dieses Produkt in der Beta?
   + redirect - kann verwendet werden, um eine Referenz zu einer neuen Seite zu erstellen, falls dies erforderlich ist.
   + doc-type: reference (Standard) / troubleshooting / developer / tutorial / kb / whitepaper.

## Weitere Informationen

Weitere Veröffentlichungsanweisungen, Stilhandbücher, Beispiele und andere Ressourcen finden Sie im [kollaborativen Dokumentationsbericht](https://git.corp.adobe.com/AdobeDocs/collaborative-doc-instructions)
