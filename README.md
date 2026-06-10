# IMCM-Mitschrift der 1BHK

Das ist das README.md File unseres Repositories. Die Dateienendung .md steht für Markdown - eine heute sehr weit verbreitete [Auszeichnungssprachen](https://de.wikipedia.org/wiki/Auszeichnungssprache). Weiter bekannte Auszeichnungssprachen sind:

- Hypertext Markup Language (HTML)
- Extensible Markup Language (XML)
- Yet Another Markup Language (YAML, YML)

> **Achtung!**
> Die Abkürzung ML steht nicht immer für _Markup Language_, sie kann auch _Machine Learning_ heißen.

## Playlist zur Funktionsweise des Internets

### Teil 1 - What is the Internet

- das Internet wurde in den 1970er-Jahren entwickelt
- Motivation: Schaffung eines dezentralen Netwerks, das auch nach einem Atomschalgs noch funktioniert (Kontext des Kalten Krieges)
- Funktionsweise: Paketvermittlung (_Packet Switching_) - Nachrichten bzw. Dateien werden in kleine Pakete aufgeteilt und unabhängig voneinander über das Netzwerk verschickt
- Internet: das Netz der Netze - besteht aus vielen kleineren Netzen unterschiedlicher Internetanbieter (_Internet Service Provider - ISP_, z.B. : Salzburg AG, Magenta, A1, ...)

### Teil 2 - The Internet: Wires, Cables and WiFi

Informationen werden im Internet als Bits übertragen. Bits haben zwei Werte: 0 und 1. 8 Bits zusammengefasst ergeben ein Byte. Mit einem Byte kann man 256 verschiedene Werte speichern (2^8).

Bits können über verschiedene Übertragungsmedien zwischen Computern versendet werden. Die Anzahl der übertragenden Bits pro Sekunde wird als **Brandbreite** bezeichnet. Bei einer Brandbreite von 300Mbit/s können beispielsweise 300 Millionen Bit pro Sekunde über die Leitung laufen. Übertragungsmedien können sein:

**1. Elektrizität / Kupferdraht (Ethernet)**

- billig
- einfach in der Verabeitung
- weit verbereitet
- hohe Verluste über mittlere und lange Distanzen (hunderte Meter)

**2. Licht / Glasfaserkabel**

- schnelle Übertragung
- verlustfrei
- geeignet für Ozeankabel
- teuer und schwierig in der Verarbeitung

**3 Funk / Radiowellen**

- hoher Komfort, Internet überall

### Teil 3 - The Internet: IP-Addresses & DNS

- Protokolle sind die Regeln der Kommunikation
- eines der wichtigsten Protokolle im Internet ist das Internet Protocol (IP)
- jedes Gerät im Internet hat zumindest eine (eindeutige) IP-Adresse, viele Geräte haben aber eine externe IP (ähnlich wie die Hausnummer) und eine internet IP (ähnlich wie die Raumnummer)
- das _Domain Name System_ (DNS) übersetzt menschenlesbare Domainnamen (z.b.: www.google.com) in IP-Adressen
- DNS-Server führen Tabellen mit Domainnamen und den entsprechenden IP-Adressen

### Teil 4 - The Internet: Packets, Routing & Relability

- Über das Internet versendete Daten werden in Pakete aufgeteilt
- einzelne PAkete haben eine Größe von 1,5kB. D.h. ein Foto mir einer Größe von 10MB wird in 6700 Pakete aufgeteiltm bevor es über das Internet versendet wird
- Pakete können untershciedliche Routen durch das Internet nehmen. Die Route wird je nach Auslastung, Störungen etc. durch spezielle Computer - die Router- dynamisch bestimmt
- jedes Paket enthäöt die Quell- und Ziel-IP_Adresse! sowie eine eindeutige Paketnummer
- das _Transmisssion Control Protocoll_ (TCP) prüft am Ziel, ob alle Pakete einer Übertragung angekommen sind, falls Pakete fehlen fordert es diese erneut vom vom Absender an.
  -TCP und IP bilden gemeinsam das Rückrat des Internet. Man spricht auch von einem IP/TPS Models.

### Teil 5 - The Internet : HTTP & HTML

- HTTP steht für _Hypertext Transport Protocol_. HTTP arbeitet nach dem CLient-Server-Prinzip:

  - ein Web-Client (Browser) sendet eine Anfrage (_request_) an einen Web-Server
  - der Web-Server verarbeitet die Anfrage und sendet eine Antwort (_response_) zurück. Die Antwort enthält u.a. einen sogennanten [HTTP-Statuscode](https://de.wikipedia.org/wiki/HTTP-Statuscode), der Auskunft über die Verarbeitung der Anfrage gibt.

  > ### HTTP-Statuscode
  >
  > - **1xx** - Die Anfrage dauert noch an
  > - **2xx** - Die Anfrage war erfolgreich
  > - **3xx** - Um- oder Weiterleitung
  > - **4xx** - Clientfehler (z.b. 404 - _Page not Found_)
  > - **5xx** - Serverfehler 💀🌹👿

- HTTP-Anfragen werden immer mit einer **HTTP-Methode** übertragen
- Date (HTML-Seiten, Bilder, Videos, ...) werden mit Get-Anfragen angefordert
- Benutzereingaben (z.b. aus Formularfeldern z.b. Passwort, Datei-Uploads, ...) werden mit POST-Anfragen verschlüsselt versendet.
- es gibt auch adnere HTTP-Methoden. Diese lernen wir aber erst später
- HTTP-Anfragen und Antworten können auch **Cookies** erhalten. Cookies sind kleine Textdateien, die aus Schlüssel-Wert-Paaren (_key-value-pairs_) bestehen. Sie werden bejder Anfrage vom Client mitgesendet und ermöglichen so u.a. die Identifikation einzelner Nutzer.

### Playlist zur Funktionsweise des Internets

[TCP-IP-Model](assets/https___miro.medium.com_v2_resize_fit_720_format_webp_1_g1GzSjM5-J3aN2wjVz6qKA.png)

### Teil 8 - The Internet: How Search Works

- Suchmaschinen-Bots (_Crawler_) durchstreichen ständig das WWW und katalogisieren Websites. Der entstehende Katalog wird auch **Index** genannt.
- Wenn wir einen Suchbegriff bei Google (oder einer anderen _Search Engine_) eingeben, wird NICHT das WWW dursucht, sondern lediglisch der zuvor erstellte Index
- Suchergebnisse werdenauf Basis eines (geheimen) Algorithmus geranked - Ergebnisse, die weiter oben stehen, werden öfter angeklickt
- Einfluss auf das Ranking haben u.a.:
  - im Text vorkommende Suchbegriffe (_Keywords_)
  - Links die auf meine Seite zeigen (_Blacklinks_)
- Die Suchergebnisse werden an die Benutzer*innen angepasst! D.h. nicht jede/r sieht die gleichen Informationen, selbst wenn sie idente Suchanfragen durchführen! -[Startpage] (https://www.startpage.com/de/) ist eine datensparsame Suchmaschine, die ihren Benutzer*innen die Verwendung von Google ohne Tracking oder Personalisierung erlaubt
