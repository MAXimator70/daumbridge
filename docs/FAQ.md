# DaumBridge – Häufige Fragen und Fehlerbehebung

🇬🇧 **[English version](en/FAQ.md)** · [← Zurück zur Übersicht](../README.md)

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

**„Nach Update suchen“ geht auf einem älteren Handy (Android 7.0) nicht.**
Bis Version 0.9.7 kannte DaumBridge auf Android 7.0 (z. B. Galaxy S6) das Zertifikat von GitHub nicht. Ab 0.9.8 behoben – einmalig die neue Version per Browser oder vom PC installieren, danach klappt die Update-Suche wieder.

## Installation

**Beim Installieren kommt „Google Play Store angehalten“.**
Das kommt nicht von DaumBridge: Beim Installieren einer APK prüft *Google Play Protect* (Teil des Play Stores) die Datei, und auf älteren Handys stürzt diese Prüfung manchmal ab. Meist läuft die Installation trotzdem durch – nach „App schließen“ unter Menü ☰ → *Nach Update suchen* die Version prüfen. Sonst nochmal installieren. Hilft das nicht: *Android-Einstellungen → Apps → Google Play Store → Speicher → Cache leeren*, oder – wenn der Play Store gar nicht genutzt wird – dort **Deaktivieren** (lässt sich jederzeit wieder **Aktivieren**, gelöscht wird nichts).

**Gehen bei einem Update meine Einstellungen oder Trainings verloren?**
Nein. Ein Update überschreibt nur die App; Profile, Einstellungen und gespeicherte Trainings bleiben.

## Verbinden

**Android fragt beim Koppeln keine PIN ab – ist das falsch?**
Nein. Manche Adapter koppeln ohne PIN. Fragt Android danach, ist es die 4-stellige Nummer auf dem Adapter.

**Der Chip „Daum“ wird nicht grün.**
- Ist der Daum eingeschaltet und steckt der Adapter?
- Ist der Adapter in den Android-Bluetooth-Einstellungen gekoppelt und in DaumBridge unter *Geräte* gewählt?
- Ist der Adapter noch mit einem anderen Gerät (z. B. altem Handy, PC) verbunden? Dort trennen.
- Handy-Bluetooth einmal aus- und einschalten, dann erneut **Verbinden**.

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
Der Pulsempfänger im Daum ist oft ungenau. Mit einem Bluetooth-Pulsgurt (*Einstellungen → Geräte → Pulsgurt*) nimmt DaumBridge nur noch den Wert vom Gurt. Den Puls vom Daum nimmt DaumBridge gar nicht: Der Schalter *Einstellungen → Geräte → Puls nie vom Daum nehmen* ist ab Werk an. Nur wer ohne Gurt trotzdem den Daum-Puls sehen will, schaltet ihn aus.

**Der Puls springt stark auf und ab, obwohl ich ruhig sitze.**
Meist schlechter Hautkontakt am Gurt: Elektroden anfeuchten, Gurt enger und direkt unter der Brust tragen, Kunstfaser-Shirt vermeiden, Batterie prüfen. Grobe Ausreißer (über dem Maximalpuls, sprunghafte Spitzen) filtert DaumBridge seit 0.9.7 heraus.

**Android meldet beim Koppeln des Pulsgurts „Kopplung abgelehnt“.**
Das ist normal – viele Gurte lassen sich nicht koppeln. Stattdessen in DaumBridge *Pulsgurt suchen* verwenden.

**Der Pulsgurt verbindet sich nicht.**
- Gurt anlegen und Kontakte befeuchten – ohne Hautkontakt sendet er nicht.
- Viele Gurte (z. B. Polar H9) erlauben nur **eine** Verbindung. Ist er mit Laptop, Uhr oder Trainings-App verbunden, dort trennen.
- In DaumBridge unter *Einstellungen → Geräte → Pulsgurt* auf **Pulsgurt suchen** tippen – Koppeln in Android ist nicht nötig.
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

**Wie kommen meine Trainings aufs iPhone (z. B. in MaxUp)?**
Am einfachsten mit **LocalSend**: auf dem iPhone die kostenlose App LocalSend installieren und öffnen, in DaumBridge unter Einstellungen → *An das iPhone (LocalSend)* das iPhone wählen. Danach geht jedes Training beim Stopp automatisch übers WLAN ans iPhone (Dateien-App → LocalSend). Alternativ **per E-Mail** (Einstellungen → *Per E-Mail*). Per Bluetooth geht es nicht – das iPhone nimmt von Android-Handys keine Dateien per Bluetooth an.

**Bei einem Handy fehlt der Eintrag „An … senden“ / es steht „Ziel wählen“.**
Das Ziel-Gerät für LocalSend wird **pro Handy** gespeichert. Auf einem Handy, auf dem noch keins gewählt wurde, steht **An iPhone senden – Ziel wählen**: antippen, iPhone (mit geöffnetem LocalSend) auswählen – danach wird gesendet und das Ziel gemerkt. Oder vorab unter *Einstellungen → An das iPhone (LocalSend) → Ziel-Gerät*.

**Kann ich ein altes Training nochmal ansehen?**
Ja: Menü ☰ → *Trainings* → Training antippen → **Diagramm ansehen**. Das Training öffnet sich im Querformat mit Durchschnitts- und Maximalwerten links, dem Diagramm über das ganze Training rechts und der Zeit in Pulszonen unten. Zoomen mit zwei Fingern, Doppeltipp zeigt wieder alles.

**Wird das Diagramm in der FIT-Datei mitgeschickt?**
Die Daten ja – Leistung, Kadenz, Puls, Tempo und Strecke Sekunde für Sekunde. Das Bild selbst nicht: MaxUp, Strava, Garmin Connect & Co. zeichnen ihre Diagramme beim Import selbst. Die Pulszonen rechnet die Ziel-App nach ihren eigenen Einstellungen.

**LocalSend findet mein iPhone nicht.**
LocalSend muss am iPhone geöffnet sein, „Lokales Netzwerk“ muss erlaubt sein (iPhone-Einstellungen → LocalSend), und beide Geräte müssen im selben WLAN sein. Gast-WLANs und Router mit „Geräte voneinander abschirmen“ verhindern, dass sich die Geräte sehen.

**LocalSend findet das iPhone, aber es kommt nichts an („Handshake failed“ im Protokoll).**
Ältere Android-Handys bekommen die verschlüsselte Verbindung zu LocalSend auf dem iPhone manchmal nicht aufgebaut. Abhilfe: am iPhone in LocalSend unter **Einstellungen** die **Verschlüsselung** ausschalten. DaumBridge erkennt das selbst und sendet dann unverschlüsselt – im eigenen WLAN unbedenklich. Am iPhone erscheint beim Empfang eine Frage, ob du die Datei annehmen willst.

**Warum zeigt die Dauer 0:00:00, obwohl ich Verbinden getippt habe?**
Die Uhr startet erst mit dem ersten Tritt. Mit **Auto-Pause** (Schild oben rechts in der Dauer-Karte) hält sie außerdem an, wenn du länger als 5 Sekunden nicht trittst.

