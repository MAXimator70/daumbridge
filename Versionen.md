# Versionen

## 0.9.3 (Build 29) - 13.11.2026
- Neu: Pulsgurt suchen – findet Gurte direkt, ohne Kopplung in den Android-Einstellungen (viele Gurte lehnen die Kopplung ab)
- Nicht gekoppelte Gurte werden beim Start automatisch gesucht und verbunden

## 0.9.1 (Build 27) - 12.11.2026
- Neue Download-Adresse: github.com/MAXimator70/daumbridge (Update-Pruefung angepasst)

## 0.9.0 (Build 26) - 12.11.2026
- Logo antippen: dreht sich wie ein Schild und zeigt ein Diagramm (Leistung, Kadenz, Puls)
- Diagramm mit dem Finger zurueckblaettern, Doppeltipp springt wieder auf live
- Beim Start wird automatisch das Diagramm gezeigt

## 0.8.1 (Build 25) - 12.11.2026
- Entwicklername in der App durch das Pseudonym Wing-Art ersetzt

## 0.8.0 (Build 24) - 11.11.2026
- Neue Kopfzeile ohne graue Leiste: runde Knoepfe fuer Hell/Dunkel und Menue
- Rundes Menue mit Symbolen
- Einstellungen und Pulszonen mit Zurueck-Knopf, neuer Bereich App (Update, Info)
- Alle Auswahlfenster als runde Karten
- Hinweis zur PIN: manche Adapter koppeln ohne PIN

## 0.7.2 (Build 23) - 11.11.2026
- Streifen Zeit in Pulszonen immer sichtbar, fuellt sich in der ersten Stunde
- Neue graue Zone: Puls unter Erholung

## 0.7.1 (Build 22) - 11.11.2026
- Pulszonen: Ruhepuls und Maximalpuls mittig, mit Trennlinie

## 0.7.0 (Build 21) - 11.11.2026
- Fahrerprofile (Geburtsdatum, Gewicht, FTP, Pulsgurt, Pulszonen)
- Pulszonen selbst einstellbar oder automatisch berechnet
- Puls- und Leistungskachel in Zonenfarben, Balken Zeit in Pulszonen
- Zusammenfassung nach dem Training
- Verbindet sich bei Abbruch selbst neu (Daum und Pulsgurt)
- Neues Einstellungsmenue mit Drehraedern, SIM-Staerke heisst jetzt Simulatorstaerke
- Stopp-Knopf grau

## 0.6.1 (Build 20) - 11.11.2026
- Smart-Knopf farbig: gruen = EIN, rot = AUS

## 0.6.0 (Build 19) - 11.11.2026
- ANT+ entfernt, DaumBridge sendet nur noch per Bluetooth
- Umschalter Hell/Dunkel auf der Startseite

## 0.5.0 (Build 18) - 11.11.2026
- Gangschaltung entfernt: die Leistung wird am Daum selbst geregelt
- Neue Kachel "Kadenz" (Trittfrequenz in U/min) statt "Gang"
- Lautstaerketasten werden nicht mehr zum Schalten verwendet

## 0.4.1 (Build 17) - 11.11.2026
- Texte ueberarbeitet

## 0.4.0 (Build 16) - 11.11.2026
- Name "DaumBridge" steht jetzt im Haupt-Werbepaket, damit ihn auch Zwift/MyWhoosh am Windows-Laptop anzeigen (statt z. B. "POWER-4874")
- Bluetooth-Name maximal 15 Zeichen

## 0.3.9 (Build 15) - 11.11.2026
- Bluetooth-Pulsgurt (z. B. Polar H9): Einstellungen > Fitness > Pulsgurt. Der Puls kommt dann vom Gurt statt vom Daum und wird an Zwift/MyWhoosh weitergegeben
- Anzeige "Puls" oben neben Daum/ANT+/BT, wenn ein Gurt gewaehlt ist

## 0.3.8 (Build 14) - 11.11.2026
- Erscheint in Zwift, MyWhoosh & Co. als "DaumBridge" (Name in den Einstellungen aenderbar)
- Absturzberichte aelterer Versionen werden nach einem Update verworfen

## 0.3.7 (Build 13) - 10.11.2026
- Absturz beim Start behoben (Anzeige % FTP in der Leistungskachel)
- Anzeige-Fehler koennen die App nicht mehr beenden

## 0.3.6 (Build 12) - 10.11.2026
- Absturzbericht erscheint in einem eigenen Bildschirm, der nicht mehr mit geschlossen wird

## 0.3.5 (Build 11) - 10.11.2026
- Absturzbericht: Nach einem Absturz zeigt DaumBridge beim naechsten Start den Fehler an und kann ihn teilen
- Bluetooth- und ANT+-Start abgesichert, Berechtigung fuer Bluetooth-Senden wird geprueft
- Neuere Android-Versionen: Inhalt nicht mehr unter der Statusleiste

## 0.3.4 (Build 10) - 09.11.2026
- Info: Entwickler ergänzt
- Neue Installationen starten mit Verbindung Bluetooth

## 0.3.3 (Build 9) - 09.11.2026
- Startseite: Auswahl der Verbindung ANT+ / Bluetooth / Beide, die aktive Verbindung ist immer sichtbar
- Einstellungen: ANT+ FE-C / BLE FTMS als eine Auswahl

## 0.3.2 (Build 8) - 09.11.2026
- Einstellungen neu geordnet: Ergometer, Fitness, Smarttrainer, Simulationsdaten, Experten
- Neu: FTP-Einstellung, Leistung zusaetzlich in % FTP
- Neu: Menue Verbindungen (Daum, ANT+, Bluetooth auf einen Blick)
- Protokoll kann geteilt werden (Mail, Messenger)

## 0.3.1 (Build 7) - 09.11.2026
- Automatisches Update wie bei MaxBike: Pruefung beim Start, Download und Installation aus der App
- Menue: Nach Update suchen

## 0.3.0 (Build 6) - 09.11.2026
- Daum 8008: vollstaendiger Startablauf (Reset, Init, Programm, Personendaten), robusteres Lesen, bis 800 W
- Leistung abhaengig von der Trittfrequenz begrenzt, Mindestleistung nur beim Treten, Abfrage alle 250 ms
- Schalter fuer alte Daum-Firmware (vor 12/2003)
- Schaltung als sortierte Gangliste (+-1 / +-4 Gaenge), ohne virtuelle Schaltung werden die Daum-Gaenge geschaltet
- SIM: Luftwiderstand korrigiert, Steigung geglaettet; ERG: Tempo aus der Leistung
- Bluetooth: Daten gehen nicht mehr verloren, Wattbereich 25-800 W in 1-W-Schritten, eigener Puls-Sensor, Steigungsvorgabe
- ANT+: neuer Sensor Tempo/Trittfrequenz (1305), Antwort auf Kalibrier-Anfrage

## 0.2.3 (Build 5) - 09.11.2026
- Farben an das Logo angepasst: Logo-Gruen als Akzent (Start, Modus, Gang, Schaltung, Einstellungen)
- Logo auf hellgrauer Karte mit Mint-Rand

## 0.2.2 (Build 4) - 09.11.2026
- Neues Logo 'DaumBridge by Wing-Art' in der App und auf der Download-Seite
- Neues App-Symbol mit dem Daum aus dem Logo

## 0.2.1 (Build 3) – 09.11.2026
- Neues App-Symbol: Daum-Ergometer im Stil von MaxBike

## 0.2.0 (Build 2) – 09.11.2026
- Neue Oberfläche (Dauer, Steigung/Modus/Gang, Tempo/Strecke/Puls/Leistung, Smart, Start, Schaltung)
- Einstellungen: Ergometer, Übertragung, Schaltung, Simulation, Experten
- ANT+ FE-C, Leistung und Puls vorbereitet (aktiv, sobald der ANT+-Schlüssel eingebaut ist)
- Virtuelle Schaltung mit Wischgesten und Bluetooth-Tasten

## 0.1.0 (Build 1)
- Erste Testversion: Daum über Bluetooth, Bluetooth FTMS
