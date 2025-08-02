# 📖 Power Receiver Documentation – microver.ch

Welcome to the technical documentation for the **Power Receiver** by [microver.ch](https://microver.ch).  
This device adapts standard **Makita 18V batteries** for safe and versatile use in robotics and prototyping.

---

## 🔧 1. Overview

The **microver.ch Power Receiver** includes:

- 🔋 1x Makita 18V battery connector (mechanical + electrical)
- 🧷 3x M3x30 socket head cap screw mounting holes
- 🔌 1x USB-C port with smart PMIC (charge + discharge)
- 🔥 1x 5×20mm glass fuse holder
- 🧯 1x Replaceable 10A glass fuse for short circuit protection
- ⚡ 3x 2.1mm DC Barrel Jacks (direct battery output)

---

## 🛠️ 2. USB-C Smart Charging & Discharging

The Power Receiver uses a **Power Management IC (PMIC)** for intelligent USB-C handling.

### 🔋 Charging Mode

- Charges 18V Makita batteries with CC/CV profile
- Example: Charges a 2Ah battery in ~120 minutes (80% in first 60)
- Charging LED: blinks red at 1Hz while charging, solid red when full
- Charging power draw: ~2A at ~21V (CV)

### ⚡ Discharging Mode

- Acts as a USB-C power bank
- Supports multiple protocols:
  - USB-C 3.0A
  - PD2.0 / PD3.0 (up to 100W)
  - QC3.0, Apple 2.4A, Samsung AFC, Huawei FCP/SCP
- Output capabilities:
  - 5V/3A (15W), 9V/3A (27W), 12V/3A (36W), 15V/3A (45W), 20V/5A (100W)

### ❗ Usage Notes

To **enable power-bank mode**, you must:

1. Clip in a battery  
2. Plug into a USB-C wall charger for 2–3 seconds  
3. Then unplug charger and connect your device  
4. Do not remove the battery in between, or the PMIC resets

> LED ON (no blink) = discharging successfully  
> LED blinking = discharging failed (needs re-init)

---

## 🔐 3. Protections

### ✅ USB-C PMIC Protections

- ✅ Undervoltage cutoff at 15.0V  
- ✅ Overvoltage cutoff at 21.0V  
- ✅ Overcurrent protection (max 5.0A USB-C)

### 🔥 Replaceable Glass Fuse

- 5×20mm 10A glass fuse
- Protects from short circuits via DC jacks or other errors
- Always **unplug the fuse** when testing circuits!

**To replace:**

1. Pull the fuse gently with pliers  
2. Dispose of broken fuse  
3. Insert new 5×20mm 10A fuse  

: Good fuse: intact wire  
> Bad fuse: wire blown or glass blackened

---

## ⚡ 4. DC Barrel Jacks (Direct Battery Output)

- 3x 2.1mm barrel jacks at back of Power Receiver
- Direct connection to battery terminals
- No internal regulation or protection

**⚠️ DANGER:**  
- Never charge batteries using these jacks  
- Never discharge battery below **15.0V**  
- Always monitor voltage with a voltmeter!

---

## 🔋 5. Makita 18V Battery Notes

### 🔢 Voltage Range

- Normal operating range: **15.0V – 21.0V**
- Below 15.0V → battery may become permanently disabled
- Above 21.0V → risk of fire or explosion

### ⚡ Current Capability

- Handles 8–10A safely for up to 12 minutes
- Protected by 10A fuse

### 🌡️ Temperature & Humidity

- Operating temperature: **0°C – 40°C**
- Do not expose to water or high humidity

---

## 🚨 6. Battery Indicator Disclaimer

- Makita charge LEDs are not functional with Power Receiver charging (circuit goes into fault and blinks LEDs after 2-3 charges)
- Use a **voltmeter** via barrel jack to estimate charge

| Voltage (V) | Charge (%) |
|-------------|-------------|
| 21.0        | 100%        |
| 19.5        | 75%         |
| 18.0        | 33%         |
| 15.0        | 0%          |

> Never probe battery pins directly!  
> Always use a barrel jack and multimeter to check voltage.

---

## 📏 7. Mounting & Mechanical

- Overall Dimensions: ~72mm × 94 mm × 42mm
- Mount with 3x M3x30 screws through chassis
- Screw Pattern is: 44mm x 50mm
- Fits most robotics platforms

---

## 🧪 8. Best Practices

- Always check your circuit before inserting the fuse  
- Never work live — remove fuse before debugging  
- Always use USB-C for charging  
- Never charge via DC barrel jacks  
- Monitor voltage when discharging via barrel jacks

---

## 🛒 9. Purchase & Files

- Order units at: [shop.microver.ch](https://shop.microver.ch)  
- Included: Power Receiver, 3x M3x30 screws, quick-start sheet  
- Optional: USB-C cable, chassis adapters

🔽 Download 3D CAD (STEP) file:  
📄 [`/cad/power-receiver.step`](/cad/v1-power-receiver.step)     
📄 [`/cad/makita-2ah-battery.step`](/cad/makita-2ah-battery.step)     

---

## 📬 10. Support

Questions or issues?  
📧 Email: [contact@microver.ch](mailto:contact@microver.ch)  
🌐 Website: [https://microver.ch](https://microver.ch)

---

**Stay safe, charge smart, and power your robots responsibly.**

![Power Receiver](../images/power_receiver.jpg)

