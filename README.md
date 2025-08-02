# 🔌 Makita Power Receiver – microver.ch

The **V1 Power Receiver** is a rugged, smart interface that lets you power your robots using standard **Makita 18V batteries**.  
It features USB-C PD charging/discharging, a built-in fuse, and direct DC outputs — all in a mountable, field-friendly form factor.

---

## 🚀 Features

- 🔋 Standard Makita 18V Li-Ion battery slot
- 🔌 USB-C PD/QC port for charging & discharging (PMIC-controlled)
- ⚡ 3x 2.1mm DC barrel jacks (direct battery output)
- 🔥 Integrated 5×20mm glass fuse holder with 10A fuse
- 🧷 Mountable with 3x M3x30 screws
- 📦 Compact and tough: 72mm × 94mm × 42mm

---

## ⚡ What It Does

| Mode         | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| USB-C Charge | Safely recharges Makita 18V batteries via USB-C (CC-CV, 2A @ ~21V)          |
| USB-C Power  | Smart power bank for 5V–20V USB-C devices (up to 100W)                      |
| DC Output    | Access full battery power from 3x DC jacks — for motors, controllers, etc. |

---

## 🧠 Smart Power Management

The onboard **PMIC** negotiates with devices and chargers using:

- USB-C 3.0A / PD2.0 / PD3.0
- QC3.0, Apple 2.4A, Samsung AFC, Huawei FCP/SCP

### Discharge Limits:

- 5V/3A (15W)  
- 9V/3A (27W)  
- 12V/3A (36W)  
- 15V/3A (45W)  
- 20V/5A (100W)

> ❗ To activate USB-C power mode, plug into a wall charger for 2–3s with battery inserted, then switch to your device.

---

## 🛡️ Safety Built-In

- ✅ USB-C PMIC over-voltage, under-voltage, and current limit protections  
- 🔥 10A replaceable glass fuse on DC output  
- 🔌 Use only USB-C for charging (not DC jacks!)  
- 🧯 Remove fuse while debugging your circuit

---

## 📏 Mechanical Specs

- Dimensions: **72 × 94 × 42 mm**
- Screw Mount Pattern: **44 mm × 50 mm**
- Screws: **3x M3×30** (included)

![Mount Diagram](images/mounting_diagram.jpg)

---

## 📈 Battery Guidelines

| Voltage (V) | Estimated Charge (%) |
|-------------|-----------------------|
| 21.0        | 100%                  |
| 19.5        | 75%                   |
| 18.0        | 33%                   |
| 15.0        | 0% (cutoff)           |

> ⚠️ Never probe battery terminals directly. Use a barrel jack + voltmeter.  
> ⚠️ Below 15.0V risks permanently disabling Makita packs.

---

## 📦 What's in the Box

- ✅ 1x Power Receiver  
- 🔩 3x M3x30 mounting screws  
- 📄 Quick-start instruction sheet  
- 📁 [Power Receiver STEP File](./cad/v1-power-receiver.step)
- 📁 [Makita 2Ah Battery STEP File](./cad/makita-2ah-battery.step)

---

## 🛒 Purchase

Buy now at 👉 [shop.microver.ch](https://shop.microver.ch)

---

## 📚 Documentation

📖 Full documentation available in [`docs/README.md`](./docs/README.md)

---

## 📬 Contact & Support

Need help or want to integrate with your system?  
📧 [contact@microver.ch](mailto:contact@microver.ch)  
🌐 [microver.ch](https://microver.ch)

---

**Power up your robots. Safely. Intelligently. Anywhere.**

![Power Receiver Product Image](images/power_receiver.jpg)

