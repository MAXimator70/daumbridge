# DaumBridge – Häufige Fragen und Fehlerbehebung

**Deutsch** | [English](en/FAQ.md) · [← Zurück zur Übersicht](../README.md)

## Allgemein

**Läuft DaumBridge auf dem iPhone?**
Nein. Der blaue Daum-Adapter nutzt klassisches Bluetooth (serielle Verbindung). Apple erlaubt Apps diesen Zugriff nur bei Geräten mit Apple-Zertifizierung – der Daum-Adapter hat keine. DaumBridge braucht deshalb ein Android-Handy. Die Trainings-App selbst darf aber auf iPhone, iPad, Apple TV, Mac oder PC laufen.

**Welche Daum-Ergometer werden unterstützt?**
Entwickelt und getestet mit dem **Daum 8008 TRS 3**. Andere Daum-Modelle mit demselben seriellen Protokoll können funktionieren – Rückmeldungen sind willkommen.

**Der originale Daum-Bluetooth-Adapter ist vergriffen – was nun?**
Ein handelsüblicher Bluetooth-RS232-Adapter mit **klassischem Bluetooth (SPP)** und **DB9-Stecker** funktioniert auch. Worauf es ankommt (keine BLE-Variante, 9600 Baud, Stecker, Nullmodem): [Bluetooth-Adapter](ADAPTER.md).

**Kostet DaumBridge etwas?**
Nein. Kein Abo, keine Werbung, kein Konto.

**Warum steht „Smart“ statt „ERG“?**
Smart ist der Oberbegriff: Bei *Smart EIN* darf die Trainings-App den Daum steuern – je nach Training im ERG-Modus (feste Watt) oder SIM-Modus (Steigung). Welcher Modus gerade läuft, zeigt die Kachel **Modus**.

## Verbinden

**Android fragt beim Koppeln keine PIN ab – ist das falsch?**
Nein. Manche Adapter koppeln ohne PIN. Fragt Android danach, ist es die 4-stellige Nummer auf dem Adapter.

**Der Chip „Daum“ wird nicht grün.**
- Ist der Daum eingeschaltet und steckt der Adapter?
- Ist der Adapter in den Android-Bluetooth-Einstellungen gekoppelt und in DaumBridge unter *Geräte* gewählt?
- Ist der Adapter noch mit einem anderen Gerät (z. B. altem Handy, PC) verbunden? Dort trennen.
- Handy-Bluetooth einmal aus- und einschalten, dann erneut **Start**.

**Die Trainings-App findet „DaumBridge“ nicht.**
- Läuft das Training in DaumBridge (Stopp-Knopf sichtbar)? Gesendet wird nur, solange ein Training läuft.
- Ist der Chip **BT** grün?
- Im Trainings-Programm nach einem **Smart-Trainer / steuerbaren Trainer** suchen, nicht nach einem Leistungsmesser.
- Laptop: Bluetooth am Laptop eingeschaltet? Manche PCs brauchen einen USB-Bluetooth-Stick.

**In der Trainings-App heißt der Trainer „DaumBridge-4874“.**
Manche Apps (z. B. MyWhoosh) hängen eine eigene Nummer an. Das ist normal.

**Hieß er früher „POWER-…“?**
Ältere Versionen hatten den Namen nur in einem Teil der Bluetooth-Meldung. Seit Version 0.4.0 heißt der Trainer überall „DaumBridge“.

**Ändert DaumBridge den Bluetooth-Namen meines Handys?**
Ja, aber nur während des Trainings – Android meldet den Trainer unter dem Namen des Handys. Nach dem Training (und auch nach einem Absturz beim nächsten Start) bekommt das Handy seinen alten Namen zurück.

## Puls

**DaumBridge zeigt einen viel zu hohen Puls an.**
Der Pulsempfänger im Daum ist oft ungenau. Mit einem Bluetooth-Pulsgurt (*Einstellungen → Geräte → Pulsgurt*) nimmt DaumBridge nur noch den Wert vom Gurt.

**Der Pulsgurt verbindet sich nicht.**
- Gurt anlegen und Kontakte befeuchten – ohne Hautkontakt sendet er nicht.
- Viele Gurte (z. B. Polar H9) erlauben nur **eine** Verbindung. Ist er mit Laptop, Uhr oder Trainings-App verbunden, dort trennen.
- Erst in den Android-Bluetooth-Einstellungen koppeln, dann in DaumBridge wählen.
- Kommen 20 Sekunden keine Werte, verbindet sich DaumBridge selbst neu.

**Der Streifen „Zeit in Pulszonen“ bleibt leer.**
Er füllt sich erst beim Fahren und nur, wenn Pulswerte ankommen. Rechts daneben steht, warum er leer ist („kein Puls“ oder „füllt sich beim Fahren“).

**Stimmen meine Pulszonen?**
Die automatische Berechnung schätzt den Maximalpuls aus dem Alter – bei vielen Menschen weicht der echte Wert um 10 Schläge oder mehr ab. Besser: den Maximalpuls messen (Leistungstest, Pulsuhr) und eintragen. Pulszonen sind keine medizinische Beratung.

## Training

**Der Widerstand ändert sich nicht, wenn ich am Daum drehe.**
Bei *Smart EIN* steuert die Trainings-App den Daum und überstimmt den Drehknopf. Für freies Fahren *Smart AUS* wählen.

**Die Steigungen sind zu hart.**
*Einstellungen → Erweitert → Simulatorstärke* herabsetzen (z. B. 50–70 %). Oder in Zwift die „Trainer-Schwierigkeit“ verringern – aber nicht beides stark, sonst wirkt es doppelt.

**Das Handy geht während des Trainings aus.**
*Einstellungen → Erweitert → Bildschirm anlassen* einschalten. Bei manchen Herstellern zusätzlich in den Android-Akku-Einstellungen DaumBridge vom Energiesparen ausnehmen.

## Fehler melden

1. Menü ☰ → **Protokoll** → **Teilen** (z. B. per Mail oder Messenger).
2. Kurz beschreiben, was passiert ist und welches Handy und welche Trainings-App genutzt wurden.

Stürzt DaumBridge ab, zeigt die App beim nächsten Start einen Absturzbericht, der sich ebenfalls teilen lässt.
