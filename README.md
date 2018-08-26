# Technische Dokumentation
BärnHäckt 2018 - Smart City BFH Challenenge

## Ausgangslage
Da wir in unserer Challenge viel konzeptionell (siehe [Konzeptionelle Dokumentation](https://github.com/sspaeti/bfh-Hackathon-Open-City-Cargo/blob/master/Konzept.md)) gearbeitet haben, haben wir uns für die technische Umsetzung einen spezifischen Use Case ausgesucht, der im ganzen Prozess abgewickelt wird. Der Use Case ist aus Sicht eines Zustellers. Dieser kann in einer Web-App (Microsoft PowerApps) alle offenen Pakete einsehen und sich seine auswählen, welche er ausliefern möchte.
Da er seine Fahrzeuge hinterlegt hat, werden nur Pakete angezeigt, die seinen Dimensionen des Fahrzeugs entsprechen. 

Automatisch werden ihm Vergütungen entsprechend seiner Auswahl errechnet.

### Vergütungen
Die Vergütung wird nach Auslastung seines Fahrzeuges, CO2 Emission und Lärm berechnet. Falls er sich anbietet, Rücktransporte auf dem Weg zurück aufzunehmen, wird ihm je nach aktuellen offenen Paketen ein variabler Preis vergütet.

## Technische Grundsatzentscheide
Wir haben uns für Microsoft PowerApps mit SQL Server auf Azure entschieden, damit wir Backend und Frontend mit einer vorhandenen Internet-Verbindung von überall erreichen können. Zusätzlich ist die Lösung beliebig skalierbar falls wir viele Users in kurzer Zeit haben werden. PowerApps sind auch optimiert für Smartphones, Tablets und Notebooks out-of-the-box.

Die Lösung eignet sich vor allem für schnelles Prototyping. Für eine produktive Umgebung würden wir jedoch andere Technologien und Produkte in Erwägung ziehen.

## Implementation
- Die Karte wurde über Google Maps Static API implementiert.
- Die App ist auf Cloud-Lösungen basierend und einfach skalierbar. Die App ist einfach wartbar und mit Standard-Software von Microsoft PowerApps erstellt.
- Wir haben uns bewusst auf einen Use Case beschränkt, da es nicht möglich ist, eine ganze SmartCity Lösung umzusetzen und da das Hauptprodukt eine konzeptionelle Lösung ist.

## Aktueller Stand des Sourcecodes
- Source-code ist die Microsoft PowerApp, die als Export-Datei bereitsteht und die SQL-Tabellen als Script.
- Die SQL Tabellen wurden optimiert für die PowerApps und bewusst einfach und denormalisiert gehalten. Bei einer richtigen Applikation würde man dies normalisieren und die Datenbank optimiert erstellen.
- Link zum WebApp-Sourcecode: [Open City Cargo PowerApp](https://github.com/sspaeti/bfh-Hackathon-Open-City-Cargo/blob/master/Open%20City%20Cargo%20V1_1.msapp)
- [Power App Screenshots und Beschreibung](https://github.com/sspaeti/bfh-Hackathon-Open-City-Cargo/blob/master/PowerApp%20Description.md)


