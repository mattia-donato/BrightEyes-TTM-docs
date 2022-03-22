.. role:: raw-html-m2r(raw)
   :format: html


DataReceiverW
=============

The DataReceiverW is the porting of the DataReceiver for Linux to Windows. It based on the libusb-win32 driver and it is in an experimental phase.
The installation of the libusb-win32 drivers can be done with the tool Zadig. It is a software that allows to install and to switch different drivers on the USB devices in Windows. It can be downloaded the site https://zadig.akeo.ie/ .

How to install libusb-32 driver in Windows 10
---------------------------------------------


* Download Zadig from  https://zadig.akeo.ie/ 
* Run Zadig and grant the permission to change your system.
  :raw-html-m2r:`<figure> </br>
  <div align="left">
  <img src="/dataReceiver/windows/img/zadig_0.png" alt="Zadig" width="50%"/>  
  <!--<figcaption>Fig. 1 - Time-tagging principle. </figcaption>--> </br></br>
  <img src="/dataReceiver/windows/img/zadig_1.png" alt="Zadig" width="50%"/>  
  <!--<figcaption>Fig. 1 - Time-tagging principle. </figcaption>--> </br></br>
  </div>  
  </figure>` </br>
  :raw-html-m2r:`<figure></br>
  <div align="left">
  <img src="/dataReceiver/windows/img/zadig_2.png" alt="Zadig" width="50%"/>  
  <!--<figcaption>Fig. 1 - Time-tagging principle. </figcaption>--> </br></br>
  </div>  
  </figure>`\ </br>

Select in the menu **Options --> List All Devices**

:raw-html-m2r:`<figure>` </br>

:raw-html-m2r:`<div align="left">
  <img src="/dataReceiver/windows/img/zadig_3.png" alt="Zadig" width="50%"/>  
  <!--<figcaption>Fig. 1 - Time-tagging principle. </figcaption>--></br></br>
</div>`\ :raw-html-m2r:`<br>`
</figure></br>

Select in the list of devices **FX3** 

:raw-html-m2r:`<figure>`\ </br>

:raw-html-m2r:`<div align="left">
  <img src="/dataReceiver/windows/img/zadig_4.png" alt="Zadig" width="50%"/>  
  <!--<figcaption>Fig. 1 - Time-tagging principle. </figcaption>--></br></br>
</div>`\ :raw-html-m2r:`<br>`
</figure></br>

Select in the scrollbox **libusb-win32** and click on **"Replace Driver"** and wait for the installation

:raw-html-m2r:`<figure>`\ </br>

:raw-html-m2r:`<div align="left">
  <img src="/dataReceiver/windows/img/zadig_5.png" alt="Zadig" width="50%"/>  
  <!--<figcaption>Fig. 1 - Time-tagging principle. </figcaption>--></br></br>
</div>`\ :raw-html-m2r:`<br>`
</figure></br>

:raw-html-m2r:`<figure>`\ </br>

:raw-html-m2r:`<div align="left">
  <img src="/dataReceiver/windows/img/zadig_6.png" alt="Zadig" width="50%"/>  
  <!--<figcaption>Fig. 1 - Time-tagging principle. </figcaption>--></br></br>
</div>`\ :raw-html-m2r:`<br>`
</figure></br>

Now the libusb-win32 drivers should be correctly installed.

How to run DataReceiverW
------------------------

:raw-html-m2r:`<figure>`\ </br>

:raw-html-m2r:`<div align="left">
  <img src="/dataReceiver/windows/img/datawriterW.png" alt="Zadig" width="50%"/>  
  <!--<figcaption>Fig. 1 - Time-tagging principle. </figcaption>--></br></br>
</div>`\ :raw-html-m2r:`<br>`
</figure></br>

The **dataReceiverW.exe** executable file is in `dataReceiverW/x64/Debug </dataReceiverW/x64/Debug>`_. It is a command-line interface CLI software, so it is suggested to run into a Command Prompt (cmd.exe). To run correctly the dataReceiverW needs the library **libpthread.dll** and **libusb-1.0.dll**. The software crash if the subfolder **data\** is it not present in the folder where the dataReceiverW is executed.
