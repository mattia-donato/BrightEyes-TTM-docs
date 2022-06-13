# DataReceiverW


The DataReceiverW is the porting of the DataReceiver for Linux to Windows. It based on the libusb-win32 driver and it is in an experimental phase.
The installation of the libusb-win32 drivers can be done with the tool Zadig. It is a software that allows to install and to switch different drivers on the USB devices in Windows. It can be downloaded the site https://zadig.akeo.ie/ .

## How to install libusb-32 driver in Windows 10

* Download Zadig from  https://zadig.akeo.ie/ 
* Run Zadig and grant the permission to change your system.

:::{figure} img/dataReceiver/zadig_0.png
:align: center
:width: 50%
:::


:::{figure} img/dataReceiver/zadig_1.png
:align: center
:width: 100%
:::

:::{figure} img/dataReceiver/zadig_2.png
:align: center
:width: 100%
:::


Select in the menu **Options --> List All Devices**

:::{figure} img/dataReceiver/zadig_3.png
:align: center
:width: 100%
:::


Select in the list of devices **FX3** 

:::{figure} img/dataReceiver/zadig_4.png
:align: center
:width: 100%
:::


Select in the scrollbox **libusb-win32** and click on **"Replace Driver"** and wait for the installation

:::{figure} img/dataReceiver/zadig_5.png
:align: center
:width: 100%
:::

:::{figure} img/dataReceiver/zadig_6.png
:align: center
:width: 100%
:::

Now the libusb-win32 drivers should be correctly installed.

## How to run DataReceiverW

:::{figure} img/dataReceiver/datawriterW.png
:align: center
:width: 100%
:::


The **dataReceiverW.exe** executable file is in [dataReceiverW/x64/Debug](/dataReceiverW/x64/Debug). It is a command-line interface CLI software, so it is suggested to run into a Command Prompt (cmd.exe). To run correctly the dataReceiverW needs the library **libpthread.dll** and **libusb-1.0.dll**. The software crash if the subfolder **data\\** is it not present in the folder where the dataReceiverW is executed.
