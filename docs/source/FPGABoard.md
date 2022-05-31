# Kintex-7 evaluation board

Xilinx® FPGA Kintex-7 KC705 Evaluation Board

- *Brand:* Xilinx®
- *Product code:* EK-K7-KC705-G
- *Link to the product:* <https://www.xilinx.com/products/boards-and-kits/ek-k7-kc705-g.html>

BrightEyes-TTM is based on a commercially available and low cost [field-programmable-gate-array (FPGA)](https://en.wikipedia.org/wiki/Field-programmable_gate_array) evaluation Board (Fig.1), equipped with a state-of-the-art FPGA (the [Kintex 7](https://www.xilinx.com/products/silicon-devices/fpga/kintex-7.html), XC7K325T-2FFG900C) and a series of [I/Os connectors](docs/img/TTM_Assembly.PNG) granting an easy interface of the board with the laser scanning microscope controller, the detector(s) and the personal computer.

After having downloaded and installed [Vivado Design Suite](https://www.xilinx.com/products/design-tools/vivado.html) (Xilinx FPGA Programming software environment) the Xilinx FPGA evaluation card can be directly programmed with a standard precompiled [BrightEyes-TTM firmware](/FPGA/ttm/project/ttm.runs/impl_1/top.bit) (see the BrightEyes-TTM FPGA architecture section below for further info on the standard firmware design) or by synthesizing a new project solution starting from the low-level [VHDL/verilog open-source code](/FPGA/ttm/hdl).

:::{figure-md} img/KC705_FPGA.png
:align: center
:alt: Xilinx FPGA Board
:width: 50%

Fig.1 - Xilinx FPGA Board
:::

Follow the links below for downloading the complete project solution:

- [BrightEyes-TTM main board](/boards/FPGAboard) - the Xilinx FPGA evaluation board used in the BrightEyes-TTM project
- [BrightEyes-TTM FPGA firmware](/FPGA/ttm/project/ttm.runs/impl_1/top.bit) - .bit firmware ready to be downloaded into the evaluation FPGA board
- [BrightEyes-TTM FPGA VHDL/Verilog code](/FPGA/ttm/hdl) - VHDL and Verilog open-source codes for future TTM developments and modifications
- [Vivado Design Suite](https://www.xilinx.com/products/design-tools/vivado.html) - required Xilinx FPGA Programming software
  environment for handling the BrightEyes-TTM project

See the {doc}`BrightEyes-TTM FPGA architecture architecture.rst`
