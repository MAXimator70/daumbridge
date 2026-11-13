# DaumBridge – Privacy

🇩🇪 **[Deutsche Version](../DATENSCHUTZ.md)** · [← Back to overview](../../README.en.md)

**In short:** DaumBridge stores everything on your phone only and doesn't send personal data anywhere.

## What is stored?

Only on the phone, in the app settings:

- rider profiles (name, date of birth, sex, weight, FTP, heart rate and zone values)
- the selected Bluetooth devices (Daum adapter, heart rate strap)
- other app settings

Ride data (power, heart rate etc.) is only kept in memory during the ride and is not stored permanently. The log is also kept in memory only.

Uninstalling the app deletes everything.

## What leaves the phone?

- **Via Bluetooth to your training app:** power, cadence, speed, heart rate – that's the purpose of the app. The training app may send your weight; DaumBridge only uses it for its calculations.
- **Update check:** On start, DaumBridge requests the file `version.json` from GitHub to find new versions. Like any web request, GitHub sees your IP address. No data about you is sent.
- **Log and crash reports** only leave the phone if you send them yourself via *Teilen* (share).

No ads, no analytics or tracking services, no account.

## Permissions

| Permission | What for |
|---|---|
| Bluetooth (nearby devices) | connection to the Daum adapter and heart rate strap, broadcasting to the training app |
| Location (Android 11 and older only) | required by Android to search for the heart rate strap. DaumBridge never reads your location. |
| Notifications | "ride running" notification so Android doesn't stop the app |
| Foreground service, wake lock | the ride keeps running when the screen is off |
| Internet | only for the update check and downloading new versions |
| Install apps | to install a downloaded update (asks every time) |

During a ride, DaumBridge temporarily changes the phone's Bluetooth name (e.g. to "DaumBridge") and restores it afterwards.
