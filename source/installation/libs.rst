安装依赖库
==========

.. code-block:: bash

	compile libs
	Compile bacio
        cd ~/rap/nwprod/lib/sorc/bacio_v2.0.1/src
        ./makebacio_zeus.sh
        cp ../lib/libbacio_* ../../../
	Compile bufr
        cd ~/rap/nwprod/lib/sorc/bufr_v10.2.5
        ./makebufrlib.sh
	Compile g2tmpl
        cd ~/rap/nwprod/lib/sorc/g2tmpl_v1.2.2
        make
        Compile gfsio
	cd ~/rap/nwprod/lib/sorc/gfsio_v1.1.0
        rm ../../libgfsio_4.a
        ./make_wcoss.sh
	Compile ip
        cd ~/rap/nwprod/lib/sorc/ip/src
rm ../lib/libip_*
        ./makelibip.sh
        cp ../lib/libip_* ../../../
	Compile nemsio
        cd ~/rap/nwprod/lib/sorc/nemsio_v2.2.1
        make
        cp libnemsio.a ../../.
        cp incmod/nemsio_* ../../incmod/nemsio/
	Compile sfcio
        cd ~/rap/nwprod/lib/sorc/sfcio
        rm ../../libsfcio_big_4.a
        make.sh
	Compile sigio
        cd ~/rap/nwprod/lib/sorc/sigio_v2.0.1
        rm -fr sigio_v2.0.1
        make_sigio_lib.sh ifort.setup
        cp sigio_v2.0.1/libsigio_v2.0.1.a ../../libsigio.a
        cp sigio_v2.0.1/incmod/sigio_v2.0.1/sigio_* ../../incmod/sigio_4/.
	Compile sp
        cd ~/rap/nwprod/lib/sorc/sp_v2.0.2/sorc
        makelibsp.sh_Linux
        mv ../../libsp_v2.0.2_* ../../../.
	Compile transutil	
        cd ~/rap/nwprod/lib/sorc/transutil
        rm ../../libtransutil_*
        ./makelibtransutil.sh
	Compile w3emc
        cd ~/rap/nwprod/lib/sorc/w3emc_v2.0.5
        rm ../../libw3emc_*
        makelibw3.sh
	Compile w3nco
        cd ~/rap/nwprod/lib/sorc/w3nco_v2.0.6
        rm ../../libw3nco_*
        ./makelibw3_nco.sh
	Compile g2
cd ~/ rap/nwprod/lib/sorc/g2_v2.5.0
edit makefile_4 and makefile_d for correct paths
make –f makefile_4
make –f makefile_d
	Compile xmlparser
        cd ~/rap/nwprod/lib/sorc/xmlparse_v2.0.0
        make clean
        make FORCE
        make
        cp libsrc/libxmlparse.a ../../libxmlparse.a
        cp libsrc/*.mod ../../incmod/xmlparse/.
	Compile crtm
        cd ~/rap/nwprod/lib/sorc/crtm_2.1.3
        make clean
        . configure/ifort.setup
        make
        cp libsrc/libCRTM.a ../../libCRTM_2.1.3.a 
        mv libsrc/*.mod ../../incmod/crtm_2.1.3/

	Compile crtm 2.0.6
        cd ~/rap/nwprod/lib/sorc/crtm_2.0.6
        make clean
        . configure/ifort.setup
        make
        cp libsrc/libCRTM.a ../../libCRTM_2.0.6.a 
        mv libsrc/*.mod ../../incmod/crtm_2.0.6/

