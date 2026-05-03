# Wireless-Power-Hub-PCB-STWLC38-TP4056-Power-Management-Board
A compact, circular wireless power receiver and Li-ion battery management PCB. Features the STWLC38JRM for Qi-compliant wireless charging, TP4056 for battery charging, TPS259521 eFuse for robust output protection, and AP2112K 3.3V LDO. Ideal for custom power banks and portable IoT devices.
# Wireless Power Hub PCB (STWLC38JRM + TP4056)

![EasyEDA](https://img.shields.io/badge/Designed_in-EasyEDA-blue)
![License](https://img.shields.io/badge/License-MIT-green)

This repository contains the complete hardware design files for a **Wireless Power Hub**. This board is designed to harvest energy from a Qi wireless charging pad, manage a Lithium-Ion battery, and provide a stable, protected power output. Its circular form factor makes it perfect for embedding into custom electronics, power banks, or wearable devices.

![3D Render](images/3d_render.png) <!-- Make sure to add the 3D render image in an images/ folder -->

## ✨ Key Features
--------------------------------------------
<img width="2003" height="1303" alt="Schematic_Power_HUB-copy-copy-copy_2026-05-02" src="https://github.com/user-attachments/assets/9778a75e-2c73-43bb-8b7c-2dfa9bda1ddd" />

--------------------------------------------
<img width="602" height="567" alt="Power_HUB_PCB_3D_Top_View" src="https://github.com/user-attachments/assets/ad8bc3d6-70dc-42c1-942b-7114a028cd6a" />

--------------------------------------------
<img width="647" height="655" alt="Power_HUB_PCB_3D_Bottom_View" src="https://github.com/user-attachments/assets/023f13c0-9d1c-422b-8aa7-335019a1c89c" />

--------------------------------------------
<img width="560" height="525" alt="Power_HUB_PCB_2D_View" src="https://github.com/user-attachments/assets/c46ff970-1255-45b5-88f3-0ed95b5c121d" />

--------------------------------------------
*   **Wireless Input:** Qi-compliant wireless charging receiver utilizing the **STWLC38JRM** (STMicroelectronics) IC. Handles AC-to-DC rectification and power control.
*   **Battery Management:** Classic **TP4056** charging IC with charge/discharge protection circuitry, supporting 1-cell Li-Ion/Li-Po batteries.
*   **Power Protection & Output:** Uses the **TPS259521DSGR** (TI) eFuse IC for intelligent over-current/over-voltage protection on the output path.
*   **System Voltage:** Dedicated **AP2112K-3.3** LDO regulator for stable 3.3V logic supply.
*   **Low Profile Design:** Circular PCB layout optimized for integration into spaces with a wireless coil.
*   **Interface:** 
    *   **CN3:** 2-pin JST connector for battery connection.
    *   **U4:** 8-pin JST I2C breakout (useful for communicating with the STWLC38 and monitoring its status).
    *   **Test Points:** `TP_VOUT`, `TP_VCC`, `TP_VRECT`, `TP_ENB`, `TP_AC1/2` for easy debugging and prototyping.
    *   **U7:** Jumper selectable for configuration.

## 📂 Repository Structure
```text
/
├── images/                                   # 3D renders and PCB images
├── Schematic_Power_HUB_2026-05-02.pdf        # Full circuit schematics
├── PCB_PCB_Power_HUB_2026-05-02.pdf          # PCB layout traces
├── BOM_Power_HUB_2026-05-02.csv             # Bill of Materials (LCSC)
└── PickAndPlace_PCB_Power_HUB_2026-05-02.csv # Pick & Place file for assembly
