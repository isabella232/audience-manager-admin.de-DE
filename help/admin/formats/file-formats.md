---
description: Listet die Makros auf, mit denen Sie FTP-basierte Datendateien erstellen können. Einige Makros können für alle Datendateifelder und Zeilen verwendet werden. Andere Makros sind nur für Kopf- und Datenzeilen spezifisch.
seo-description: Listet die Makros auf, mit denen Sie FTP-basierte Datendateien erstellen können. Einige Makros können für alle Datendateifelder und Zeilen verwendet werden. Andere Makros sind nur für Kopf- und Datenzeilen spezifisch.
seo-title: Dateiformat-Makros
title: Dateiformat-Makros
uuid: f 91 c 91 b 6-6581-4 ed 7-8 d 7 f-f 8532 bd 41 df 9
translation-type: tm+mt
source-git-commit: e1122a7f3d3e8c2d67616eb56cb186a4750ed29b

---


# Dateiformat-Makros {#file-format-macros}

Listet die Makros auf, mit denen Sie basierte Datendateien erstellen [!DNL FTP]können. Einige Makros können für alle Datendateifelder und Zeilen verwendet werden. Andere Makros sind nur für Kopf- und Datenzeilen spezifisch.

## Häufige Makros {#common-macros}

Diese Makros können in jedem beliebigen Format verwendet werden. Beispiele finden Sie unter [Dateiformat-Makrobeispiele](../formats/file-format-examples.md).

<table id="table_A3309E175ABF4651BD11CE3632B3C553"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Makro </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>ASCII_ SOH</code> </p> </td> 
   <td colname="col2"> <p>Ein nicht druckbares ASCII-Zeichen. Es zeigt den Anfang einer Zeile oder einen Inhaltsabschnitt an. Sie kann auch zum Trennen von Datenspalten in einer Datei verwendet werden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DPID</code> </p> </td> 
   <td colname="col2"> <p>Target-Datenanbieter-ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>MASTER_ DPID</code> </p> </td> 
   <td colname="col2"> <p>Benutzer-ID-Schlüsseldatenanbieter-ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>ORDER_ ID</code> </p> </td> 
   <td colname="col2"> <p>Bestell-/Ziel-ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>PIDALIAS</code> </p> </td> 
   <td colname="col2"> <p>Ein Alias für eine Bestell-/Ziel-ID. </p> <p>Der Wert für diesen Alias wird im Feld <span class="wintitle"> "Foreign Account ID </span> «für ein Ziel (im Abschnitt <span class="wintitle"> " Grundlegende Einstellungen </span> «) festgelegt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SYNC_ MODE</code> </p> </td> 
   <td colname="col2"> <p>Gibt den Synchronisierungstyp an. Akzeptiert die folgenden optionalen Variablen: </p> 
    <ul id="ul_87E8E3CE6565447A9810B5119298CC7B"> 
     <li id="li_66F4889FB84E40AC92F69F3FF6B0042C"> <code>voll</code>: Vollständige Synchronisierung. </li> 
     <li id="li_BFE2C2D9A33A44FB9A840A7232ECCFFF"> <code>iter</code>: Inkrementelle Synchronisierung. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SYNC_ TYPE</code> </p> </td> 
   <td colname="col2"> <p>Gibt die Datenübertragungsmethode an. Akzeptiert die folgenden optionalen Variablen: </p> 
    <ul id="ul_13BE35BBBF7C4C67AEFC514C5D192902"> 
     <li id="li_195FE9B4C5494600BD17D7172A8FB630"> <code>ftp</code> </li> 
     <li id="li_751AD59C4C934D66BC530D9806B500AF"> <code>http</code> </li> 
     <li id="li_4638AF7D1FB54E2C890045048B85309C"> <code>s3</code> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TIMESTAMP</code> </p> </td> 
   <td colname="col2"> <p>Eine 10-stellige UTC- und Unix-Zeitstempel. </p> <p>Sie kann auch <code>als JJJMMTDHHMMSS formatiert werden, nachdem</code> Java-Datums-/Zeitstempelformatierungsregeln angewendet wurden. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Kopfzeilenfeldmakros {#header-field-macros}

Makros, die nur in Kopfzeilenfeldern verwendet werden. Beispiele finden Sie unter [Dateiformat-Makrobeispiele](../formats/file-format-examples.md).

<table id="table_1A8BD1750F4940B3A34E3F80371A447A"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Makro </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>TAB</code> </p> </td> 
   <td colname="col2"> <p>Dieses Makro wird als Trennzeichen verwendet und fügt eine Registerkarte zwischen Feldern ein. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Datenzeilenmakros {#data-row-macros}

Makros, die nur in Datenzeilen verwendet werden. Beispiele finden Sie unter [Dateiformat-Makrobeispiele](../formats/file-format-examples.md).

<table id="table_E378F94A3907407AA8110C8EE6C10909"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Makro </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>CLOSE_ CURLY_ BRACKET</code> </p> </td> 
   <td colname="col2"> <p>Fügt ein geschlossenes geschweifte Klammernzeichen ein. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>KOMMA</code> </p> </td> 
   <td colname="col2"> <p>Fügt ein Komma ein. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DP_ UUID</code> </p> </td> 
   <td colname="col2"> <p> <span class="term"> Unique Users-ID </span>des Datenpartners. Gibt die ID zurück, die Sie einem Benutzer/Site-Besucher zugewiesen haben, wenn diese ID bereits mit einer <span class="keyword"> Audience Manager </span> -Geräte-ID synchronisiert wurde. </p> <p>Wenn die DPID 0 ist, gibt dieses Makro die <span class="keyword"> Audience Manager </span> ID anstelle Ihrer ID für den Benutzer zurück. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DP_ UUID_ LIST</code> </p> </td> 
   <td colname="col2"> <p>Gibt eine Liste zurück, die mehrere IDs für einen Datenpartner enthält. Dies ist nützlich, wenn Sie eine große Organisation mit mehreren Unterteilungen oder anderen Organisationsgruppen haben, für die Sie Daten freigeben dürfen. Dieses Makro gibt eine Liste der IDs für diese untergeordneten Gruppen zurück. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DPUUIDS</code> </p> </td> 
   <td colname="col2"> <p>Die Ausgabe dieses Makros ordnet die Datenanbieter-ID (DPID) den eindeutigen Benutzer-IDs (DPUUID) zu. Dieses Makro muss über eine Formatierungszeichenfolge verfügen, um die Ausgabe zu steuern. Die Beispielausgabe würde wie folgt aussehen: </p> <p> <code>" dpids = dpid 1, dpid 2,… dpid n | maxmappings = n | format = json "</code> </p> <p>Mit der <code>Einstellung "maxmappings</code> " wird festgelegt, wie viele Zuordnungen das Makro zurückgeben soll. Wenn <code>maxmappings = 0</code>, gibt dieses Makro alle Zuordnungen für jede angegebene DPID zurück. Die Daten werden nach Zeitstempel sortiert (erster erster Wert) und gibt Ergebnisse mit dem größten Zeitstempel zurück. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>endif</code> </p> </td> 
   <td colname="col2"> <p>Erforderlich, wenn die Makros "Bedingung <code>«,"</code> <code>SEGMENT_ LIST</code> " und " <code>REMOVED_ SEGMENT_ LIST</code> " verwendet werden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>if (SEGMENT_ LIST &amp; &amp; REMOVED_ SEGMENT_ LIST) endif</code> </p> </td> 
   <td colname="col2"> <p>Diese Kombination von Makros erstellt eine bedingte Anweisung, in der die Segmente aufgeführt sind, zu denen die Benutzer gehören <i>und</i> aus denen entfernt wurden. Wenn beide Bedingungen nicht erfüllt sind oder keine Daten vorhanden sind, wird eine leere Zeichenfolge zurückgegeben. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>MCID</code> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Adobe Experience Cloud </span> ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>OPEN_ CURLY_ BRACKET</code> </p> </td> 
   <td colname="col2"> <p>Fügt ein öffnendes geschweifte Klammernklammernzeichen ein. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>OPT_ OUT</code> </p> </td> 
   <td colname="col2"> <p>Herabgestuft. Verwenden Sie nicht. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>OUTPUT_ ATTRIBUTE_ TYPE</code> </p> </td> 
   <td colname="col2"> <p>Herabgestuft. Verwenden Sie nicht. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>OUTPUT_ ATTRIBUTE_ VALUE</code> </p> </td> 
   <td colname="col2"> <p>Gibt <code>1</code> als statischer, hartkodierter Wert zurück. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>PID</code> </p> </td> 
   <td colname="col2"> <p>Partner-ID (PID). Die PID wird auf der Registerkarte <span class="wintitle"> Profil </span> in der Admin-Benutzeroberfläche angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_ SEGMENT_ LIST</code> </p> </td> 
   <td colname="col2"> <p>Gibt ggf. eine Liste von Segmenten zurück, die entfernt wurden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENT_ LIST</code> </p> </td> 
   <td colname="col2"> <p>Gibt eine Liste von Segmenten in einer Liste zurück. Akzeptiert die folgenden optionalen Variablen: </p> 
    <ul id="ul_B111AA0D6C18445598A1444B8B7E9325"> 
     <li id="li_8603B40229624856AF1FBC434DB8F16A"> <code>Segmentid</code>: Legacy-ID. Herabgestuft. <code>Verwenden Sie sid</code> (nur Kleinschreibung). </li> 
     <li id="li_1EF40DDCA3C5447586904CF021D8F912"> <code>csegid</code>: Legacy-ID. Herabgestuft. <code>Verwenden Sie sid</code> (nur Kleinschreibung). </li> 
     <li id="li_D85F0A5D16AE4DAFB55C17DBB35EA66E"> <code>sid</code>: Segment-ID. </li> 
     <li id="li_9BE103EFD8384464B46FAC00422431DB"> <code>type</code>: Gibt <code>5</code>, einen statischen hartkodierten Wert zurück, der Daten als Segmentdaten identifiziert. </li> 
     <li id="li_FE5049089F2944FA9DB9F9D546DBA167"> <code>alias</code>: Zuordnung des Segments. Herabgestuft. <code>Verwenden Sie sid</code> (nur Kleinschreibung). </li> 
     <li id="li_DD778AA2D1DB4D409CF5026B5D9DBD27"> <code>Lastupdatetime</code>: Ein Unix-Zeitstempel, der angibt, wann ein Segment zuletzt erstellt wurde. </li> 
    </ul> <p>Setzen Sie diese Variablen nach dem Makro in geschweifte Klammern. Dieser Code trennt beispielsweise die Ergebnisse durch einen senkrechten Strich "|" Zeichen: <code>&lt; SEGMENT_ LIST: {seg|&lt; seg. type &gt;, &lt; seg. sid &gt;}; separator = "|" &gt;</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SET_ ATTRIBUTE</code> </p> </td> 
   <td colname="col2"> <p>Gibt <code>1</code> als statischer, hartkodierter Wert zurück. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TAB</code> </p> </td> 
   <td colname="col2"> <p>Fügt einen Tabulator-Trennzeichen ein. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TRAIT_ LIST</code> </p> </td> 
   <td colname="col2"> <p>Gibt eine Liste mit Eigenschaften zurück. Akzeptiert die folgenden optionalen Argumente: </p> 
    <ul id="ul_757DEB56E4F849768468F3C166B0D171"> 
     <li id="li_859E1F4F21D645519F150DC512B3EB1A"> <code>type</code>: Eigenschaften, die durch eine numerische ID identifiziert werden. Diese Variable gibt Folgendes zurück: 
      <ul id="ul_C9839266783D42CCADAAC3FEA33BE4D7"> 
       <li id="li_6996A218E3F04EC3BC70032559DD87FC"> <code>10</code> , der eine DPM-Eigenschaft kennzeichnet (offline, von einem eingehenden Auftrag aufgelöst). </li> 
       <li id="li_831FF929BF50434C8804C13E5786DF79"> <code>3</code> der eine regelbasierte Eigenschaft (Echtzeit; über das <span class="wintitle"> DCS </span>umbenannt). </li> 
      </ul> </li> 
     <li id="li_E84D6BC80AEE4F10963C9882C4151ED4"> <code>Traitid</code>: Eigenschafts-ID. </li> 
     <li id="li_D30A849BA35248E6B9110FA3ADEFC332"> <code>Lastrealized</code>: Das letzte Mal, wenn die Eigenschaft realisiert wurde. Unix-Zeitstempel. </li> 
    </ul> <p>Setzen Sie diese Variablen nach dem Makro in geschweifte Klammern. Dieser Code trennt beispielsweise die Ergebnisse durch einen senkrechten Strich "|" Zeichen: <code>TRAIT_ LIST {type | traitid}; separator = "|"</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>UUID</code> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager </span> -Benutzer-ID. </p> </td> 
  </tr> 
 </tbody> 
</table>