# Assembly Instructions

The Xilinx® KC705 Evaluation board, the Cypress® FX3™ SuperSpeed Explorer Kit and the connector card can be easily stacked together, using FMC connectors, as shown below (Fig. 3). I/Os connections are also labeled for a more intuitive assembly and mapped in the [I/O pins table](IOConnectorBoard.md) which shows the correspondence between inputs (typically the digital output from the SPAD array detector elements, named photon chaneels) and the connection pins. For a correct use of the BrightEyes-TTM the [dip switches](https://en.wikipedia.org/wiki/DIP_switch) in the orange BOX (always Fig.3) should be all set to the OFF position.

The Cypress® FX3™ SuperSpeed Explorer Kit board interlock into the FMC-LPC connector block. While the I/Os connector cards is connected to the FMC-HPC connector.

:::{figure} img/TTM_Assembly.PNG
:align: center
:alt: Assembly
:width: 3500

Fig.3 - BrightEyes-TTM detailed assembly.
:::

In the current application CH11 on J5 input connector board is internally duplicated and sampled with a 400MHz clock and returned as output on pin J17. This feature allow to monitor CH11 activity and content while it is still connected and used into the TTM design (Fig.4).

:::{figure} img/TTM_ch11_duplication.PNG
:align: center
:alt: Assembly
:width: 600

Fig.4 - CH11 duplication pin map
:::
