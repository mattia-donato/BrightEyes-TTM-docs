Operational software list
=========================

Softwares tools for the BrightEyes-TTM FPGA programming and data acquisition.

.. list-table::
   :header-rows: 1

   * - Name
     - Description
     - Where to get
   * - Vivado Design Suite®
     - Xilinx® FPGA Programming software environment
     - https://www.xilinx.com/products/design-tools/vivado.html
   * - Python 3
     - Python environment to run the analysis softwares
     - https://www.python.org/download/releases/3.0/
   * - BrightEyes-TTM custom Python 3 libraries
     - In order to be able to reconstruct and process the data streamed by the BrightEyes-TTM few python libraries have to be previously installed in the host-processing computer
     - `dataProcessing <dataProcessing>`_
   * - Data acquisition software (Linux)
     - The data receiver is a CLI program for reading the data from the TTM through the USB 3.0 and write them to the PC memory. It is program written in C/C++ developed for Linux OS.
     - `dataReceiver (Linux) <dataReceiver/linux>`_
   * - Data acquisition software (Windows)
     - Here a version of the data receiver ported to Windows OS. Please note that the Linux version is our reference version for measurments and tests.
     - `dataReceiverW (Windows) <dataReceiver/windows>`_


Analysis software list
======================

In order to give the user some preliminary tools to process, reconstruct and use the acquired TTM data we developed 3 main examples using Jupyter Notebook and we provide the associated examples dataset on `Zenodo <https://doi.org/10.5281/zenodo.4912656>`_. Explore the `data processing and analysis section <dataProcessing>`_ for further info.

.. list-table::
   :header-rows: 1

   * - Name
     - Description
     - PDF version
     - Where to get
     - Associated example dataset on Zenodo
   * - TSCPC Histogram
     - Jupyter Notebook example for TCSPC histogram reconstruction
     - `TCSPC_Histogram_reconstruction.pdf <dataProcessing/pynotebook/PDF/TCSPC_Histogram_reconstruction.pdf>`_
     - `TCSPC_Histogram_reconstruction.ipynb <dataProcessing/pynotebook/TCSPC_Histogram_reconstruction.ipynb>`_
     - **Fluorescence_Spectroscopy_Dataset_40MHz** 
     
     .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4912656.svg
        :target: https://doi.org/10.5281/zenodo.4912656
        :alt: DOI
     
   * - Imaging
     - Jupyter Notebook example for intensity images as well as FLIM images reconstruction
     - `Image_reconstruction.pdf <dataProcessing/pynotebook/PDF/Image_reconstruction.pdf>`_
     - `Image_reconstruction.ipynb <dataProcessing/pynotebook/Image_reconstruction.ipynb>`_
     - **FLIM_512x512pixels_dwelltime250us_Dataset_40MHz** 
     
     .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4912656.svg
        :target: https://doi.org/10.5281/zenodo.4912656
        :alt: DOI
     
   * - FCS
     - Jupyter Notebook example for calculating fluorescence correlation curve
     - `FCS.pdf <dataProcessing/pynotebook/PDF/FCS.pdf>`_
     - `FCS.ipynb <dataProcessing/pynotebook/FCS.ipynb>`_
     - **FCS_scanfcs_Dataset_40MHz** 
     
     .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4912656.svg
        :target: https://doi.org/10.5281/zenodo.4912656
        :alt: DOI
     
   * - ISM and phasor analysis
     - Jupyter Notebook example for implementing the pixel reassignment algorithm as well as the phasor plot analysis for FLIM data
     - `ISM&Phasors.pdf <dataProcessing/pynotebook/PDF/ISM_Decay_Reconstruction_BrightEyes-TTM_v1_opensource.pdf>`_
     - `ISM&Phasors.ipynb <dataProcessing/pynotebook/ISM_Decay_Reconstruction_BrightEyes-TTM_v1_opensource.ipynb>`_
     - Output 4D (x,y,t,ch) file from  `Image_reconstruction.ipynb <dataProcessing/pynotebook/Image_reconstruction.ipynb>`_ notebook after having processed **FLIM_512x512pixels_dwelltime250us_Dataset_40MHz** 
     
     .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4912656.svg
        :target: https://doi.org/10.5281/zenodo.4912656
        :alt: DOI
     

