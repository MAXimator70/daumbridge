# DaumBridge – Anleitung

🇬🇧 **[English version](en/GUIDE.md)** · [← Zurück zur Übersicht](../README.md)

## 1. Installieren

1. Auf dem Android-Handy [DaumBridge.apk herunterladen](https://raw.githubusercontent.com/MAXimator70/daumbridge/main/DaumBridge.apk) (oder unter [Releases](https://github.com/MAXimator70/daumbridge/releases)).
2. Die Datei öffnen. Beim ersten Mal fragt Android, ob der Browser (oder Dateimanager) Apps installieren darf → **erlauben**, zurück, **Installieren**.
3. Beim ersten Start fragt DaumBridge nach **Bluetooth** („Geräte in der Nähe“) und **Benachrichtigungen** → beides erlauben. Ohne Bluetooth geht nichts; die Benachrichtigung zeigt, dass ein Training läuft.

Spätere Versionen meldet DaumBridge selbst (oder Menü ☰ → *Nach Update suchen*).

## 2. Daum-Adapter koppeln (einmalig)

Kein originaler Daum-Adapter? Ein handelsüblicher Bluetooth-RS232-Adapter geht auch – siehe [Bluetooth-Adapter](ADAPTER.md).

1. Den Daum einschalten – der blaue Bluetooth-Adapter muss am Daum stecken.
2. Am Handy **Android-Einstellungen → Bluetooth** öffnen (oder in DaumBridge: *Einstellungen → Geräte → Neues Gerät koppeln*).
3. Den Adapter in der Liste antippen (meist ein Name wie `Daum_BT_…`).
4. **PIN:** Fragt Android danach, ist es die 4-stellige Nummer, die auf dem Adapter steht. Manche Adapter koppeln ohne PIN – das ist normal.
5. Zurück in DaumBridge: **Menü ☰ → Einstellungen → Geräte → Daum-Adapter** und den Adapter auswählen.

## 3. Training starten

1. Auf der Startseite **Start** tippen. Der Chip **Daum** oben wird grün, sobald die Verbindung steht.
2. Der Chip **BT** wird grün, sobald DaumBridge sendet; die Zahl daneben zeigt, wie viele Apps verbunden sind. Antippen eines Chips (Daum, BT, Puls) zeigt alle Verbindungen auf einen Blick.
3. Beim Start dreht sich das Logo automatisch um und zeigt das **Diagramm** (Leistung, Kadenz, Puls der letzten 10 Minuten). Mit dem Finger nach rechts wischen blättert zurück, **Doppeltipp** springt wieder auf live, einfaches Antippen dreht zurück zum Logo.
4. Die **Uhr startet mit dem ersten Tritt** – vorher steht unter DAUER „wartet auf den ersten Tritt“ und es wird noch nichts aufgezeichnet. Du kannst also in Ruhe Start tippen und erst später losfahren.
5. **Auto-Pause:** Das kleine Schild **⏸ Auto-Pause** oben rechts in der Dauer-Karte schaltet sie ein (grün) oder aus (grau). Eingeschaltet hält die Uhr an, wenn du länger als 5 Sekunden nicht trittst – das Schild zeigt dann gelb **PAUSE**, die Zeit wird gelb. Pausen zählen nicht in Dauer, Durchschnitte, Zonenzeit und FIT-Datei.
6. Fertig? **Stopp** tippen – danach erscheint die Zusammenfassung.
7. **Training teilen (FIT)** öffnet das Teilen-Menü: Telegram, Google Drive, Dropbox, Synology Drive, Mail, MaxUp … Die Zusammenfassung bleibt offen – versehentlich geschlossen? Einfach nochmal tippen. Ist ein LocalSend-Gerät oder eine E-Mail-Adresse eingestellt (siehe unten), gibt es dafür eigene Knöpfe.

### Querformat

Handy quer drehen: Links stehen in einer schmalen Spalte alle Werte übereinander (Dauer mit Auto-Pause, Leistung, Kadenz, Puls mit aktueller Zone, Tempo, Strecke), rechts nimmt das große Diagramm vier Fünftel der Breite ein, mit den Pulszonen als farbigen Bändern. Ein Punkt markiert die aktuelle Position, das Diagramm läuft mit.

- **Zoomen** mit zwei Fingern (1 bis 30 Minuten), **wischen** blättert zurück, **Doppeltipp** beendet Zoom und Zurückblättern.
- Unten der Streifen **Zeit in Pulszonen** fürs ganze Training – bleibt beim Zoomen unverändert. Der Knopf **Zonen** in der Puls-Kachel blendet ihn aus, dann wird das Diagramm größer.
- Die Puls-Kachel färbt sich in der aktuellen Pulszone und zeigt den Namen ausgeschrieben (z. B. „Z2 · FETTVERBRENNUNG“). **Pause** (Auto-Pause) und **Zonen** sind Knöpfe über die ganze Kachelhöhe. Die Gurt-Batterie zeigt im Querformat nur die Farbe, ohne Zahl.
- Hochkant drehen = zurück zur normalen Ansicht, das Training läuft weiter.

### Trainings ans iPhone schicken (LocalSend)

DaumBridge kann jedes Training direkt an ein Gerät im selben WLAN schicken, auf dem die kostenlose App **LocalSend** läuft – z. B. ein iPhone. Auf dem Android-Handy ist dafür keine zusätzliche App nötig.

1. Auf dem iPhone **LocalSend** aus dem App Store installieren, öffnen und „Lokales Netzwerk“ erlauben. Tipp: in LocalSend **Schnellspeichern** einschalten, dann ist kein Annehmen nötig.
2. In DaumBridge: **Einstellungen → An das iPhone (LocalSend) → Ziel-Gerät** – DaumBridge sucht im WLAN, iPhone antippen.
3. **Nach dem Training senden** eingeschaltet: Beim Stopp geht die FIT-Datei automatisch ans iPhone. Die Zusammenfassung zeigt „Sende …“, „✓ gesendet“ oder einen Hinweis, falls das iPhone nicht erreichbar war (LocalSend öffnen, dann **An … senden** tippen).
4. Auf dem iPhone liegt die Datei in der **Dateien**-App im Ordner LocalSend – antippen, teilen, z. B. an MaxUp.

LocalSend muss auf dem Empfänger geöffnet sein, wenn gesendet wird. Ältere Trainings schickst du über Menü ☰ → *Trainings* → Training antippen → **An … senden**.

### Trainings per E-Mail

**Einstellungen → Per E-Mail → E-Mail-Adresse** eintragen. Dann gibt es in der Zusammenfassung und unter Menü ☰ → *Trainings* den Knopf **Per E-Mail**: Die Mail-App öffnet sich mit Empfänger, Betreff, Kennzahlen und der FIT-Datei im Anhang – nur noch **Senden** tippen. Mit **Nach dem Training öffnen** geht die fertige Mail beim Stopp von selbst auf.

Jedes Training ab 30 Sekunden bleibt auf dem Handy gespeichert. Später teilen oder löschen: **Menü ☰ → *Trainings*** → Training antippen. Bereits geteilte Trainings haben ein **✓** (mit der App, an die geteilt wurde). Mit **Aufräumen** löschst du mehrere auf einmal: älter als 3 Monate, älter als 1 Jahr, alle bereits geteilten oder alle – immer mit Rückfrage. Die FIT-Datei lässt sich in MaxUp, Strava, Garmin Connect, TrainingPeaks & Co. importieren.

Bricht die Verbindung zum Daum ab (Adapter kurz aus, außer Reichweite), wird der Chip **Daum …** gelb und DaumBridge verbindet sich selbst neu.

## 4. Mit der Trainings-App verbinden

DaumBridge erscheint in der Trainings-App als Smart-Trainer mit dem Namen **DaumBridge** (änderbar unter *Einstellungen → Erweitert → Bluetooth-Name*). Manche Apps hängen eine Nummer an, z. B. „DaumBridge-4874“ – das ist richtig so.

### Zwift
*Gepaarte Geräte* → bei **Leistung**, **Trittfrequenz** und **Steuerbarer Trainer** jeweils **DaumBridge** wählen.

### MyWhoosh
*Geräte verbinden* → **Smart Trainer** → **DaumBridge**. Trittfrequenz kommt automatisch mit.

### Apple TV
Wie bei Zwift. Hinweis: Apple TV verbindet höchstens **zwei Bluetooth-Geräte** gleichzeitig (Fernbedienung zählt mit). Den Pulsgurt deshalb lieber über DaumBridge laufen lassen (siehe unten) – dann reicht eine Verbindung.

### Puls in der Trainings-App
Kommt der Puls über DaumBridge, in der Trainings-App bei **Herzfrequenz** ebenfalls **DaumBridge** wählen.

## 5. Pulsgurt (optional)

DaumBridge kann sich selbst mit einem Bluetooth-Pulsgurt verbinden, den Puls anzeigen und an die Trainings-App weitergeben. Das ist genauer als der Pulsempfänger im Daum.

1. Den Gurt anlegen (Kontakte leicht befeuchten), damit er sendet.
2. DaumBridge → *Einstellungen → Geräte → Pulsgurt* → **Pulsgurt suchen** → Gurt antippen.

Koppeln in den Android-Einstellungen ist nicht nötig – viele Gurte lehnen das sogar ab („Kopplung abgelehnt“). Bis Android 11 fragt Android für die Suche einmal nach dem **Standort** und der Standort muss eingeschaltet sein; DaumBridge nutzt ihn nicht.

Sobald die App offen ist, verbindet sie sich mit dem Gurt – der Puls steht schon **vor dem Start** in der Kachel. Der Chip **Puls** oben ist **grün**, wenn Werte vom Gurt kommen, und **gelb**, solange der Gurt gesucht wird. Das **♥** neben „bpm“ ist dann gelb bzw. **rot und schlägt im Takt deines Pulses**. Ist die App im Hintergrund und läuft kein Training, trennt sie den Gurt nach 20 Sekunden wieder.

Offensichtliche Messfehler (z. B. 199 bpm im Sitzen bei schlechtem Hautkontakt oder sprunghafte Ausreißer) filtert DaumBridge heraus. Springt der Puls trotzdem stark: Elektroden anfeuchten, Gurt enger stellen, Batterie prüfen.

Wichtig: Viele Gurte (z. B. **Polar H9**) erlauben nur **eine** Bluetooth-Verbindung. Ist der Gurt schon mit dem Laptop, der Uhr oder der Trainings-App verbunden, bekommt DaumBridge keine Werte. Dort also trennen.

**Herz und Akku:** Das ♥ in der Puls-Kachel ist **rot** und schlägt im Takt deines Pulses, sobald Werte kommen, **gelb**, solange der Gurt gesucht wird, und **grau**, wenn kein Gurt verbunden ist. Daneben zeigt eine senkrechte **Batterie** den Akkustand des Gurts – grün, unter 20 % gelb, unter 10 % rot; unter 15 % erscheint beim Verbinden einmal ein Hinweis. Gurte, die keinen Akkustand melden, zeigen keine Batterie.

## 6. Fahrerprofile

Fahren mehrere Personen, bekommt jede ein eigenes Profil mit Geburtsdatum, Gewicht, FTP, Pulsgurt, Pulszonen und Simulatorstärke.

- *Einstellungen → Fahrer* → **+ Neu** legt ein Profil an.
- Auf ein Profil tippen wählt es aus; das aktive Profil nochmal antippen → umbenennen oder löschen.
- **Profil ›** öffnet eine eigene Seite mit Name, Geburtsdatum, Geschlecht, Gewicht und FTP (und *Fahrer löschen*).
- Auf der Startseite steht der aktive Fahrer bei der **Dauer**. Antippen wechselt den Fahrer (wenn kein Training läuft).

Werte stellst du mit **Drehrädern** ein – keine Tastatur nötig.

## 7. Pulszonen und Zonenfarben

*Einstellungen → Pulszonen* zeigt Ruhepuls, Maximalpuls und die fünf Zonen:

| Zone | Farbe | Bedeutung |
|---|---|---|
| Erholung | blau | Grundlage, Regeneration |
| Fettverbrennung | grün | lange, ruhige Ausfahrten |
| Aerob | gelbgrün | verbessert die Ausdauer |
| Anaerob | gelb | hohe Intensität, Intervalle |
| Roter Bereich | rot | Maximalbelastung, nur sehr kurz |

- **Berechnung – zwei Methoden** (umschaltbar, die Zonen rechnen sofort neu):
  - **Mit Ruhepuls (Karvonen):** Untergrenzen = Ruhepuls + 50 / 60 / 70 / 80 / 90 % der Pulsreserve (Maximalpuls − Ruhepuls). Berücksichtigt die Fitness – am besten, wenn du deinen Ruhepuls kennst (morgens im Liegen messen).
  - **% vom Max.:** Untergrenzen = 70,5 / 76,5 / 82 / 88 / 94 % vom Maximalpuls. Einfach, braucht nur den Maximalpuls.
  - *Welche Methode? ›* auf der Zonen-Seite erklärt beide.
- Änderst du Ruhe- oder Maximalpuls, werden die Zonen nach der gewählten Methode neu berechnet.
- **Automatisch berechnen:** berechnet die Zonen nach der gewählten Methode. Ist ein Geburtsdatum hinterlegt, schlägt DaumBridge einen Maximalpuls aus dem Alter vor.
- **Selbst einstellen:** Jeden Wert antippen und per Drehrad ändern. Ein gemessener Maximalpuls (Leistungstest, Pulsuhr) ist genauer als die Schätzung.

Beim Fahren färben sich die Kacheln **Puls** und **Leistung** nach Zone. Der Streifen **Zeit in Pulszonen** füllt sich während der ersten Stunde; grau ist die Zeit unterhalb der Erholungszone.

Die Leistungszonen richten sich nach der **FTP** im Profil.

## 8. Smart, ERG und SIM

- **Smart EIN:** Die Trainings-App steuert den Daum – im **ERG**-Modus gibt sie Watt vor, im **SIM**-Modus Steigungen. Der Drehknopf am Daum wird dann überstimmt.
- **Smart AUS:** DaumBridge misst nur; die Leistung stellst du am Daum selbst ein.
- **Simulatorstärke** (*Erweitert*): 100 % = Steigungen wie in der App, 50 % = halb so steil. Achtung: Zwift hat einen eigenen Regler „Trainer-Schwierigkeit“ – beide wirken zusammen.

## 9. Erweiterte Einstellungen

Unter *Einstellungen → Erweitert*: Simulatorstärke, maximale und minimale Leistung, Fahrradgewicht, Radumfang, Bluetooth-Name, alte Daum-Firmware, *Puls vom Daum verwenden* (ohne Gurt; aus = kein Puls statt ungenauer Werte), Bildschirm anlassen, Abfrage-Intervall, Protokoll und *Auf Standard zurücksetzen* (Profile und Geräte bleiben erhalten).

---
Probleme? → [Häufige Fragen und Fehlerbehebung](FAQ.md)
