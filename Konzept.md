# Konzept
BärnHäckt 2018 - Smart City BFH Challenenge


## Die Vision
Direkte Transporte in die Innenstadt werden unterbunden, die Feinverteilung den Spezialisten überlassen . Dadurch gibt es im Stadtzentrum weniger Verkehr und mehr Lebensqualität.

![alt text](https://github.com/sspaeti/bfh-Hackathon-Open-City-Cargo/blob/master/screenshots/skizze%20Open%20City%20Cargo.jpg)

## Nötige Massnahmen
Die Stadt sichert sich auf Gesetzesebene das Recht, die Logistik in problematischen Perimeter zu kontrollieren. Die Stadt muss eine Infrastruktur aufbauen, um die Logistik optimiert abzuwickeln.
Sie betreibt HUBs rund um den Innenstadt-Perimeter und stellt das Management der Sendungen sicher.
Sie konzessioniert und zertifiziert Transport-Dienstleiter.

## Teilnehmer
- Versandhäuser und Online-Shops
- Zulieferer von Geschäften und KMUs
- nationale und internationale Transport-Dienstleiter
- lokale Transportdienstleister, Velokuriere, Taxiunternehmen
- Privatkunden und Gewerbetreibende im Stadt-Perimeter
- Polizei und Verkehrsleitzentrale

## Ziele
Nicht ökologische und verkehrsbehindernde Transporte (insbesondere LKW) werden besteuert -
ökologische Transportsysteme hingegen werden mit einem Bonussystem belohnt.

## Umfang und Vorteile
- Optimierte Transporte durch Konsolidierung/Entflechtung bei den HUBs
- Dynamische Steuerung der Transportwege aufgrund von geplanten oder aktuellen Gegebenheiten
  - Verkehrsstörungen, Baustellen, Stau, Sperrungen
  - Ökologische und ökonomische Gegebenheiten
  - Ausfall von Kapazitäten bei Logistikern
- Sendungen werden einheitlich ausgezeichnet und getrackt
- Beteiligte Parteien haben jederzeit Zugang zu Routing-/Tracking-Infos
- Automatische oder Persönliche Quittierung des Empfängers
  - RFID-Tags an Briefkästen oder Quittierung des Empfangs per Device mit NFC

## Bonus-Malus-System
- Leerfahrten (pain) und Fahrten mit schlechter Auslastung werden bestraft (tiefere Vergütung).
- Ökologische und Lärmarme Fahrzeuge wie Elektromobile werden mit höheren Vergütungen belohnt.
- Bietet sich ein Zusteller an, Rücktransporte von Paketen zum HUB oder Direktlieferungen innerhalb des Perimeters vorzunehmen, wird er durch eine Pauschale belohnt. Diese Pauschale ist variabel. So kann gesteuert werden, wie viele "Pickup-Zusteller" für Zeitnahe Paketaufnahmen (z.B. Pizza-Lieferung) jeweils bereitstehen. Will ein Zusteller am Abend eine letzte Tour machen und dann in den Feierabend, kann er auf Rücktransporte verzichten.
- Die Stadt kann Anlässe wie ein Stadtfest im Portal registrieren und den Liefer-Verkehr durch in dieser Zeit erhöhte Preise eindämmen.
- Werden Pakete zu "Ladenhütern" (niemand will diese zustellen, da zu schwer, zu weit weg etc.) wird die Vergütung für dieses Paket durch das System schrittweise erhöht, damit der Auftrag doch noch angenommen wird und die Lieferfrist eingehalten wird.

## Regeln/Gesetze
- Optional können Regeln wie aktive Verbote für Verbrennungsmotoren durch die Stadt in der Plattform erfasst werden.

## Kundenkonto auf Open City Cargo
 - Kunden können verschiedene Lieferadressen in zentralem Portal erfassen. Diese müssen somit nur einmal erfasst werden. Adressen würden an Zulieferer weitergegeben und entsprechend auf Navigation angezeigt.
 - Es können auch mehrere Lieferadressen erfasst werden wie Geschäft, Home und Grosseltern. Das Kundenportal zeigt einem automatisch die günstigste Lieferung und somit auch die ökologischste Adresse an.
 - Gewünschter Lieferzeitpunkt wählen optimiert auf die Umwelt. Falls an Tagen an denen Zulieferer freien Platz auf Autos haben, können diese ökologisch und preisgünstiger angeboten werden. In Rushhours wo viele Pakete ausgeliefert werden und evtl. Extra-Fahrten für einzelne Pakete gemacht würden, ist der Preis dementsprechend teurer.

## Eingesetzte Technologien
- Blockchain
  - Versandkette des Pakets nachvollziehbar und unveränderbar dokumentieren
  - Vergütung könnte optional über Crypto Währung ausbezahlt werden
- IoT - Internet of Things
  - Per RFID können die Pakete identifiziert und geleitet werden und zu jederzeit getrackt werden im welchen Fahrzeug diese sich gerade befinden plus ausgelieferte Zeit kann errechnet werden.
- Open Government Data
  - Die gesperrten Perimeter einer Stadt, die Positionen der Hubs, die Regeln und Tarife der Vergütung sowie die Veranstaltungen einer Stadt werden als Open Government Data bereitgestellt. Dies ermöglicht Firmen und Drittanbietern mittels API darauf zuzugreifen. Eine mögliche Anbindung wäre die Plattform CPaaS.io.
- What3words
  - Weltweites Adresssystem, welches in einfacher Art in 3 m x 3 m Quadrate aufgeteilt und jedem dieser Quadrate eine einmalige 3-Wörter-Adresse zugeordnet. So kann jeder jeden Ort präzise auffinden und die Adresse schneller, einfacher und eindeutiger als in jedem anderen System weitergeben. 
  - Der Vorteil dieser Technologie ist, dass die Auslieferung exakt an den Wareneingang geliefert werden kann und der Bote nicht unnötig viel Zeit und Weg benötigt bei grossen Gebäuden, bei denen die Hausnummer allein nicht präzise genug ist.
  - Diese Adresse würde bei der Registrierung der Adressen in unseren Open City Cargo Plattform gleich erfasst mit einer API zu https://map.what3words.com/
- Microsoft PowerApps
  - Einfache Erstellung eines Prototyps optimiert für Geschäfts-Apps, und Einbindung in existierende Prozesse.
  - Mehr dazu in der Technischen Dokumentation (https://github.com/sspaeti/bfh-Hackathon-Open-City-Cargo)
  
