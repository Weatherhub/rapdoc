安装HRRR WRF
============

.. code-block:: bash

    $ cd ~/rap/nwprod/hrrr.v1.0.6/sorc/hrrr_wrf.fd/WRFV3.4.2
    $ export WRF_DFI_RADAR=1
    $ ./clean –aa
    $ ./clean –a
    $ ./configure 
    # Select 15
    $ ./compile em_real
    $ cp main/wrf.exe ../../../exec/hrrr_wrfarw
    $ cp main/real.exe ../../../exec/hrrr_real

