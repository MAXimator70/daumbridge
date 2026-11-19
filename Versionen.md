# Versionen

## 0.9.20 (Build 46) - 19.11.2026
- Neuer Schalter "Puls nie vom Daum nehmen" unter Einstellungen > Geraete, ab Werk an: der Pulsempfaenger im Daum wird ignoriert, Puls nur vom Pulsgurt

## 0.9.19 (Build 45) - 19.11.2026
- Querformat: Knopf heisst wieder "Auto-Pause", zweizeilig beschriftet

## 0.9.18 (Build 44) - 19.11.2026
- Pulsgurt trennen: roter Knopf in Einstellungen -> Pulsgurt und im Fenster Verbindungen (Chips oben antippen); trennt sofort, der Gurt ist frei fuer andere Geraete

## 0.9.17 (Build 43) - 18.11.2026
- LocalSend: kam am iPhone nichts an ("Handshake failed"), wird die verschluesselte Verbindung jetzt mehrfach versucht; DaumBridge erkennt selbst, ob das iPhone verschluesselt oder unverschluesselt empfaengt, und wechselt automatisch
- LocalSend: klare Meldung mit Abhilfe (am iPhone in LocalSend die Verschluesselung ausschalten)
- Loeschen und Aufraeumen in Rot, Bestaetigungsknopf zum Loeschen rot

## 0.9.16 (Build 42) - 18.11.2026
- Knopf rechts unten heisst jetzt "Verbinden" statt "Start" (die Uhr laeuft ohnehin erst mit dem ersten Tritt); waehrend des Trainings weiter "Stopp"

## 0.9.15 (Build 41) - 18.11.2026
- Querformat: Zahlen groesser und extra fett
- Querformat: Knoepfe Pause und Zonen quadratisch, Beschriftung mittig und in fester Groesse
- Querformat: Puls direkt unter Leistung, Kadenz darunter; Puls ohne "bpm", damit die Zahl Platz hat

## 0.9.14 (Build 40) - 18.11.2026
- Querformat: Werte-Spalte deutlich schmaler (20 %), das Diagramm bekommt 80 % der Breite
- Querformat: Zahlen passen sich der Spalte an, Knoepfe schmaler, Batterie ohne Zahl
- Herz wird selbst gezeichnet: auf manchen Handys (z. B. Samsung) war es als Emoji immer rot, jetzt wirklich grau/gelb/rot

## 0.9.13 (Build 39) - 18.11.2026
- Querformat: Auto-Pause und Zonen als grosse Knoepfe ueber die ganze Kachelhoehe
- Querformat: Puls-Kachel in der Farbe der aktuellen Pulszone, Zonenname ausgeschrieben
- Grosses Herz, schlaegt im Pulstakt; rot = Werte kommen, gelb = Gurt wird gesucht, grau = kein Gurt verbunden
- Akkustand des Pulsgurts: senkrechte Batterie in der Puls-Kachel (gruen, gelb unter 20 %, rot unter 10 %), im Verbindungsfenster und Hinweis unter 15 %

## 0.9.12 (Build 38) - 18.11.2026
- Uhr startet erst mit dem ersten Tritt (vorher wird nichts aufgezeichnet)
- Auto-Pause: Uhr haelt an, wenn 5 s nicht getreten wird; Schalter klein in der Dauer-Karte (Hauptseite und Querformat), gelb PAUSE waehrend der Pause
- Querformat neu: links alle Werte uebereinander, rechts das Diagramm mit Pulszonen, Zoomen mit zwei Fingern (1-30 min), Punkt an der aktuellen Position, Streifen Zeit in Pulszonen (Knopf Zonen blendet ihn aus)
- Trainings per LocalSend direkt ans iPhone (oder andere Geraete) im WLAN, auf Wunsch automatisch nach jedem Training
- Trainings per E-Mail: Adresse in den Einstellungen, fertige Mail mit FIT-Anhang

## 0.9.11 (Build 37) - 18.11.2026
- Handy quer drehen: Diagramm ueber den ganzen Bildschirm, ohne Tasten und ohne Statusleiste; aktuelle Leistung, Kadenz, Puls und Dauer gross in der Kopfzeile
- Pulszonen als farbige Baender hinter der Pulskurve, aktuelle Zone als farbiges Schild neben dem Puls
- Hochkant drehen = zurueck zur normalen Ansicht, das Training laeuft weiter

## 0.9.10 (Build 36) - 13.11.2026
- Menue: Eintrag Verbindungen entfernt - das Fenster oeffnet sich per Tipp auf die Chips Daum, BT oder Puls

## 0.9.9 (Build 35) - 13.11.2026
- Chips Puls und Daum: gruen = verbunden, gelb = Verbindung wird gesucht bzw. aufgebaut
- Herz neben bpm: gelb beim Suchen, rot und schlaegt im Takt des Pulses, sobald Werte kommen
- Ueberschrift PULS neutral statt rot

## 0.9.8 (Build 34) - 13.11.2026
- Update-Suche und Update-Download funktionieren jetzt auch auf Android 7.0 (z. B. Galaxy S6): die App kennt die Let's-Encrypt-Stammzertifizierung, die GitHub verwendet

## 0.9.7 (Build 33) - 13.11.2026
- Pulsgurt verbindet sich schon, wenn die App offen ist: Puls vor dem Start sichtbar, Herz neben bpm gruen (Werte kommen) bzw. orange, Chip Puls gruen
- Filter gegen Puls-Ausreisser (ueber Maximalpuls, sprunghafte Spitzen) fuer Gurt und Daum
- Neu: Erweitert > Puls vom Daum verwenden (aus = kein Puls statt ungenauer Werte)
- Einstellungen: eigene Seite Profil (Name, Geburtsdatum, Geschlecht, Gewicht, FTP, Fahrer loeschen)

## 0.9.6 (Build 32) - 13.11.2026
- Pulszonen: zwei Berechnungsmethoden wie in MaxUp - mit Ruhepuls (Karvonen) oder % vom Maximalpuls; Umschalten rechnet sofort neu, Erklaerung unter "Welche Methode?"
- Aenderung von Ruhe- oder Maximalpuls rechnet die Zonen nach der gewaehlten Methode neu

## 0.9.5 (Build 31) - 13.11.2026
- Trainings-Liste: Haken bei bereits geteilten Trainings, mit der App, an die geteilt wurde
- Neu: Aufraeumen - aelter als 3 Monate, aelter als 1 Jahr, alle bereits geteilten oder alle loeschen (mit Rueckfrage und Anzahl)

## 0.9.4 (Build 30) - 13.11.2026
- Neu: Training teilen als FIT-Datei - Knopf in der Zusammenfassung oeffnet das Teilen-Menue (Telegram, Google Drive, Dropbox, Synology, MaxUp ...); die Zusammenfassung bleibt dabei offen
- Neu: Menue > Trainings - alle Trainings ab 30 s bleiben auf dem Handy gespeichert und lassen sich jederzeit teilen oder loeschen

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
