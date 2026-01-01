# 🛰️ GPS Time & Grid Viewer

<img width="802" height="938" alt="GPS Grid" src="https://github.com/user-attachments/assets/6f6d7711-0a4f-41a1-b896-41b71e9396db" />  

A modern Windows application for displaying **live GPS time and location data** from a serial-connected GPS receiver. Designed with **radio amateurs**, **time-nuts**, and technical users in mind.

**GPS Time & Grid Viewer** provides accurate **UTC time**, **local time**, **latitude / longitude**, **Maidenhead locator**, and **UK Ordnance Survey National Grid references** in a clean, dark-themed interface.
 
---

## ✨ Features

- 📡 Live GPS data via **Serial (COM) port**
- 🕒 **UTC time** from GPS (RMC)
- 🕰 **Local time** (system time zone conversion)
- 🌍 **Latitude & Longitude** (decimal degrees)
- 📐 **Maidenhead locator** (ham radio grid square)
- 🗺 **UK Ordnance Survey National Grid**
  - Automatically shown only when inside **Great Britain**
- 🔴🟢 Visual **connection status indicator**
- 🎨 Modern **dark UI**, fixed-size layout

---

## 🖥 Platform Support

- **Windows 10 / 11**
- **x86 (32-bit)**
- **x64 (64-bit)**
- **.NET 6 or newer**

---

## 🔌 GPS & NMEA Support

The application listens for standard **NMEA 0183** sentences from a GPS receiver.

Supported sentences:
- `$GPRMC`
- `$GNRMC`

Used data fields:
- Fix validity
- UTC time
- Date
- Latitude
- Longitude

All other sentence types are ignored safely.

---

## 🚀 Usage

1. Connect a GPS device that outputs NMEA data
2. Launch **GPS Time & Grid Viewer**
3. Select the correct **COM port**
4. Enter the **baud rate** (default: `9600`)
5. Click **Connect**

When a valid GPS fix is received, all displayed fields update automatically in real time.

---

## 📊 Display Overview

### Time
- **UTC** – directly from GPS
- **Local** – converted using your system time zone

### Location
- Latitude
- Longitude

### Ham Radio
- **Maidenhead Locator** (e.g. `IO91wm`)

### UK Mapping
- **OS National Grid Reference** (e.g. `TQ301808`)
- Automatically hidden when outside Great Britain

---

## ⚠️ Important Notice

> **Warning**  
> This software must **not** be used as a sole or authoritative location reference in emergencies.  
> Accuracy depends on GPS reception quality, antenna placement, and satellite geometry.

---

## 🛠 Technical Highlights

- Thread-safe serial input handling
- Robust NMEA sentence buffering
- Accurate Maidenhead grid calculation
- WGS-84 → OSGB36 Helmert transformation
- Transverse Mercator projection for OS grid
- Clean WinForms UI with custom styling

---

## 📜 License

Provided for **educational, experimental, and amateur radio use**.

You are free to:
- Use
- Modify
- Redistribute

No warranty is provided.

---

## 📡 Author

**UHPOWERUP**  
Amateur Radio Callsign: **2E0UMR**

- https://uhpowerup.com  
- https://2e0umr.me  
