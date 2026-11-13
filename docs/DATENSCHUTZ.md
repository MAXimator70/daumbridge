# DaumBridge – Datenschutz

🇬🇧 **[English version](en/PRIVACY.md)** · [← Zurück zur Übersicht](../README.md)

**Kurz:** DaumBridge speichert alles nur auf deinem Handy und schickt keine persönlichen Daten irgendwohin.

## Was wird gespeichert?

Nur auf dem Handy, in den App-Einstellungen:

- Fahrerprofile (Name, Geburtsdatum, Geschlecht, Gewicht, FTP, Puls- und Zonenwerte)
- die gewählten Bluetooth-Geräte (Daum-Adapter, Pulsgurt)
- weitere Einstellungen der App

Jedes Training ab 30 Sekunden wird beim Stopp als FIT-Datei (Zeit, Leistung, Trittfrequenz, Tempo, Strecke, Puls) im App-Speicher abgelegt – damit du es später teilen kannst. Andere Apps haben darauf keinen Zugriff. Einzelne Trainings löschst du unter Menü ☰ → *Trainings*. Das Protokoll liegt nur im Arbeitsspeicher.

Beim Deinstallieren der App wird alles gelöscht.

## Was verlässt das Handy?

- **Per Bluetooth an deine Trainings-App:** Leistung, Trittfrequenz, Tempo, Puls – das ist der Zweck der App. Die Trainings-App kann das Gewicht senden; DaumBridge nutzt es nur für die Berechnung.
- **Update-Prüfung:** Beim Start fragt DaumBridge bei GitHub die Datei `version.json` ab, um neue Versionen zu finden. Dabei sieht GitHub wie bei jedem Webseitenaufruf die IP-Adresse. Es werden keine Daten über dich mitgeschickt.
- **Trainings, Protokoll und Absturzberichte** verlassen das Handy nur, wenn du sie selbst über *Teilen* verschickst.

Keine Werbung, keine Analyse- oder Tracking-Dienste, kein Konto.

## Berechtigungen

| Berechtigung | Wofür |
|---|---|
| Bluetooth (Geräte in der Nähe) | Verbindung zum Daum-Adapter und Pulsgurt, Senden an die Trainings-App |
| Standort (nur bis Android 11) | Android verlangt ihn für die Suche nach dem Pulsgurt. DaumBridge liest den Standort nie aus. |
| Benachrichtigungen | Anzeige „Training läuft“, damit Android die App nicht beendet |
| Vordergrunddienst, Wach halten | Training läuft weiter, auch wenn der Bildschirm aus ist |
| Internet | nur für die Update-Prüfung und den Download neuer Versionen |
| Apps installieren | um ein heruntergeladenes Update zu installieren (fragt jedes Mal nach) |

Während des Trainings ändert DaumBridge vorübergehend den Bluetooth-Namen des Handys (z. B. auf „DaumBridge“) und stellt ihn danach wieder her.
