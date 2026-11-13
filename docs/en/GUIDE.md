# DaumBridge – Guide

🇩🇪 **[Deutsche Version](../ANLEITUNG.md)** · [← Back to overview](../../README.en.md)

The app is in German. German menu names are shown in *italics* with the English meaning in brackets.

## 1. Install

1. On your Android phone, [download DaumBridge.apk](https://raw.githubusercontent.com/MAXimator70/daumbridge/main/DaumBridge.apk) (or from [Releases](https://github.com/MAXimator70/daumbridge/releases)).
2. Open the file. The first time, Android asks whether your browser (or file manager) may install apps → **allow**, go back, **Install**.
3. On first start, DaumBridge asks for **Bluetooth** ("Nearby devices") and **notifications** → allow both. Nothing works without Bluetooth; the notification shows that a ride is running.

DaumBridge announces new versions itself (or menu ☰ → *Nach Update suchen* [check for update]).

## 2. Pair the Daum adapter (once)

No original Daum adapter? A standard Bluetooth RS232 adapter works too – see [Bluetooth adapters](ADAPTER.md).

1. Switch on the Daum – the blue Bluetooth adapter must be plugged into the Daum.
2. On the phone open **Android Settings → Bluetooth** (or in DaumBridge: *Einstellungen → Geräte → Neues Gerät koppeln* [Settings → Devices → Pair new device]).
3. Tap the adapter in the list (usually named like `Daum_BT_…`).
4. **PIN:** If Android asks, it's the 4-digit number printed on the adapter. Some adapters pair without a PIN – that's normal.
5. Back in DaumBridge: **menu ☰ → *Einstellungen* → *Geräte* → *Daum-Adapter*** and select the adapter.

## 3. Start a ride

1. Tap **Start** on the main screen. The **Daum** chip at the top turns green once the connection is up.
2. The **BT** chip turns green once DaumBridge is broadcasting; the number next to it shows how many apps are connected.
3. On start, the logo flips over automatically and shows the **chart** (power, cadence, heart rate of the last 10 minutes). Swipe right to scroll back, **double-tap** to jump back to live, single tap flips back to the logo.
4. Done? Tap **Stopp** (stop) – the summary appears.
5. **Training teilen (FIT)** (share ride) opens the share menu: Telegram, Google Drive, Dropbox, Synology Drive, e-mail, MaxUp … The summary stays open – closed the share menu by accident? Just tap again.

Every ride of 30 seconds or more stays saved on the phone. To share or delete it later: **menu ☰ → *Trainings*** (rides) → tap the ride. The FIT file can be imported into MaxUp, Strava, Garmin Connect, TrainingPeaks and others.

If the connection to the Daum drops (adapter switched off, out of range), the chip turns orange (**Daum …**) and DaumBridge reconnects by itself.

## 4. Connect your training app

DaumBridge shows up as a smart trainer called **DaumBridge** (changeable under *Einstellungen → Erweitert → Bluetooth-Name* [Settings → Advanced → Bluetooth name]). Some apps add a number, e.g. "DaumBridge-4874" – that's fine.

### Zwift
*Paired devices* → choose **DaumBridge** for **Power**, **Cadence** and **Controllable**.

### MyWhoosh
*Connect devices* → **Smart trainer** → **DaumBridge**. Cadence comes along automatically.

### Apple TV
Same as Zwift. Note: Apple TV only connects **two Bluetooth devices** at a time (the remote counts). So it's best to route the heart rate strap through DaumBridge (see below) – then one connection is enough.

### Heart rate in the training app
If the heart rate comes through DaumBridge, also choose **DaumBridge** as **Heart rate** in the training app.

## 5. Heart rate strap (optional)

DaumBridge can connect to a Bluetooth heart rate strap itself, show your heart rate and pass it on to the training app. This is more accurate than the Daum's built-in receiver.

1. Put on the strap (moisten the contacts) so it starts sending.
2. DaumBridge → *Einstellungen → Geräte → Pulsgurt* [heart rate strap] → **Pulsgurt suchen** [search strap] → tap the strap.

Pairing in the Android settings is not needed – many straps even refuse it ("pairing rejected"). Up to Android 11, Android asks once for **location** permission for the search and location must be switched on; DaumBridge doesn't use it.

Important: many straps (e.g. **Polar H9**) allow only **one** Bluetooth connection. If the strap is already connected to a laptop, watch or the training app, DaumBridge gets no data. Disconnect it there.

## 6. Rider profiles

If several people ride, each gets their own profile with date of birth, weight, FTP, heart rate strap, heart rate zones and simulator strength.

- *Einstellungen → Fahrer* [Settings → Rider] → **+ Neu** [new] creates a profile.
- Tap a profile to select it; tap the active profile again to rename (*Umbenennen*) or delete (*Löschen*) it.
- On the main screen the active rider is shown next to **Dauer** (duration). Tap it to switch riders (when no ride is running).

Values are set with **scroll wheels** – no keyboard needed.

## 7. Heart rate zones and zone colours

*Einstellungen → Pulszonen* [heart rate zones] shows resting heart rate, max heart rate and the five zones:

| Zone (German) | Colour | Meaning |
|---|---|---|
| Erholung | blue | recovery, base |
| Fettverbrennung | green | fat burning, long easy rides |
| Aerob | yellow-green | aerobic, improves endurance |
| Anaerob | yellow | anaerobic, high intensity, intervals |
| Roter Bereich | red | red zone, maximum effort, very short only |

- ***Automatisch berechnen*** [calculate automatically]: the zone limits are calculated from your max heart rate. If a date of birth is set, DaumBridge suggests a max heart rate based on age.
- **Set manually:** tap any value and change it with the scroll wheel. A measured max heart rate (fitness test, sports watch) is more accurate than the estimate.

While riding, the **Puls** (heart rate) and **Leistung** (power) tiles change colour by zone. The bar ***Zeit in Pulszonen*** (time in heart rate zones) fills up during the first hour; grey is time below the recovery zone.

Power zones are based on the **FTP** in the profile.

## 8. Smart, ERG and SIM

- ***Smart ist EIN*** (smart on): the training app controls the Daum – in **ERG** mode it sets target watts, in **SIM** mode it sends slopes. The knob on the Daum is overridden.
- ***Smart ist AUS*** (smart off): DaumBridge only measures; you set the resistance on the Daum yourself.
- ***Simulatorstärke*** (simulator strength, under *Erweitert* [advanced]): 100 % = slopes as in the app, 50 % = half as steep. Note: Zwift has its own "trainer difficulty" slider – both add up.

## 9. Advanced settings

Under *Einstellungen → Erweitert* [Settings → Advanced]: simulator strength, maximum and minimum power, bike weight, wheel circumference, Bluetooth name, old Daum firmware, keep screen on, polling interval, log (*Protokoll*) and *Auf Standard zurücksetzen* (reset to defaults – profiles and devices are kept).

---
Problems? → [FAQ and troubleshooting](FAQ.md)
