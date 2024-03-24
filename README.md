# FPGAmp (WIP)
Customizable FPGA-Powered Guitar Amp and Effects.
## System overview
 Below is a block diagram representing the proposed concept of a system which takes in a Line In signal from the electric guitar, hands it off to the FPGA, ending with a class-D Amplifier and a speaker. 

In addition to handling guitar sound processing, the FPGA is linked to a PC via UART. This connection facilitates audio recording at 44.1 kHz and provides access to effect parameters through a GUI program, akin to traditional guitar amplifiers.

![System block diagram](/0.doc/block_diagram.png)
## Prerequisites
## Target platform and hardware
This project provides a FPGA RTL backbone, along with appropriate PC software going hand-in-hand with the running hardware. The project aims for maximum portability. The RTL is crafted with this goal in mind, allowing users to easily transfer the project to different hardware platforms without encountering major hurdles. On top of that the project is utilizing a completely open-source toolchain for deploying on FPGA. 

However, for those who wish to have a plug-and-play procedure the project is set up for the following components:

- Standalone audio CODEC
- Gowin LittleBee FPGA 
- 4 Ohm 5 W speaker
## Features

An evident benefit is that incorporating new features typically involves primarily additional coding work. In terms of functionality, the following standard components will be accessible:
 - 2 audio channels
 - Looping capability

Apart from transmitting sound to the speaker and effectively amplifying it, our design integrates numerous expandable effects, such as:
- Reverb
- Delay
- Distortion/Overdrive
- Equalization
- Tremolo
- Wah-wah

## Build
