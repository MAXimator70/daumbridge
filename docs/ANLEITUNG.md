# DaumBridge – Anleitung

**Deutsch** | [English](en/GUIDE.md) · [← Zurück zur Übersicht](../README.md)

## 1. Installieren

1. Auf dem Android-Handy [DaumBridge.apk herunterladen](https://raw.githubusercontent.com/MAXimator70/daumbridge-download/main/DaumBridge.apk) (oder unter [Releases](https://github.com/MAXimator70/daumbridge-download/releases)).
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
2. Der Chip **BT** wird grün, sobald DaumBridge sendet; die Zahl daneben zeigt, wie viele Apps verbunden sind.
3. Fertig? **Stopp** tippen – danach erscheint die Zusammenfassung.

Bricht die Verbindung zum Daum ab (Adapter kurz aus, außer Reichweite), wird der Chip **Daum …** orange und DaumBridge verbindet sich selbst neu.

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
2. In den Android-Bluetooth-Einstellungen koppeln.
3. DaumBridge → *Einstellungen → Geräte → Pulsgurt* → Gurt wählen.

Wichtig: Viele Gurte (z. B. **Polar H9**) erlauben nur **eine** Bluetooth-Verbindung. Ist der Gurt schon mit dem Laptop, der Uhr oder der Trainings-App verbunden, bekommt DaumBridge keine Werte. Dort also trennen.

## 6. Fahrerprofile

Fahren mehrere Personen, bekommt jede ein eigenes Profil mit Geburtsdatum, Gewicht, FTP, Pulsgurt, Pulszonen und Simulatorstärke.

- *Einstellungen → Fahrer* → **+ Neu** legt ein Profil an.
- Auf ein Profil tippen wählt es aus; das aktive Profil nochmal antippen → umbenennen oder löschen.
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

- **Automatisch berechnen:** Die Grenzen werden aus dem Maximalpuls berechnet. Ist ein Geburtsdatum hinterlegt, schlägt DaumBridge einen Maximalpuls aus dem Alter vor.
- **Selbst einstellen:** Jeden Wert antippen und per Drehrad ändern. Ein gemessener Maximalpuls (Leistungstest, Pulsuhr) ist genauer als die Schätzung.

Beim Fahren färben sich die Kacheln **Puls** und **Leistung** nach Zone. Der Streifen **Zeit in Pulszonen** füllt sich während der ersten Stunde; grau ist die Zeit unterhalb der Erholungszone.

Die Leistungszonen richten sich nach der **FTP** im Profil.

## 8. Smart, ERG und SIM

- **Smart EIN:** Die Trainings-App steuert den Daum – im **ERG**-Modus gibt sie Watt vor, im **SIM**-Modus Steigungen. Der Drehknopf am Daum wird dann überstimmt.
- **Smart AUS:** DaumBridge misst nur; die Leistung stellst du am Daum selbst ein.
- **Simulatorstärke** (*Erweitert*): 100 % = Steigungen wie in der App, 50 % = halb so steil. Achtung: Zwift hat einen eigenen Regler „Trainer-Schwierigkeit“ – beide wirken zusammen.

## 9. Erweiterte Einstellungen

Unter *Einstellungen → Erweitert*: Simulatorstärke, maximale und minimale Leistung, Fahrradgewicht, Radumfang, Bluetooth-Name, alte Daum-Firmware, Bildschirm anlassen, Abfrage-Intervall, Protokoll und *Auf Standard zurücksetzen* (Profile und Geräte bleiben erhalten).

---
Probleme? → [Häufige Fragen und Fehlerbehebung](FAQ.md)
