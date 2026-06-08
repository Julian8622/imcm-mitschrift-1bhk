# IMCM-Mitschrift der 1BHK

Das ist das README.md File unseres Repositories. Die Dateienendung .md steht für Markdown - eine heute sehr weit verbreitete [Auszeichnungssprachen](https://de.wikipedia.org/wiki/Auszeichnungssprache). Weiter bekannte Auszeichnungssprachen sind:

- Hypertext Markup Language (HTML)
- Extensible Markup Language (XML)
- Yet Another Markup Language (YAML, YML)

> **Achtung!**
 Die Abkürzung ML steht nicht immer für *Markup Language*, sie kann auch *Machine Learning* heißen.

## Playlist zur Funktionsweise des Internets


### Teil 1 - What is the Internet

- das Internet wurde in den 1970er-Jahren entwickelt
- Motivation: Schaffung eines dezentralen Netwerks, das auch nach einem Atomschalgs noch funktioniert (Kontext des Kalten Krieges)
- Funktionsweise: Paketvermittlung (*Packet Switching*) - Nachrichten bzw. Dateien werden in kleine Pakete aufgeteilt und unabhängig voneinander über das Netzwerk verschickt
- Internet: das Netz der Netze - besteht aus vielen kleineren Netzen unterschiedlicher Internetanbieter (*Internet Service Provider - ISP*, z.B. : Salzburg AG, Magenta, A1, ...)

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
- das *Domain Name System* (DNS) übersetzt menschenlesbare Domainnamen (z.b.: www.google.com) in IP-Adressen
- DNS-Server führen Tabellen mit Domainnamen und den entsprechenden IP-Adressen

### Teil 8 -  The Internet: How Search Works

- Suchmaschinen-Bots (*Crawler*) durchstreichen ständig das WWW und katalogisieren Websites. Der entstehende Katalog wird auch **Index** genannt.
- Wenn wir einen Suchbegriff bei Google (oder einer anderen *Search Engine*) eingeben, wird NICHT das WWW dursucht, sondern lediglisch der zuvor erstellte Index
- Suchergebnisse werdenauf Basis eines (geheimen) Algorithmus geranked - Ergebnisse, die weiter oben stehen, werden öfter angeklickt
- Einfluss auf das Ranking haben u.a.:
    - im Text vorkommende Suchbegriffe (*Keywords*)
    - Links die auf meine Seite zeigen (*Blacklinks*)
- Die Suchergebnisse werden an die Benutzer*innen angepasst! D.h. nicht jede/r sieht die gleichen Informationen, selbst wenn sie idente Suchanfragen durchführen!