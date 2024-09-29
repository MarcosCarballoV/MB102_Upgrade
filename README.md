# Custom MB102 PCB Design in Altium Designer
[![Altium Designer](https://img.shields.io/badge/Altium-21.0-blue.svg)](https://www.altium.com/)

## Overview
This project presents a custom PCB design created in Altium Designer, improving upon the original MB102 power supply module. Key upgrades include LiPo battery support, dynamic power management, USB-C connectivity, and enhanced power control with dual SEPIC switching regulators. Additional features such as configurable SMD buttons, battery monitoring, and independent power source control make this board highly versatile. The design files are ready for manufacturing through JLCPCB or PCBWay.

<p align="center">
  <img src="https://github.com/user-attachments/assets/76ecc2ea-a4ce-4063-a1a3-5192372483a4" alt="MB102_Upgrade">
  <br>
  <em>MB102_Upgrade Render</em>
</p>

## Key Features

- **LiPo Battery Support:** 1-cell LiPo with JST-PH connector.
- **Dynamic Power Path Management:** Optimized LiPo charging and power distribution.
- **USB-C Connector:** Modern interface for power and data.
- **Power Switch:** Full device shutdown capability.
- **Configurable SMD Buttons:** With pull-down/pull-up resistors.
- **Dual SEPIC Switching Regulators:** 5V and 3.3V outputs.
- **3.3V LDO:** For low-power sleep modes.
- **Battery Monitoring:** MOSFET-controlled resistive divider for accurate readings.
- **Battery Status Indicator:** Charging/full status pins.
- **Independent Power Control:** Enable/disable 3.3V or 5V regulators individually.


## Ordering the PCB (JLCPCB/PCBWay)

### JLCPCB
To order this PCB from JLCPCB:
1. **Download Gerber Files:** The necessary Gerber files are included in the `Project Outputs for MB102_Upgrade/MB102_Upgrade_GerberFiles.zip` directory of this repository.
2. **Upload to JLCPCB:**
   - Go to [JLCPCB's website](https://jlcpcb.com/).
   - Click on "Quote Now" and upload the Gerber files.
   - Select your desired options for layer count, color, and PCB thickness.
3. **Order and Checkout:** Complete your order by choosing the shipping method, and submit the payment.

### PCBWay
To order from PCBWay:
1. **Download Gerber Files:** The files are compatible with PCBWay’s system and can be found in the `Project Outputs for MB102_Upgrade/MB102_Upgrade_GerberFiles.zip` folder.
2. **Upload to PCBWay:**
   - Go to [PCBWay's website](https://www.pcbway.com/).
   - Click "Quote Now" and upload the Gerber files.
   - Customize your PCB options like color and surface finish.
3. **Proceed to Checkout:** Finalize your order and select the appropriate shipping option.

## Improvements Over the MB102

This custom PCB offers several key improvements over the MB102:

</p>
<p align="center">
    <img src="https://github.com/user-attachments/assets/400febef-be6c-4d22-964d-fbb57746e161" alt="MB102 Origin" style="width: 40%; height: auto;">
    <img src="https://github.com/user-attachments/assets/e979c19c-0622-45e9-90ac-3940d0b9b2be" alt="B102 Improvements" style="width: 45%; height: auto;">
  <br>
  <p align="center">
  <em>Comparison of MB102 Original vs. MB102 Upgrade</em>
</p>



- **Power Supply:** Added support for a 1-cell LiPo battery with a 2-pin JST-PH connector (without NTC).
- **Dynamic Power Path Management:** Integrated LiPo battery charger with dynamic power path management for optimized power distribution.
- **USB-C Connector:** Upgraded to a USB-C connector for modern power and data interfaces.
- **Power Control:** Equipped with a switch for complete device shutdown.
- **Configurable Buttons:** SMD buttons configurable with pull-down or pull-up resistors.
- **Advanced Power Regulation:** SEPIC-type switching regulators providing stable 5V and 3.3V outputs.
- **Low Power Consumption:** Added a 3.3V LDO for projects utilizing microcontroller sleep modes.
- **Battery Monitoring:** Battery level measurement using a resistive divider controlled by MOSFETs for accurate readings.
- **Battery Status Indicator:** Pin and indicator for battery status notifications (charging or fully charged).
- **Independent Power Control:** Pins available to individually enable or disable each switching regulator (3.3V or 5V).

<p align="center">
  <img src="https://github.com/user-attachments/assets/0e931d75-1580-4409-a22c-91d21e2e97ff" alt="Schematic of MB102 Origin page 1" style="width: 35%; height: auto;">
  <img src="https://github.com/user-attachments/assets/36ffdd20-7dbd-4bee-8e7d-760339191f31" alt="Schematic of MB102 Origin page 2" style="width: 30%; height: auto;">
  <img src="https://github.com/user-attachments/assets/60095534-64b9-41b9-9af6-1bb06fc202c8" alt="Schematic of MB102 Origin page 3" style="width: 30%; height: auto;">
  <br>
  <em>Schematic of MB102 Upgrade</em>
</p>

## Assembly and Testing

### Physical Assembly
The board was assembled using through-hole and surface-mount components. Special attention was paid to the orientation and placement of key components to ensure that the layout matches the design.

<p align="center">
  <img src="" alt="PCB Assembly">
  <br>
  <em>Assembly of the PCB</em>
</p>

### Electrical Testing
After assembly the boards, the following tests:
- **Continuity Tests:** Ensured that all connections were properly made without any shorts or open circuits.
- **Power-On Test:** Verified the correct voltage outputs (5V and 3.3V) with no significant voltage drops.
- **Load Testing:** The board was tested under different loads to verify that it could maintain stable output voltage without overheating or overloading the components.



## Future Work
Currently, we are working on miniaturizing the design further to make it suitable for portable applications. The next iteration will focus on reducing size while maintaining power efficiency and stability.

## Authors

- [@tu_usuario](https://github.com/tu_usuario)
