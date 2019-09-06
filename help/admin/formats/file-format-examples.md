---
description: Beispiele für die Verwendung von Makros zum Erstellen ausgehender FTP-Dateivorlagen.
seo-description: Beispiele für die Verwendung von Makros zum Erstellen ausgehender FTP-Dateivorlagen.
seo-title: Beispiele für Dateiformat-Makros
title: Beispiele für Dateiformat-Makros
uuid: f 00 d 431 d -7 e 33-457 a-b 633-c 79 cbc 4 c 8 f 10
translation-type: tm+mt
source-git-commit: 4c6d1752ff10d2d3d12cab88e823f25f5ef4fcd0

---


# Beispiele für Dateiformat-Makros {#file-format-macro-examples}

Beispiele für die Verwendung von Makros zum Erstellen ausgehender [!DNL FTP] Dateivorlagen.

>[!NOTE]
>
>In den Tabellen identifiziert **Fettschrift** jedes Makro mit der zugehörigen Ausgabe. Für die Formatbeispiele wurden die Symbole &lt; &gt; Symbole hinzugefügt, um jedes Makro visuell zu trennen.

## Häufige Makros {#common-macros}

Diese Makros können in jedem beliebigen Format verwendet werden. Eine vollständige Liste und Definitionen finden Sie unter [Dateiformat-Makros](../formats/file-formats.md) .

<table id="table_B5073597219B470298EE614902DACAE8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Makro </th> 
   <th colname="col2" class="entry"> Format- und Ausgabebeispiele </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>DPID </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Ausgabe: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>MASTER_ DPID </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; MASTER_ DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Ausgabe: <code>ftp_ 215_ 888_ 20915_ iter_ 1449756724. sync </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>ORDER_ ID </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Ausgabe: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SYNC_ MODE </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Ausgabe: 
     <ul id="ul_F63D7B78AF1246639D6ED85C1621B17C"> 
      <li id="li_4D0D7B4D047345FE861FCBA2BD0408ED">Voll: <code>ftp_ 215_ 888_ full_ 1449756724. sync </code> </li> 
      <li id="li_23F4D1F6B2784E599EDA29AA457327E6">Inkrementell: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SYNC_ TYPE </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Ausgabe: 
     <ul id="ul_11B14E740E40474F8302BDB809C428FE"> 
      <li id="li_54A3EAA468B44AC8B2528F855E03D04B">FTP: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </li> 
      <li id="li_93468C56B661463CA7F62B1F5D3A53FF">https: <code>http_ 215_ 888_ iter_ 1449756724. sync </code> </li> 
      <li id="li_8A204C7BEDBC41C096FE953B5F827DEC">S 3: <code>s 3_ 215_ 888_ iter_ 1449756724. sync </code> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TIMESTAMP </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; SYNC_ TYPE &gt;_ &lt; ORDER_ ID &gt;_ &lt; DPID &gt;_ &lt; SYNC_ MODE &gt;_ &lt; TIMESTAMP &gt;. sync </code> </p> <p>Ausgabe: <code>ftp_ 215_ 888_ iter_ 1449756724. sync </code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Kopfzeilenfeldmakros {#header-field-macros}

Makros, die nur in Kopfzeilenfeldern verwendet werden. Eine vollständige Liste und Definitionen finden Sie unter [Dateiformat-Makros](../formats/file-formats.md) .

<table id="table_ABC31B3D660D47969E111EBC734D5BBC"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Makro </th> 
   <th colname="col2" class="entry"> Format- und Ausgabebeispiele </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>TAB </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; ORDER_ ID &gt; &lt; TAB &gt; &lt; SYNC_ TYPE &gt; </code> </p> <p>Ausgabe: <code>888 full. sync </code> </p> <p>In der Ausgabe trennt das nicht druckbare Tabulatorzeichen jedes Element. </p> </td>
  </tr>
 </tbody>
</table>

## Datenzeilenmakros {#data-row-macros}

Makros, die nur in Kopfzeilenfeldern verwendet werden. Eine vollständige Liste und Definitionen finden Sie unter [Dateiformat-Makros](../formats/file-formats.md) .

<table id="table_408C6DD2B9D54550B003EAC93562E64F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Makro </th> 
   <th colname="col2" class="entry"> Format- und Ausgabebeispiele </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>DP_ UUID </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; DP_ UUID &gt; &lt; TAB &gt; &lt; DP_ UUID_ LIST; separator = TAB &gt; </code> </p> <p>Ausgabe: <code>123456 UUID 1 UUID 2 UUID 3 </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DP_ UUID_ LIST </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; DP_ UUID &gt; &lt; TAB &gt; &lt; DP_ UUID_ LIST; separator = TAB &gt; </code> </p> <p>Ausgabe: <code>123456 UUID 1 UUID 2 UUID 3 </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENT_ LIST &amp; &amp; REMOVED_ SEGMENT_ LIST </code> </p> </td> 
   <td colname="col2"> <p>In diesem Beispiel wird ein Format erstellt, das entfernte Segmente in einem Server-zu-Server-Feed zurückgibt. </p> <p> 
     <code>{"Advertiserid": " &lt; PIDALIAS &gt; "," datacenterid ": 2, "TDID": " &lt; DP_ UUID &gt; ", 
 " Daten" : [&lt; SEGMENT_ LIST: {seg|&lt; OPEN_ CURLY_ BRACKET &gt; "Name": " &lt; seg. alias &gt; " &lt; CLOSE_ CURLY_ BRACKET &gt;}; 
 separator = "," &gt; &lt; if (SEGMENT_ LIST &amp; &amp; REMOVED_ SEGMENT_ LIST) &gt; &lt; COMMA &gt; &lt; endif &gt; 
 &lt; REMOVED_ SEGMENT_ LIST: {seg|&lt; OPEN_ CURLY_ BRACKET &gt; "Name": " &lt; seg. alias &gt; ", 
 " Ttlinminutes" : 0 &lt; CLOSE_ CURLY_ BRACKET &gt;}; separator = "," &gt;]} </code>
  </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENT_ LIST </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; DP_ UUID &gt; &lt; SEGMENT_ LIST &gt;; separator = "" &gt; </code> </p> <p>Ausgabe: <code>123456 105955 101183 101180 101179 </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SET_ ATTRIBUTE </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; TID &gt; &lt; TAB &gt; &lt; TAB &gt; &lt; DP_ UUID &gt; &lt; TAB &gt; &lt; SET_ ATTRIBUTE &gt; &lt; TAB &gt; &lt; OPT_ OUT &gt; &lt; TAB &gt; &lt; SEGMENT_ LIST: &lt; TAB &gt; &lt; SEGMENT_ LIST: {seg|&lt; seg. type &gt;, &lt; seg. alias &gt;, &lt; OUTPUT_ ATTRIBUTE_ VALUE &gt;, &lt; seg. lastupdatetime &gt; &amp;} &gt; </code> </p> <p>Ausgabe: <code>1159 000880085796836537415162975097709717335000 17 t 0 aj 01 b 120 hp 1 0 5,103714,1,1344110 00 &amp; 5,103713,1,134325061000 </code> </p> </td>
  </tr>
  <tr> 
   <td colname="col1"> <p> <code>TAB </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; DP_ UUID &gt; &lt; TAB &gt; &lt; DP_ UUID_ LIST; separator = TAB &gt; </code> </p> <p>Ausgabe: <code>123456 UUID 1 UUID 2 UUID 3 </code> </p> <p>In der Ausgabe trennt das nicht druckbare Tabulatorzeichen jedes Element. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TRAIT_ LIST </code> </p> </td> 
   <td colname="col2"> <p>Format: <code>&lt; PID &gt; &lt; TAB &gt; &lt; DP_ UUID &gt; &lt; TAB &gt; &lt; SET_ ATTRIBUTE &gt; &lt; TAB &gt; &lt; TRAIT_ LIST; separator = "|» &gt; </code> </p> <p>Ausgabe: <code>1131 12345 1 123|456|789 </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
