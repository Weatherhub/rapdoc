安装rap工具
===========

compile bufr_avgdata
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/obsproc_shared/bufr_avgdata.v1.0.1/sorc
        # edit setlibs.rc  for the correct paths
        $ ./clean.sh
        $ ./build.sh
        $ ./install.sh

compile bufr_cword
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/obsproc_shared/bufr_cword.v1.0.0/sorc
        # edit setlibs.rc  for the correct paths
        $ ./build.sh
        $ ./install.sh

compile bufr_remorest
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/obsproc_shared/bufr_remorest.v1.0.0/sorc
        # edit setlibs.rc  for the correct paths	
        $ ./clean.sh
        $ ./build.sh
        $ ./install.sh

compile nam_stnmlist
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/nam.v3.1.15/sorc/nam_stnmlist.fd
        # edit makefile for the correct paths
        $ make


compile rap_prdgen
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/rap_prdgen.fd
        # edit makefile for correct path
        $ make clean
        $ make
        $ cp rap_prdgen ../../exec/rap_prdgen


compile wrfbufr
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/rap_wrfbufr.fd
        # edit makefile for correct paths
        $ make clean
        $ make
        $ cp rap_wrfbufr ../../exec/rap_wrfbufr


compile rap_sndp
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/rap_sndp.fd
        # edit makefile for correct path
        $ make clean
        $ make
        $ cp rap_sndp ../../exec/rap_sndp


compile data_process
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/data_process
        # edit configure.process for correct paths

Compile rap_full_cycle_surface
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/data_process/updatebk/netcdf
        # edit makefile for correct path
        $ make clean
        $ make
        $ cp rap_full_cycle_surface ../../../../exec/rap_full_cycle_surface

Compile imssnow
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/data_process/imssnow/ascii
        # edit makefile for correct paths
        $ make clean
        $ make
        $ cp rap_process_imssnow ../../../../exec/rap_process_imssnow
        
Compile process_sst
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/data_process/ssthires/netcdf
        # edit makefile for correct paths
        $ make clean
        $ make
        $ cp rap_process_sst ../../../../exec/rap_process_sst
        
Compile update_height
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/data_process/updateHeight/netcdf
        # edit makefile for correct paths
        $ make clean
        $ make
        $ cp rap_update_height ../../../../exec/rap_update_height
        
Compile mosaic
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/data_process/mosaic/netcdf
        # edit makefile for correct paths
        $ make clean
        $ make
        $ cp rap_process_mosaic ../../../../exec/rap_process_mosaic
        
Compile process_cloud
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/data_process/nasalarc/netcdf
        # edit makefile for correct paths
        $ make clean
        $ make
        $ cp rap_process_cloud ../../../../exec/rap_process_cloud
        
Compile subfild
-----------------------

.. code-block:: bash

        $ cd ~/rap/nwprod/rap.v2.0.11/sorc/rap_subflds.fd
        # edit makefile_130 for correct path
        $ ./compile.sh
        $ cp rap_subflds_130 ../../exec/rap_subflds_130

