
Requirements
^^^^^^^^^^^^

.. code-block::

   sudo apt-get install libusb-dev libusb-1.0-0-dev

How to compile?
^^^^^^^^^^^^^^^

.. code-block::

   gcc "dataReceiver.c" -O2 -g `pkg-config libusb-1.0 --libs --cflags`  -lpthread -o "dataReceiver"
