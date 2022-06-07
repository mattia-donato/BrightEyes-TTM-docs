# Getting started
In this section you will find the hardware and software needed to build and run the BrightEyes-TTM.

## Microscope
The BrightEyes-TTM can be connected to commercial or custom imaging microscopes if they provide the following synchronization outputs:
|      |     |     |
|------|-----|-----|
| Laser SYNC | | needed |
| Pixel | | needed <br /> for imaging |
| Line | | needed <br /> for imaging |
| Frame | | needed <br /> for imaging |

The FPGA synchronization inputs have LVTTL level so if you need to adapt the signal see "MPD NIM 2 TTL" and "8xDigiBuffer" in the Hardware list here below.

### Detector
The BrightEyes-TTM channel inputs supports either LVTTL or LVDS input signals. That means it can receive signal from SPAD array detectors (which we strongly suggest) as well from ADP or PMT after CFD. Depending from the type of signal you will need to use a specific firmware and "I/O to FMC adapter board" in the Hardware list here below.

## Hardware
|      |     |     |
|------|-----|-----|
|PC  <br /> Req.: USB 3.0, >= 1.5 GHz CPU, >= 16 GB RAM, SSD hard disk, |  commercial   | needed <br /> (strongly suggested linux OS)   |
|[Xilinx Kintex-7 KC705 evaluation board](FPGABoard.md)| commercial  | |
|[CYUSB3ACC-005 FMC Interconnect Board for the EZ-USB® FX3™ SuperSpeed Explorer Kit](FMCAdapter.md)| commercial  | |
|[I/O to FMC adapter board](IOConnectorBoard.md) | custom |      |
|[MPD NIM 2 TTL](NIM2TTL.md) | commercial| strongly suggested   |
|[8xDigiBuffer](DigiBuffer.md) | custom | strongly suggested | 

## Software
|------|-----|-----|
|Your own microscope <br /> sync outputs (laser, pixel, line, frame) |  |  |
