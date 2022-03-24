
Hardware list
=============

In the table below you can find the complete list of all the needed hardware components for builing the BrightEyes-TTM.

Xilinx® KC705 Evaluation Board
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- Kintex-7 evaluation board for the BrightEyes-TTM
- *Brand:* Xilinx®
- *Product code:* EK-K7-KC705-G
- *Link to the product:* https://www.xilinx.com/products/boards-and-kits/ek-k7-kc705-g.html
- **How-To / Firmware**: read here `<FPGABoard>`


EZ-USB® FX3™ SuperSpeed Explorer Kit
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- USB board for data transmission from the FPGA to a host-PC
- *Brand:* Cypress®
- *Product code:* CYUSB3KIT-003 EZ-USB
- *Link to the product:* https://www.cypress.com/documentation/development-kitsboards/cyusb3kit-003-ez-usb-fx3-superspeed-explorer-kit
- **How-To / Firmware**: read here <boards/USB3.0>

FMC Interconnect Board for the EZ-USB® FX3™
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- FMC adapter connector card to interconnect a Xilinx® FPGA board with the EZ-USB® FX3™ SuperSpeed Explorer Kit
- *Brand:* Cypress®
- *Product code:* CYUSB3ACC-005
- *Link to the product:* https://www.cypress.com/documentation/development-kitsboards/cyusb3acc-005-fmc-interconnect-board-ez-usb-fx3-superspeed
- **How-To / Firmware**: read here <boards/USB3.0/FMCadapter>


I/Os SMA-FMC daugther connector card
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- FMC daugther card to interface the BrightEyes-TTM with external photon-signals 
- *Brand:* *custom-built*
- *Product code:* *custom-built*
- **Description:** </boards/IOconnectorBoard>
- **Gerber File:** Gerber_SMA_FMC.zip <boards/IOconnectorBoard/Gerber_SMA_FMC.zip>


Optional hardware parts
^^^^^^^^^^^^^^^^^^^^^^^


NIM to TTL converter
--------------------
- Signal converter module capable to convert an input NIM pulse to a Low Voltage TTL for triggering the laser sync out and feeding it to the 
- *Brand:* MPD
- *Product code:* MPD NIM 2 TTL
- *Producer link:* http://www.micro-photon-devices.com/Products/Instrumentation/NIM2TTL-Converter
- **How-To / Firmware**: Gerber_SMA_FMC.zip <boards/IOconnectorBoard/Gerber_SMA_FMC.zip>

8xDigiBuffer
------------
- I/O multichannel (8x) digital buffer to match the impedance of external reference signals with the input impedance of the Xilinx® KC705 Evaluation kit
- *Brand:* *custom-built*
- *Product code:* *custom-built*
- **Description:** <boards/8xDigiBuffer>
- **Gerber File:** `8xDigiBuffer_Gerber.zip <boards/8xDigiBuffer/files/DigiBuff8_rev2_GerberFiles.zip>`_
   


**BrightEyes-TTM operation**

.. list-table::
   :header-rows: 1

   * - 
     - 
   * - PC interface
     - USB 3.0 SuperSpeed
   * - PC requirements
     - min. 1.5 GHz CPU clock, min. 16 GB RAM memory, SSD hard disk
   * - Operating system
     - Linux (native) / Windows (ported)

.. toctree::
   FPGABoard
   USB3
   FMCadapter
   IOconnectorBoard
   8xDigiBuffer
