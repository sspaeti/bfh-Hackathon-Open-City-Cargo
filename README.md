# Technische Dokumentation
BärnHäckt 2018 - Smart City BFH Challenenge

## Ausgangslage
Da wir in unserer Challenge viel Konzeptionell unterwegs waren, haben wir uns für die technische Umsetzung einen spezifischen Use Case ausgesucht der im ganzen Prozess abgewickelt werden. Der Use Case ist aus Sicht eines Zusteller. Dieser kann in einer Web-App (Microsoft PowerApps) alle offenen Pakete einsehen und sich seine Auswählen welche er ausliefern möchte.
Da er seine Fahrzeuge hinterlegt hat, werden nur Pakete angezeigt die seinen Dimensionen des Fahrzeugs entsprechen. 

Automatisch werden ihm Vergütungen entsprechend seiner Auswahl errechnet.

### Vergütungen
Die Vergütung wird nach Auslastung seines Fahrzeuges, CO2 Emission und Lärm berechnet. Falls er sich anbietet Rücktransporte auf dem Weg zurück aufzunehmen, wird ihm je nach aktuellen offenen Paketen einen variablen Preis vergütet.

Technische Grundsatzentscheide
Wir haben uns für Microsoft PowerApps mit SQL Server auf Azure entschieden, damit wir Backend und Frontend mit einer vorhandenen Internet-Verbindung von überall erreichen können. Zusätzlich ist die Lösung beliebend skalierbar falls wir viele Users in kurzer Zeit haben werden.

PowerApps sind auch optimiert für Smartphones, Tablets und Notebooks out-of-the-box.

## Implementation
- Google Maps Karte wurde über Google API implementiert, aufgrund der maximalen Map Aufrufe von 200 pro Tag haben wir die Bilder generiert und zeigen diese statisch an.
- Die App ist auf Cloud-Lösung und einfach skalierbar. Die App ist mit einfach Wartbar und mit standard Software von Microsoft PowerApps erstellt.
- Wir haben uns bewusst auf einen Use Case beschränkt, da es nicht möglich ist eine ganze SmartCity Lösung umzusetzen und das Hauptprodukt eine konzeptionellen Lösung ist.

## Aktueller Stand des Sourcecodes
- Source-code ist die Web-App als Microsoft PowerApps export und SQL Server Tabellen.
- Die SQL Tabellen wurden optimiert für die PowerApps und bewusst einfach und denormalisiert gehalten. Bei einer richtigen Applikation würde man dies normalisieren und Datenbank optimiert erstellen
Link zum WebApp Source code: [Open City Cargo PowerApp](https://github.com/sspaeti/bfh-Hackathon-Open-City-Cargo/blob/master/Open%20City%20Cargo%20V1_1.msapp)
- [Power App Screenshots und Beschreibung](https://github.com/sspaeti/bfh-Hackathon-Open-City-Cargo/blob/master/PowerApp%20Description.md)


