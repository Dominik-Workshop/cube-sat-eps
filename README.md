# EPS - Electric Power System

## Used tools:
<img align="center" height="64" src="images/logos/Altium_Designer.jpg">&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; 
<img align="center" height="64" src="images/logos/STM32CubeIDE.png">

# Project Overview
This project is part of a CubeSat prototype built as a group project at Wrocław University of Science and Technology. [GitLab Repository](https://gitlab.com/wust-satellite)
<img align="center" src="images/photos/PCB_top-no-background.png">
The primary functions of this board are:

1. **Battery Management**:
    - Charging a 1S Li-ion battery pack using Maximum Power Point Tracking (MPPT).
    - Monitoring the battery voltage.

2. **Power Conversion**:
    - Generating stable 5V and 3.3V power rails to supply various components of the system.

3. **Communication**:
    - Establishing UART communication with a radio board for data transmission and control.

4. **Deployment of Solar Panels and Radio Antenna**:
    - Providing two power outputs capable of driving high current to external resistors, which can burn wires to deploy the solar panels and antenna.

5. **Remove Before Flight (RBF) Circuit**:
    - Ensuring that the satellite starts operation only after ejection from the launch vehicle.

> [!NOTE]
> Certain features, such as current monitoring and switches on all power lines, were omitted due to time constraints.

# Project Status ✅
The `Electric Power System` has been fully tested, confirming that **all** its intended functions **operate as expected**. The development of both the PCB and the corresponding code is complete, and this specific board is no longer under active development. Notably, the `EPS` was successfully integrated into our `CubeSat` prototype, which was assembled and was operating as planned. It is important to remember that this is a **prototype** and, despite its successful operation, certain features were omitted due to time constraints, as noted earlier. Therefore, this `EPS` design is not yet ready for use in a final `CubeSat` intended for space deployment.

# Schematic
<img align="center" src="images/schematics/schematic_top_sheet.png">

The image above shows the top sheet of the `EPS` schematic. The complete schematic diagram, including all sheets, is available as a `PDF` file and can be accessed [here](/pcb/Project%20Outputs%20for%20EPS_board/EPS_full_schematic.pdf).
 

# PCB
<img align="center" src="images/renders/EPS_top_angle.png">
<img align="center" src="images/renders/EPS_top.png">
<img align="center" src="images/renders/EPS_bottom.png">

# Project structure
```
.
├── images
│   ├── logos
│   ├── photos
│   ├── renders
│   └── schematics
├── pcb
│   ├── ***Altium schematic and PCB Documents***
│   ├── ***Altium CAMtastic Documents***
│   ├── ***other Altium files***
│   ├── Lib
│   │   └── ***My parts libraries***
│   └── Project Outputs for EPS_board
│       ├── EPS_full_schematic.pdf
│       ├── ***Gerber and NC drill files***
│       └── EPS_gerber_files.zip
├── code
│   └── ***STM32CubeIDE project***
└── README.md
```
