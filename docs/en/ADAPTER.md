# DaumBridge – Bluetooth adapters

🇩🇪 **[Deutsche Version](../ADAPTER.md)** · [← Back to overview](../../README.en.md)

DaumBridge needs a **Bluetooth serial adapter** on the Daum. The original blue Daum Bluetooth adapter is hard to find these days – luckily a standard **Bluetooth RS232 adapter**, available cheaply from electronics retailers, works as well.

## What the adapter must support

| Property | Must be | Why |
|---|---|---|
| Bluetooth type | **classic Bluetooth with SPP** ("Serial Port Profile", often "Bluetooth 2.0/2.1" or "Classic") | DaumBridge connects via SPP. **BLE-only adapters** (Bluetooth Low Energy, often "BLE" or "4.0 LE" in the name) do **not** work. |
| Interface | **RS232 with a 9-pin D-sub connector (DB9)** | That's the Daum's PC port. **No** "TTL" or "UART" modules with pin headers – they use different voltages. |
| Serial settings | **9600 baud, 8 data bits, no parity, 1 stop bit (8N1)** | This is the factory default of most adapters. Otherwise change it once according to the adapter's manual. |
| Power | USB cable (charger or power bank) or battery | Many adapters don't get power from the Daum through the DB9 connector. |

## Connectors and cables

Whether the adapter fits the Daum directly depends on the connector:

- **Male or female?** Check whether the Daum and the adapter have pins ("male") or holes ("female"). If they don't match, a **DB9 gender changer** (a few euros) helps.
- **Null modem?** If the connection is up but no data arrives, transmit and receive (pins 2 and 3) may need to be swapped – with a **DB9 null modem adapter**. Some Bluetooth adapters have a switch for this (DCE/DTE).

## Examples

Suitable are classic Bluetooth RS232 adapters with DB9, for example the **DSD TECH SH-B23A** series or comparable models from other brands.

Check the name when buying: versions with **"BLE"** in the name (e.g. *SH-B30-BLE*) are Bluetooth Low Energy and do **not** work with DaumBridge.

> These examples have not been tested with DaumBridge and are not a buying recommendation. Please check the manufacturer's specifications before buying. If you use an adapter successfully, let us know – it will be added to this list.

## Setup

1. Plug the adapter into the Daum (with gender changer / null modem if needed) and power it.
2. Pair it in the **Android Bluetooth settings**. The PIN is in the adapter's manual – often **1234** or **0000**. The original Daum adapter sometimes pairs without a PIN.
3. In DaumBridge: **menu ☰ → *Einstellungen* → *Geräte* → *Daum-Adapter*** [Settings → Devices → Daum adapter] → select the new adapter.
4. **Start** – the **Daum** chip turns green as soon as the Daum responds.

If the chip doesn't turn green: check the baud rate (9600), then try a null modem adapter. The log (menu ☰ → *Protokoll*) shows whether the Daum responds.

## iPhone?

iPhones cannot access classic Bluetooth with SPP – that's why DaumBridge is Android-only. See the [FAQ](FAQ.md).
