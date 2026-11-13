# DaumBridge – FAQ and troubleshooting

🇩🇪 **[Deutsche Version](../FAQ.md)** · [← Back to overview](../../README.en.md)

## General

**Does DaumBridge run on iPhone?**
No. The blue Daum adapter uses classic Bluetooth (serial connection). Apple only lets apps access that for Apple-certified (MFi) devices – the Daum adapter isn't one. DaumBridge therefore needs an Android phone. The training app itself can run on iPhone, iPad, Apple TV, Mac or PC.

**Which Daum ergometers are supported?**
Developed and tested with the **Daum 8008 TRS 3**. Other Daum models with the same serial protocol may work – feedback is welcome.

**The original Daum Bluetooth adapter is sold out – what now?**
A standard Bluetooth RS232 adapter with **classic Bluetooth (SPP)** and a **DB9 connector** works too. What to look for (no BLE version, 9600 baud, connector, null modem): [Bluetooth adapters](ADAPTER.md).

**Does DaumBridge cost anything?**
No. No subscription, no ads, no account.

**Is the app available in English?**
Not yet – the app is in German. This documentation explains all menus in English.

**Why does it say "Smart" and not "ERG"?**
Smart is the umbrella term: with *Smart ist EIN* (smart on) the training app may control the Daum – in ERG mode (fixed watts) or SIM mode (slope), depending on the workout. The **Modus** (mode) tile shows which one is active.

## Connecting

**Android didn't ask for a PIN when pairing – is that wrong?**
No. Some adapters pair without a PIN. If Android asks, it's the 4-digit number on the adapter.

**The "Daum" chip doesn't turn green.**
- Is the Daum switched on and the adapter plugged in?
- Is the adapter paired in the Android Bluetooth settings and selected in DaumBridge under *Geräte* (devices)?
- Is the adapter still connected to another device (old phone, PC)? Disconnect it there.
- Switch the phone's Bluetooth off and on, then tap **Start** again.

**The training app can't find "DaumBridge".**
- Is a ride running in DaumBridge (stop button visible)? DaumBridge only broadcasts while a ride is running.
- Is the **BT** chip green?
- In the training app, search for a **smart trainer / controllable trainer**, not a power meter.
- Laptop: is Bluetooth switched on? Some PCs need a USB Bluetooth dongle.

**The training app shows the trainer as "DaumBridge-4874".**
Some apps (e.g. MyWhoosh) add their own number. That's normal.

**Does DaumBridge change my phone's Bluetooth name?**
Yes, but only during a ride – Android advertises the trainer under the phone's name. After the ride (and after a crash, on the next start) the phone gets its old name back.

## Heart rate

**DaumBridge shows a far too high heart rate.**
The Daum's built-in heart rate receiver is often inaccurate. With a Bluetooth heart rate strap (*Einstellungen → Geräte → Pulsgurt*) DaumBridge only uses the strap's value.

**Android says "pairing rejected" for the heart rate strap.**
That's normal – many straps can't be paired. Use *Pulsgurt suchen* (search strap) in DaumBridge instead.

**The heart rate strap doesn't connect.**
- Put on the strap and moisten the contacts – without skin contact it doesn't send.
- Many straps (e.g. Polar H9) allow only **one** connection. If it's connected to a laptop, watch or training app, disconnect it there.
- In DaumBridge go to *Einstellungen → Geräte → Pulsgurt* and tap **Pulsgurt suchen** (search strap) – pairing in Android is not needed.
- If no values arrive for 20 seconds, DaumBridge reconnects by itself.

**The "Zeit in Pulszonen" bar stays empty.**
It only fills while riding and only when heart rate data arrives. The text next to it says why it's empty ("kein Puls" = no heart rate, "füllt sich beim Fahren" = fills while riding).

**Are my heart rate zones right?**
The automatic calculation estimates max heart rate from age – for many people the real value differs by 10 beats or more. Better: measure your max heart rate (fitness test, sports watch) and enter it. Heart rate zones are not medical advice.

## Riding

**Turning the knob on the Daum doesn't change the resistance.**
With *Smart ist EIN* the training app controls the Daum and overrides the knob. For free riding choose *Smart ist AUS*.

**Climbs are too hard.**
Lower *Einstellungen → Erweitert → Simulatorstärke* (e.g. 50–70 %). Or lower Zwift's "trainer difficulty" – but not both by a lot, or it doubles up.

**The phone turns off during a ride.**
Switch on *Einstellungen → Erweitert → Bildschirm anlassen* (keep screen on). On some phones, also exclude DaumBridge from battery optimisation in the Android settings.

## Reporting a problem

1. Menu ☰ → ***Protokoll*** (log) → ***Teilen*** (share), e.g. by e-mail or messenger.
2. Briefly describe what happened and which phone and training app you used.

If DaumBridge crashes, it shows a crash report on the next start, which you can share too.
