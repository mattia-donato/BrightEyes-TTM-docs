
Hardware list
=============

In the table below you can find the complete list of all the needed hardware components for builing the BrightEyes-TTM.

.. list-table::
   :header-rows: 1

   * - Name
     - Product code
     - Brand
     - Description
     - Where to get
   * - Xilinx® KC705 Evaluation Board
     - EK-K7-KC705-G
     - Xilinx®
     - :ref:`Kintex-7 evaluation board for the BrightEyes-TTM <FPGABoard>`
     - https://www.xilinx.com/products/boards-and-kits/ek-k7-kc705-g.html
   * - EZ-USB® FX3™ SuperSpeed Explorer Kit
     - CYUSB3KIT-003 EZ-USB
     - Cypress®
     - `USB board for data transmission from the FPGA to a host-PC <boards/USB3.0>`_
     - https://www.cypress.com/documentation/development-kitsboards/cyusb3kit-003-ez-usb-fx3-superspeed-explorer-kit
   * - FMC Interconnect Board for the EZ-USB® FX3™ SuperSpeed Explorer Kit
     - CYUSB3ACC-005
     - Cypress®
     - `FMC adapter connector card to interconnect a Xilinx® FPGA board with the EZ-USB® FX3™ SuperSpeed Explorer Kit <boards/USB3.0/FMCadapter>`_
     - https://www.cypress.com/documentation/development-kitsboards/cyusb3acc-005-fmc-interconnect-board-ez-usb-fx3-superspeed
   * - I/Os SMA-FMC daugther connector card
     - custom-built
     - custom-built
     - `FMC daugther card to interface the BrightEyes-TTM with external photon-signals </boards/IOconnectorBoard>`_
     - `Gerber_SMA_FMC.zip <boards/IOconnectorBoard/Gerber_SMA_FMC.zip>`_


**Optional hardware parts**

.. list-table::
   :header-rows: 1

   * - Name
     - Product code
     - Brand
     - Description
     - Where to get
   * - NIM to TTL converter
     - MPD NIM 2 TTL
     - MPD
     - Signal converter module capable to convert an input NIM pulse to a Low Voltage TTL for triggering the laser sync out and feeding it to the BrightEyes-TTM
     - http://www.micro-photon-devices.com/Products/Instrumentation/NIM2TTL-Converter
   * - 8xDigiBuffer
     - custom-built
     - custom-built
     - `I/O multichannel (8x) digital buffer to match the impedance of external reference signals with the input impedance of the Xilinx® KC705 Evaluation kit <boards/8xDigiBuffer>`_
     - `8xDigiBuffer_Gerber.zip <boards/8xDigiBuffer/files/DigiBuff8_rev2_GerberFiles.zip>`_


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
