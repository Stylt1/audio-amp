View this project on [CADLAB.io](https://cadlab.io/project/30509). 

# 🎵 AudioAMP V1

![Status](https://img.shields.io/badge/Status-Completed-success)
![Hardware](https://img.shields.io/badge/Hardware-Open_Source-blue)
![PCB Layers](https://img.shields.io/badge/PCB-4--Layer-orange)
![EDA](https://img.shields.io/badge/EDA-KiCad-yellow)
[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-purple.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

This project features a custom-designed and efficient 4-layer Class-D stereo audio amplifier based on the popular **PAM8610** IC, delivering up to **2x 10W** output power.
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
    <img width="2740" height="1304" alt="BlockDiagram" src="https://github.com/user-attachments/assets/72f61a8e-5d86-40e7-8b3a-f42004b35f66" />


</p>

---

## 📦 Production & Manufacturing Files

All production files required for manufacturing and PCBA assembly are located in the `production/` directory or under [GitHub Releases](../../releases):


---

## 📂 Repository Structure

```text
AudioAMP-V1/
├── hardware/              # KiCad project source files (.kicad_pro, .kicad_sch, .kicad_pcb)
├── img/                   # Documentation graphics, 3D renders, and layer views
├── production/            # Manufacturing deliverables
│   ├── bom/               # Bill of Materials (CSV)
│   ├── gerbers/           # 4-Layer Gerber files (ZIP archive)
│   └── schematics/        # Schematic diagram (PDF)
├── LICENSE.txt            # License
└── README.md              # Main project documentation
```

---

## 📸 Gallery & Schematics

### 3D Render
| Top View | Angled View |
|:---:|:---:|
| <img width="909" height="1336" alt="Top" src="https://github.com/user-attachments/assets/feff9031-86a0-4d03-be18-47cd55577b35" />| <img width="2417" height="1343" alt="Angle frontleft" src="https://github.com/user-attachments/assets/9a42c538-1c57-48ca-b0b9-cee50218d111" />|

### 4-Layer PCB Layout

| Top Layer (F.Cu) | Inner Layer 1 (In1.Cu - GND) |
|:---:|:---:|
| <img width="1347" height="1256" alt="F Cu" src="https://github.com/user-attachments/assets/2611ad77-9ca9-4f3d-9520-ee8e6831e674" />| <img width="1043" height="1259" alt="In1 Cu" src="https://github.com/user-attachments/assets/0017a4ce-5c38-46d5-b543-d16e475f7059" />|

| Inner Layer 2 (In2.Cu - PWR) | Bottom Layer (B.Cu) |
|:---:|:---:|
| <img width="1027" height="1257" alt="In2 Cu" src="https://github.com/user-attachments/assets/1d90d841-72d0-4569-82bc-e39c5f569468" />| <img width="985" height="1260" alt="B Cu" src="https://github.com/user-attachments/assets/34eb496e-ffb1-45eb-8bda-2e6d4e63b926" />|

### Schematic Diagram
<img width="1553" height="1356" alt="Snímek obrazovky 2026-08-06 v 15 06 18" src="https://github.com/user-attachments/assets/68c90107-bf69-483f-a78a-7b18bfb6e8da" />

---

## 📝 License & Author

- **Designer:** Stylt
- **License:** ([CC BY-NC-ND 4.0 License](LICENSE))


