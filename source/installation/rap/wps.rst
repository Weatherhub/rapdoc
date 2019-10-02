安装rap wps
============

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/rap_wrf.fd/WPSV3.4.1
		$ ./clean -a
        $ configure
        # select '19'

        # Please change the configure.wps  to:

        # WRF_DIR                 =       ../WRFV3.4.1
 
        # COMPRESSION_LIBS    = -L/home/zx/rap/nwprod/gempak/NAWIPS/os/linux64/lib -ljasper -lpng -lz
 
        # COMPRESSION_INC     = -I/home/zx/rap/nwprod/gempak/NAWIPS/os/linux64/include
 
        $ ./compile
        $ cp metgrid/src/metgrid.exe ../../../exec/rap_metgrid
        $ cp ungrib/src/ungrib.exe ../../../exec/rap_ungrib
