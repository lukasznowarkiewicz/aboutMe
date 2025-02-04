# aboutMe

This repository contains a collection of my designs created over the years (at least a few of them worth sharing). It showcases various projects, including electronics, mechanical models, and creative builds. 

## 2024

### [HSSmartModule](https://github.com/lukasznowarkiewicz/HSSmartModule)

![](/img/HSSM-top.png)

![](/img/HSSM-bottom.png)

HSSmartModule is a work-in-progress light controller for existing electrical installations, targeting HomeSpan firmware for Apple HomeKit and featuring an ESP32-C6 with wireless connectivity (Wi-Fi 6, Bluetooth 5 LE, Thread, Zigbee). Its dual PCB design includes a low voltage board with the ESP32-C6, U.FL antenna connector, debugging buttons, and status LEDs, while the high voltage board handles power conversion from 230VAC via an LNK3204D non-insulated supply and safely reads high voltage inputs using an LTV-354T. The high voltage board also incorporates a CS5480-INZ power meter with shunt resistors, a TPS560200DBVR DC-DC converter, and relays for output control. A dedicated HSSM programmer based on the CP2102N employs optical isolation (using ADUM3160BRWZ-RL and HLK-1D0505A) to galwanically separate programmed device from the PC. Future development focused on custom firmware to fully leverage features such as power measurement, presence sensing, and Thread radio communication.

### [M2SmartHome](https://github.com/lukasznowarkiewicz/M2SmartHome)

![](/img/m2sh-photo.jpeg)

M2SmartHome is an add-on card designed to transform any M.2 2280 Key M-equipped device into a robust smart home hub by integrating onboard eMMC storage, a microSD card reader, WiFi 802.11n (via a Realtek RTL8188), and a Silicon Labs Thread radio. The board leverages a PCIe-to-USB 2.0 bridge (PI7C9X440SLBFDE) with integrated USB2244 controllers to consolidate multiple essential peripherals, addressing the limitations of low-power solutions like the Raspberry Pi. Early testing under Linux on an HP 800 G3 SFF has shown reliable eMMC and microSD performance, although further configuration of the PCIe bridge is needed. Overall, M2SmartHome offers a compact, high-performance platform for advanced smart home automation and storage needs.


### [iPhone13MiniCoolingCase](https://github.com/lukasznowarkiewicz/iPhone13MiniCoolingCase)

![](/img/iphone_12_mini_heatsink_casing_aluminium_2.png)

![](/img/iphone_12_mini_heatsink_casing_aluminium_4.png)

![](/img/first_attempts_importance_of_metal_sheets_under_glass.png)



iPhone13MiniCoolingCase is a custom-engineered, passively cooled case designed to tackle the overheating issues encountered during high-demand scenarios like continuous navigation, high screen brightness, and multi-tasking in direct sunlight. Using Fusion 360 for thermal simulations and CAD modeling, the project integrates a CNC-machined Aluminum 6061 heatsink—featuring meticulously studied geometric patterns and air channels—with a flexible, 3D-printed TPU casing, all while maintaining a slim profile comparable to commercial cases. Extensive testing revealed significant improvements, reducing the charge-up time from 3:37 to 1:50, marginally boosting Geekbench scores, and eliminating the dreaded "Charging On Hold" notification.&#x20;

### [HSRGB](https://github.com/lukasznowarkiewicz)

![](/img/hsrgb-assembled.jpeg)



Home Span RGB Control Board is a custom-designed PCB created in KiCad 8 around an ESP32-C6, initially aimed at enabling seamless integration of WS2812B LED strips with Apple HomeKit via HomeSpan firmware. The board features robust power management with a USB-C 15W input, a 3.3V LDO regulator, overcurrent protection via an AP22615 load switch, and a CP2102 USB UART bridge for easy programming, while also incorporating peripherals such as a user button and a TSOP4838 IR receiver for potential extended functionality. Basic hardware testing was carried out using both the Arduino IDE and the ESP-IDF framework, confirming that the board effectively supports fundamental HomeKit-based LED control. Future firmware enhancements—such as adding Thread radio support and expanded hardware features—are planned, marking a solid foundation for ongoing embedded development.

## 2023


### [SOM Module based on Rockchip RK3399](https://github.com/lukasznowarkiewicz/SOM_MODULE)

![](/img/SOM.PNG)

This project, completed as part of a course at Poznań University of Technology, involved designing a SOM module compatible with the FriendlyElec SOM-RK3399. The focus was on advanced high-speed PCB design, including detailed impedance calculations for various trace types and interfacing with RAM, eMMC, and Ethernet. Due to the complexity and costs associated with BGA assembly, the project remained at the conceptual stage, emphasizing the learning of advanced Altium Designer techniques.


### [CocktailMaker](https://github.com/lukasznowarkiewicz/cocktailMaker/tree/main)

![](/img/img_7755.jpeg)

cocktailMaker was built purely for fun—a prototype designed for a New Year's Eve party rather than as a commercial or groundbreaking innovation. The project evolved from an earlier engineering thesis, integrating a Raspberry Pi Zero 2 running Debian with a 7-inch touchscreen for the user interface and a Raspberry Pi Pico managing an 8-channel relay module for peristaltic pumps. The UI was developed in Python using customTkinter, while low-level control on the Pi Zero was handled in C. With a mechanical structure designed in Fusion 360 and assembled using extruded V-slot 2020 profiles, 3D-printed parts, and milky plexiglass panels, the cocktailMaker performed reliably for an 8-hour stretch, making it a fun and successful experiment for the event.



### [TeaMachine](https://github.com/lukasznowarkiewicz/teaMachine)



![](/img/teamachineassembly_rev_10_front.png)

![](/img/ekspres1.png)

![](/img/ekspres2.png)

teaMachine was conceived as an academic project to create a modular, automated tea maker that integrates mechanical design, embedded hardware, and multi-platform software to streamline tea preparation much like modern coffee machines. The project leverages a custom Raspberry Pi Pico control board (designed in KiCad) running C++ firmware, with control interfaces developed across platforms—from Windows 10 IoT Core (.NET Core) and Debian (Vue + Vite) to Python with customTKinter—all housed within a robust mechanical structure built from 2020 aluminum profiles, copolycarbonate panels, and 3D-printed components designed in Fusion 360. It employs both high-voltage SSRs and low-voltage mechanical relays to manage components such as heaters, pumps, and motors, while integrating various sensors and user interfaces for comprehensive system control. Ultimately, teaMachine served as an extensive academic project that successfully demonstrated cross-disciplinary integration and iterative development, providing valuable insights into mechatronics, embedded systems, and software engineering.

## 2022

### [Plant growing containers](https://github.com/lukasznowarkiewicz/PlantGrowingContainers)

![](/img/render1.png)

\### PlantGrowingContainers

PlantGrowingContainers was initiated as a research platform to study the impact of electromagnetic fields on plant growth by comparing controlled and experimental samples in two remotely managed, automated boxes. The system is built around an ESP32 microcontroller that gathers environmental data from sensors measuring temperature, humidity, light intensity, magnetic forces, and atmospheric pressure, while an 8-relay module controls actuators like fans, LED strips, and a peristaltic pump for irrigation. The hardware design features a robust power supply that steps down from 230VAC to 12VDC and 5VDC, and the mechanical framework is meticulously crafted in Fusion 360 using V-slot aluminum profiles, plywood enclosures, and custom 3D-printed components. Additionally, an ESP32 camera module paired with a local server and [Filka.io](http://Filka.io) integration enables continuous image capture and real-time data visualization to support comprehensive research analysis.

## 2021

### Wireless charging system

![](/img/antenna.png)

![](/img/wireless_charging.png)

## 2020

### [Emersense](https://github.com/lukasznowarkiewicz/Emersense)

![](/img/emersense_in_car.png)

Emersense was an attempt to develop a system for alerting drivers about approaching emergency vehicles amid urban noise, using an ESP32 running custom C code on ESP-IDF. The device combined an INMP441 MEMS microphone with a legacy electret mic to capture audio signals and used DFT-based processing to identify two-tone sirens. Its hardware also included a CP2102N for USB connectivity, an XL1509 for voltage conversion, a SI4713 FM transmitter with RDS, an MPU-6050 for motion detection, and an SPI-driven LCD—all integrated on a custom KiCad PCB and housed in a Fusion 360–designed enclosure. Although preliminary testing offered some insights, various challenges in signal processing and resource limitations ultimately led to the project’s discontinuation, providing valuable lessons rather than a market-ready solution.

## 2018 - 2019

### [Appliance connector]()

![](/img/casing_like_droplet.png)

![](/img/appliance_connector_gui.png)

Appliance Connector was developed to bridge the gap between legacy devices—such as IR-controlled TVs, RS232-based projectors, and dry contact systems—and modern smart home networks using TCP/IP and REST APIs. Built around an ESP32 module running ESP-IDF FreeRTOS, the project features custom firmware in C that handles IR transmission/reception, UART, LED, and relay control, along with a minimalist web UI crafted in HTML/CSS/JavaScript for device management. The hardware design, prototyped in Autodesk Eagle and Fusion360 with iterative 3D-printed enclosures, evolved into a two-board solution integrating both sensor/IR functions and terminal interfacing. Ultimately, while the prototype showcased promising integration capabilities, the project was abandoned due to academic commitments and emerging commercial alternatives, leaving behind valuable insights in smart home connectivity.

## 2017

### [DeafAlDer](https://github.com/lukasznowarkiewicz/DeafAlDer)

![](/img/deaf_al_der.jpg)

DeafAlDer was conceived to address the need for an accessible, multimodal home alert system tailored for the deaf community, delivering clear visual, tactile, and low-frequency auditory signals to notify users of everyday events and emergencies. The system’s core is a Siemens LOGO! 12/24 RCE PLC that orchestrates a range of custom-designed sensor and actuator modules—including flood and smoke/CO detectors, a kitchen timer, a doorbell, and an ATmega8-based alarm clock with vibration feedback—integrated via Altium-designed PCBs and housed in 3D-printed enclosures from Autodesk Inventor models. Firmware development leveraged Logo Soft Comfort for PLC programming and the Eclipse IDE with C for microcontroller applications, ensuring seamless integration between both proprietary and commercial sensors. Rigorous debugging and iterative enhancements have resulted in a robust, scalable, and cost-effective solution that meets its design specifications, with promising avenues for future improvements such as enhanced gesture sensor performance and broader system integration.

## 2016

### [3dCane]()

![](/img/cane_in_the_field.jpg)

3dCane was developed to empower visually impaired users by providing an intelligent cane that performs 3D environmental scanning and offers both tactile and audio feedback for safer navigation. The system is built around dual 8-bit AVR microcontrollers (ATmega64 in the cane and ATmega328P in the wristwatch), integrating US-015 ultrasonic sensors, NRF24L01 radio modules, ADXL accelerometers, a DS3231 RTC, and microSD storage, with firmware written in C using Eclipse Indigo. The prototype successfully demonstrated real-time obstacle detection and user alerts through robust testing and custom PCB assembly using both THT and SMT techniques. Although the project showcased promising results in competitive innovation, limitations in sensor data processing, communication range, and unfinished features like illumination highlight areas for further refinement.

## 2010 - 2015

### Bluetooth Speaker
![Bluetooth Speaker](img/bluetooth_speaker.png)

### Wind Turbine Model
![Wind Turbine Model](img/wind_turbine_model.png)

### Christmas Tree
![Christmas Tree](img/christmas_tree.png)

### Jacob's Leather
![Jacob's Leather](img/jacbos_leather.png)

### Light Control Module
![Light Control Module](img/light_control_module.png)

### Useless Box
![Useless Box](img/useless_box.png)

### Building Model
![Building Model](img/building_model.png)
