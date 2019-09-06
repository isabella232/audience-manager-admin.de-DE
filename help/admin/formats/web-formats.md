---
description: Listet die Makros auf, mit denen Sie HTTP-Datendateien erstellen können. HTTP sendet Daten in einem JSON-Format.
seo-description: Listet die Makros auf, mit denen Sie HTTP-Datendateien erstellen können. HTTP sendet Daten in einem JSON-Format.
seo-title: HTTP-Format-Makros
title: HTTP-Format-Makros
uuid: 91021 f 60-75 d 0-4 b 1 d -86 ca -91 c 9 dadafac 1
translation-type: tm+mt
source-git-commit: 1a547e421346a6bf281e2b3ff3a0bcb5cf1d78df

---


# HTTP-Format-Makros {#http-format-macros}

Listet die Makros auf, mit denen Sie Datendateien erstellen [!DNL HTTP] können. [!DNL HTTP] sendet Daten in einem [!DNL JSON] Format.

Eine Liste und Beispiele für häufig verwendete Makrokombinationen finden Sie im [HTTP-Format Makro-Beispiele](../formats/web-format-examples.md) .

<table id="table_72A72EA63C3643FB84B47A76CD2CC1CA"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Makro </th> 
   <th colname="col2" class="entry"> Methodentyp </th> 
   <th colname="col3" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>AAM_ UUID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p> <span class="keyword"> Audience Manager </span> -ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DP_ UUID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Eindeutige Benutzer-ID des Datenpartners. Dieses Makro gibt die ID zurück, die Sie einem Benutzer zugewiesen haben, wenn ihre ID bereits mit einer <span class="keyword"> Audience Manager </span> -Geräte-ID synchronisiert wurde. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DPID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Datenanbieter-ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>ECID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Datenanbieter-ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>GENERATION_ TIME</code> </p> </td> 
   <td colname="col2"> <p> <code>GET, POST</code> </p> </td> 
   <td colname="col3"> <p>Unix UTC timestamp. Ein interner Zeitstempel stellt den Zeitpunkt dar, an dem AAM benachrichtigt wurde, um das <span class="wintitle"> S 2 S </span> -Ziel unseren Partnern zu veröffentlichen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>IP</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Die IP-Adresse des Benutzers. </p> </td> 
  </tr>
    <tr> 
   <td colname="col1"> <p> <code>MCID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Experience Cloud-ID. (MCID steht für die Marketing Cloud, der alte Name der Experience Cloud) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>NUM_ REMOVED_ SEGMENTS</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Die Anzahl (Ganzzahl) von Segmenten, zu der ein Benutzer nicht mehr gehört. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>NUM_ SEGMENTS</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Die Anzahl der Segmente, zu denen ein Benutzer gehört. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>ORDER_ ID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET, POST</code> </p> </td> 
   <td colname="col3"> <p>Bestell- oder Ziel-ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>PID_ ALIAS</code> </p> </td> 
   <td colname="col2"> <p> <code>GET, POST</code> </p> </td> 
   <td colname="col3"> <p>Ein Alias für die Partner-ID. Auch als Foreign Account ID bekannt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>RANDOM</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Generiert eine zufallszahl. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REGION_ ID_ LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Der <a href="https://docs.adobe.com/help/en/audience-manager/user-guide/api-and-sdk-code/dcs/dcs-api-reference/dcs-regions.html"> Audience Manager-DCS-Bereich </a> , in dem die Aktivität erstellt wurde.</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_ SEGMENT_ LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Gibt ggf. eine Liste der Segment-IDs zurück, für die ein Benutzer nicht mehr qualifiziert ist. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_ SEGMENTS</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Eine Liste von Segmenten, für die sich ein Benutzer nicht mehr qualifiziert. Sie können auch bestimmte Segmentfelder zurückgeben, die Folgendes beinhalten: </p> <p> 
     <ul id="ul_29B83093A7624A908F0C06F2A248981A"> 
      <li id="li_57A60A54F5D44E38ACB4E2648095F246"> <code>Traitalias</code> </li> 
      <li id="li_4079F646493F40DBA0CE75D662A69454"> <code>Legacysegmentid (früher segmentid)</code> </li> 
      <li id="li_D3509A2D379E4C1FB3BC1B5E7D45A916"> <code>Newsegmentid</code> </li> 
      <li id="li_EA901C20EEEB4CFAA39A5E0E822D2394"> <code>status</code> </li> 
      <li id="li_6310E21F88CC4691980DD3C9D551409F"> <code>Datetime</code> </li> 
     </ul> </p> <p>Geben Sie diese Felder in einem Array wie im folgenden Beispiel an: </p> <p> <code>[&lt; REMOVED_ SEGMENTS: {seg|&lt; OPEN_ BRACKET &gt; "Mapping": &lt; seg. traitalias &gt;, "Status: " &lt; seg. status &gt;, "Time": &lt; seg. datetime &gt;, "legacysegmentid": &lt; seg. legacysegmentid &gt;, "newsegmentid": &lt; seg. newsegmentid &gt; &lt; CLOSE_ BRACKET &gt;}; " separator = "," &gt;]</code> </p> <p>Siehe auch Makrobeispiele für <a href="../formats/web-format-examples.md#reference_98828E32B0964FF9AAC7C5400E88BA31"> HTTP-Format </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_ TIME_ LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> Eine Liste der letzten Veralerungen für Segmente, für die der Benutzer nicht mehr qualifiziert ist. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_ TRAITALIAS_ LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Eine Liste der Segmentnamen von Segmenten, für die sich ein Benutzer nicht mehr qualifiziert. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENT_ LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Gibt eine Liste mit Segment-IDs zurück. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENTE</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Eine Liste von Segmenten, für die sich ein Benutzer qualifiziert. Sie können auch bestimmte Segmentfelder zurückgeben, die Folgendes beinhalten: </p> <p> 
     <ul id="ul_9209683A8E0A4B8081E5EFA4602F743F"> 
      <li id="li_D796526C1C9E45BEA891D619539888C4"> <code>Traitalias</code> </li> 
      <li id="li_BF12E010E1AD432C84605B9817F209DD"> <code>Legacysegmentid (früher segmentid)</code> </li> 
      <li id="li_4A81E3B715254549B9EADB983A2FC32B"> <code>Newsegmentid</code> </li> 
      <li id="li_1F01A60829DF4C87879D94299E1D589C"> <code>status</code> </li> 
      <li id="li_E52F10CD5A04487D81A4B1750B0DC4E3"> <code>Datetime</code> </li> 
     </ul> </p> <p>Geben Sie diese Felder in einem Array wie im folgenden Beispiel an: </p> <p> <code>[&lt; SEGMENTS: {seg|&lt; OPEN_ BRACKET &gt; "Mapping": &lt; seg. traitalias &gt;, "Status: " &lt; seg. status &gt;, "Time": &lt; seg. datetime &gt;, "legacysegmentid": &lt; seg. legacysegmentid &gt;, "newsegmentid": &lt; seg. newsegmentid &gt; &lt; CLOSE_ BRACKET &gt;}; " separator = "," &gt;]</code> </p> <p>Siehe auch Makrobeispiele für <a href="../formats/web-format-examples.md#reference_98828E32B0964FF9AAC7C5400E88BA31"> HTTP-Format </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TIME_ LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Eine Liste der letzten Realizationen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TIMESTAMP</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Unix, UTC Timestamp. Stellt die letzte Neualisierung des Segments dar. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TRAITALIAS_ LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Eine Liste mit Aliasnamen für ein bestimmtes Segment. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>USER_ AGENT</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Benutzeragent der ersten Anforderung. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>USER_ LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>POST</code> </p> </td> 
   <td colname="col3"> <p>Eine Liste der <span class="keyword"> Benutzer-IDs von </span> Audience Manager. Sie können auch bestimmte Felder zurückgeben, die Folgendes beinhalten: </p> 
    <ul id="ul_B6857D809FDC46749B7E745BD8C45F8E"> 
     <li id="li_F31CD82D16ED41FD82518141D90B5B35"> <code>user. aamuuid</code> </li> 
     <li id="li_623FA758C84D4A2D9B25C7FBE90F62B7"> <code>user. dpuuid</code> </li> 
     <li id="li_976B941908EB494EB476B5FB68B8972D"> <code>user. segments</code> </li> 
     <li id="li_D7E129833D1E4D59A554FFCE353924EE"> <code>user. removedsegments</code> </li> 
     <li id="li_8B3DD69D3FE3493492FC9F162812FCD5"> <code>user. useragent</code> </li> 
     <li id="li_8C7EA05585A64141876DF169C31322FE"> <code>user. ip</code> </li> 
     <li id="li_678076A31A7743C480F718C9E7A07E99"> <code>user. dpuuids</code> </li> 
     <li id="li_B598A5AED28C4304972E51DBD4E480D8"> <code>user. timestamp</code> </li> 
     <li id="li_8424D540282F449CA5AF6B3CC343DDCB"> <code>user. random</code> </li>
     <li><code>user. regions regionIds</code></li> 
    </ul> <p>Geben Sie diese Felder wie im folgenden Beispiel an: </p> <p> 
     <codeblock>
       " AAM_ UUID ": " &lt; user. aamuuid &gt; "datapartner_ 
UUID": " &lt; user. dpuuid &gt; " 
     </codeblock> </p> <p>Ein vollständiges Beispiel finden Sie unter <a href="../formats/web-format-examples.md#reference_98828E32B0964FF9AAC7C5400E88BA31"> auch Makrobeispiele </a> für HTTP-Format. </p> </td> 
  </tr>
 </tbody>
</table>