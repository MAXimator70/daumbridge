# DaumBridge – Bluetooth-Adapter

**Deutsch** | [English](en/ADAPTER.md) · [← Zurück zur Übersicht](../README.md)

DaumBridge braucht am Daum einen **Bluetooth-Seriell-Adapter**. Der originale blaue Daum-Bluetooth-Adapter ist kaum noch zu bekommen – zum Glück funktioniert auch ein gewöhnlicher **Bluetooth-RS232-Adapter**, wie es ihn für wenig Geld im Elektronikhandel gibt.

## Was der Adapter können muss

| Eigenschaft | Muss sein | Warum |
|---|---|---|
| Bluetooth-Art | **klassisches Bluetooth mit SPP** („Serial Port Profile“, oft „Bluetooth 2.0/2.1“ oder „Classic“) | DaumBridge verbindet sich per SPP. **Reine BLE-Adapter** (Bluetooth Low Energy, oft „BLE“ oder „4.0 LE“ im Namen) funktionieren **nicht**. |
| Schnittstelle | **RS232 mit 9-poligem D-Sub-Stecker (DB9)** | Das ist die PC-Schnittstelle des Daum. **Keine** „TTL“- oder „UART“-Module mit Stiftleiste – die haben andere Spannungen. |
| Übertragung | **9600 Baud, 8 Datenbits, keine Parität, 1 Stoppbit (8N1)** | Das ist bei den meisten Adaptern die Werkseinstellung. Sonst einmal laut Anleitung des Adapters umstellen. |
| Stromversorgung | USB-Kabel (Netzteil oder Powerbank) oder Batterie | Viele Adapter bekommen über den DB9-Stecker keinen Strom vom Daum. |

## Stecker und Kabel

Ob der Adapter direkt an den Daum passt, hängt vom Stecker ab:

- **Stecker oder Buchse?** Am Daum und am Adapter nachsehen, ob Stifte („male“) oder Löcher („female“) vorhanden sind. Passt es nicht, hilft ein **DB9-Gender-Changer** (wenige Euro).
- **Nullmodem?** Kommen keine Daten an, obwohl die Verbindung steht, müssen eventuell Senden und Empfangen (Pin 2 und 3) getauscht werden – mit einem **DB9-Nullmodem-Adapter**. Manche Bluetooth-Adapter haben dafür auch einen Schalter (DCE/DTE).

## Beispiele

Geeignet sind klassische Bluetooth-RS232-Adapter mit DB9, zum Beispiel aus der Serie **DSD TECH SH-B23A** oder vergleichbare Modelle anderer Hersteller.

Beim Kauf auf den Namen achten: Varianten mit **„BLE“** im Namen (z. B. *SH-B30-BLE*) sind Bluetooth Low Energy und funktionieren mit DaumBridge **nicht**.

> Diese Beispiele sind nicht von DaumBridge getestet und keine Kaufempfehlung. Bitte vor dem Kauf die Angaben des Herstellers prüfen. Wer einen Adapter erfolgreich nutzt, kann gerne Bescheid geben – dann kommt er auf diese Liste.

## Einrichten

1. Adapter an den Daum stecken (ggf. mit Gender-Changer / Nullmodem) und mit Strom versorgen.
2. Am Handy in den **Android-Bluetooth-Einstellungen** koppeln. Die PIN steht in der Anleitung des Adapters – häufig **1234** oder **0000**. Der originale Daum-Adapter koppelt teils ohne PIN.
3. In DaumBridge: **Menü ☰ → Einstellungen → Geräte → Daum-Adapter** → den neuen Adapter wählen.
4. **Start** – der Chip **Daum** wird grün, sobald der Daum antwortet.

Wird der Chip nicht grün: Baudrate (9600) prüfen, dann den Nullmodem-Adapter probieren. Das **Protokoll** (Menü ☰ → Protokoll) zeigt, ob der Daum antwortet.

## iPhone?

Klassisches Bluetooth mit SPP können iPhones nicht ansprechen – deshalb gibt es DaumBridge nur für Android. Siehe [Häufige Fragen](FAQ.md).
