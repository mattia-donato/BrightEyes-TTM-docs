# I/Os SMA-FMC daugther connector card

FMC daugther card to interface the BrightEyes-TTM with external photon-signals

- *Brand:* *custom-built*
- *Product code:* *custom-built*
- **Description:** {doc}`**READ THE NOTES** <IOConnectorBoard>`
- **Gerber File:** Gerber_SMA_FMC.zip \<boards/IOconnectorBoard/Gerber_SMA_FMC.zip>

The BrightEyes-TTM interfaces with the photon-signals thanks to a custom-built I/0s FMC daughter card (Fig.1) connected via the FPGA mezzanine connector (FMC-HPC). In principle, if needed, also the I/0s FMC daughter card can be modfied, further developed and yet manufactured to adapt the BrightEyes-TTM to any type of LSM signals.

:::{figure} img/SMA_FMC_IO_daughtercard.PNG
:align: center
:alt: I/Os SMA-FMC connector Board
:width: 50%

Fig.1 - I/Os SMA-FMC connector Board
:::

The custom-built I/0s FMC daughter card interlocks with the Xilinx KC705 Evaluation kit as shown in Fig.2 below:

:::{figure} img/ConnectorBoard_connections.PNG
:align: center
:alt: ConnectorBoard_connections
:width: 50%

Fig.2 - I/Os SMA-FMC connector Board
:::

In this repository the following files are available for builing a SMA-FMC connector board:

```{eval-rst}
.. list-table::
   :header-rows: 1

   * - Name
     - Where to get
   * - Connector card gerber files
     - `Gerber_SMA_FMC.zip </boards/IOconnectorBoard/Gerber_SMA_FMC.zip>`_
   * - Connector card circuit schematic
     - `SMA_FMC-schematic.pdf </boards/IOconnectorBoard/SMA_FMC-schematic.pdf>`_
   * - Connector card pcb
     - `SMA_FMC-pcb.pdf </boards/IOconnectorBoard/SMA_FMC-pcb.pdf>`_
   * - Connector card 3D model
     - `SMA_FMC-3D.pdf </boards/IOconnectorBoard/SMA_FMC-3D.pdf>`_

```

Starting from these general open-source design files the FMC connector board can be engineered for interfacing the TTM to any type of detectors or microscope setups.

Check the tables below for the connection map:

**Pinout synchronization**

```{eval-rst}
.. list-table::
   :header-rows: 1

   * - FPGA PIN (.xdc)
     - SMA on IO connector Board
   * - J11
     - Frame
   * - J12
     - Laser SYNC
   * - J13
     - Pixel
   * - J14
     - Line
```

**Pinout channels**

```{eval-rst}
.. list-table::
   :header-rows: 1

   * - CH
     - SMA on IO connector Board
     - FMC-HPC
     - FPGA (XDC)
   * - CH1
     - J2
     - G21
     - E19
   * - CH2
     - J7
     - G22
     - D19
   * - CH3
     - J30
     - C10
     - H30
   * - CH4
     - J10
     - C11
     - G30
   * - CH5
     - J24
     - C14
     - D29
   * - CH6
     - J8
     - C15
     - C30
   * - CH7
     - J33
     - C18
     - B28
   * - CH8
     - J28
     - C19
     - A28
   * - CH9
     - J37
     - C26
     - C19
   * - CH10
     - J16
     - C27
     - B19
   * - CH11
     - J5
     - D11
     - G29
   * - CH12
     - J34
     - D12
     - F30
   * - CH13
     - J19
     - D14
     - B30
   * - CH14
     - J9
     - D15
     - A30
   * - CH15
     - J13
     - D17
     - A25
   * - CH16
     - J23
     - D18
     - A26
   * - CH17
     - J22
     - D23
     - B22
   * - CH18
     - J27
     - D24
     - A22
   * - CH19
     - J32
     - D26
     - B18
   * - CH20
     - J11
     - D27
     - A18
   * - CH21
     - J25
     - G9
     - H26
```
