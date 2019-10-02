安装rap-gsi
===========

        cd ~/rap/nwprod/rap.v2.0.11/sorc/rap_gsi.fd
        edit Makefile.conf for correct paths
make clean
        make
        cd gsdcloud
        make clean
        make
        cd ..
        make
        cp rap_gsi ../../exec/rap_gsi
