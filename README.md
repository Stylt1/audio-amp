# 🎵 AudioAMP V1

![Status](https://img.shields.io/badge/Status-Completed-success)
![Hardware](https://img.shields.io/badge/Hardware-Open_Source-blue)
![PCB Layers](https://img.shields.io/badge/PCB-4--Layer-orange)
![EDA](https://img.shields.io/badge/EDA-KiCad-yellow)
[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-purple.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)


Welcome to the **AudioAMP V1** repository! This project features a custom-designed and efficient 4-layer Class-D stereo audio amplifier based on the popular **PAM8610** IC, delivering up to **2x 10W** output power.
Designed by **Stylt**.

---

## 📑 Table of Contents
- [✨ Key Features](#-key-features)
- [🛠️ Hardware Specifications](#️-hardware-specifications)
- [🧩 System Block Diagram](#-system-block-diagram)
- [📦 Production & Manufacturing Files](#-production--manufacturing-files)
- [📂 Repository Structure](#-repository-structure)
- [📸 Gallery & Schematics](#-gallery--schematics)
- [🚀 Getting Started](#-getting-started)
- [📝 License & Author](#-license--author)

---

## ✨ Key Features

- **Powerful Amplification:** High-efficiency **PAM8610** (Class-D) stereo amplifier providing **2x 10W** output power (into 8Ω).
- **4-Layer PCB Stackup:** 4-layer board design with dedicated power and ground planes for superior thermal dissipation, low EMI, and minimal signal crosstalk:
  - **F.Cu (Top):** Component placement & signal routing
  - **In1.Cu (Inner 1):** Solid Ground Plane (GND)
  - **In2.Cu (Inner 2):** Power Plane (+12V / VCC)
  - **B.Cu (Bottom):** Signal & secondary power routing
- **Wide Supply Voltage Range:** Operates reliably from **9V to 12V DC** via standard 5.5 x 2.1 mm DC Barrel Jack.
- **Integrated Volume & Power Control:** Quality **10K logarithmic potentiometer** with an integrated ON/OFF switch.
- **Robust Connections:** 3.5 mm AUX stereo input jack and heavy-duty green screw terminal blocks for Left (L) and Right (R) speakers.
- **Clean Audio Architecture:** Bulk **2200 µF** electrolytic decoupling capacitor on power supply lines + LC output filters (33µH/22µH inductors) for ripple noise reduction and high signal fidelity.
- **Compact & Mountable:** M2 mounting holes, precise silkscreen labeling, and integrated decorative QR code.

---

## 🛠️ Hardware Specifications

| Parameter | Specification |
| :--- | :--- |
| **Amplifier IC** | PAM8610 (Class-D Stereo) |
| **Output Power** | 10W + 10W RMS (into 8Ω @ 12V DC) |
| **Supply Voltage** | 9V – 12V DC |
| **PCB Stackup** | 4-Layer FR4 (Top, In1 [GND], In2 [PWR], Bottom) |
| **Power Connector** | 5.5 x 2.1 mm DC Barrel Jack |
| **Audio Input** | 3.5 mm Stereo AUX Jack |
| **Speaker Outputs** | Screw Terminal Blocks (Left & Right) |
| **Potentiometer** | 10K Logarithmic with ON/OFF Switch |
| **Filtration** | 2200 µF Bulk Electrolytic Cap + Output LC Filters |

---

## 🧩 System Block Diagram



<p align="center">
  <img width="2740" height="1304" alt="Snímek obrazovky 2026-08-07 v 18 47 46" src="https://github.com/user-attachments/assets/5ceffd5d-2d60-45c3-9fcd-125b2c38d460" />

</p>

---

## 📦 Production & Manufacturing Files

All production files required for manufacturing and PCBA assembly are located in the `production/` directory or under [GitHub Releases](../../releases):

- 🏭 **[Gerber Files (ZIP)](./production/gerbers/Gerber_AudioAMP_V1.zip):** Complete Gerber & Drill files for 4-layer PCB manufacturing (JLCPCB, PCBWay, etc.)
- 📊 **[Bill of Materials (BOM CSV)](./production/bom/BOM_AudioAMP_V1.csv):** Detailed component specifications and part numbers
- 🌐 **[Interactive HTML BOM](./production/bom/ibom.html):** Visual assembly guide for manual soldering
- 📐 **[Schematic (PDF)](./production/schematics/Schematic_AudioAMP_V1.pdf):** Full schematic in high-resolution PDF format

---

## 📂 Repository Structure

```text
AudioAMP-V1/
├── hardware/              # KiCad project source files (.kicad_pro, .kicad_sch, .kicad_pcb)
├── production/            # Manufacturing deliverables
│   ├── bom/               # Bill of Materials (CSV + Interactive HTML BOM)
│   ├── gerbers/           # 4-Layer Gerber files (ZIP archive)
│   └── schematics/        # Schematic diagram (PDF)
├── img/                   # Documentation graphics, 3D renders, and layer views
└── README.md              # Main project documentation
```

---

## 📸 Gallery & Schematics

### 3D Render
| Top View | Angled View |
|:---:|:---:|
| <img width="971" height="1344" alt="Snímek obrazovky 2026-08-06 v 15 42 21" src="https://github.com/user-attachments/assets/193f9201-fb71-416f-9d39-afbb3151dd46" />| <img width="2243" height="1335" alt="Snímek obrazovky 2026-08-06 v 15 40 52" src="https://github.com/user-attachments/assets/a0718cc9-ff08-498e-bb57-891cbe793cf8" />|

### 4-Layer PCB Layout

| Top Layer (F.Cu) | Inner Layer 1 (In1.Cu - GND) |
|:---:|:---:|
| <img width="1347" height="1256" alt="Snímek obrazovky 2026-08-06 v 15 07 17" src="https://github.com/user-attachments/assets/e15919ae-fc97-48ef-800a-da1e12f1fdf3" /> | <img width="1043" height="1259" alt="Snímek obrazovky 2026-08-06 v 15 07 26" src="https://github.com/user-attachments/assets/84594b02-81ca-4bdd-bb3a-f4e673fea428" />|

| Inner Layer 2 (In2.Cu - PWR) | Bottom Layer (B.Cu) |
|:---:|:---:|
| <img width="1027" height="1257" alt="Snímek obrazovky 2026-08-06 v 15 07 31" src="https://github.com/user-attachments/assets/76b6a959-e93a-4d59-9612-563feb7c95b3" /> | <img width="985" height="1260" alt="Snímek obrazovky 2026-08-06 v 15 07 37" src="https://github.com/user-attachments/assets/7d849792-37f8-401f-be16-bf2aa80e22e0" /> |

### Schematic Diagram
<img width="1553" height="1356" alt="Snímek obrazovky 2026-08-06 v 15 06 18" src="https://github.com/user-attachments/assets/68c90107-bf69-483f-a78a-7b18bfb6e8da" />

---

## 📝 License & Author

- **Designer:** Stylt
- **License:** Open-Source Hardware ([CC BY-NC-ND 4.0 License](LICENSE))

> *Built with ❤️ for electronics and audio enthusiasts.*
