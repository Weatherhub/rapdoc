安装wrf_post
============

        cd ~/rap/nwprod/rap.v2.0.11/sorc/rap_wrfpost.fd
        edit makefile for correct paths
		make clean
        cd xml
        make clean
        make
        cd ..
        make
        cp rap_wrfpost ../../exec/rap_wrfpost
