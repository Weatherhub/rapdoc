安装rap wrf
===========

        cd ~/rap/nwprod/rap.v2.0.11/sorc/rap_wrf.fd/WRFV3.4.1
        ./clean -a
        ./configure radardfi
        Select '15' and then select '1' to get configure.wrf
        ./compile em_real |& tee make.log
./compile em_real |& tee make.log
        cp main/rap_real ../../../exec/rap_real
        cp main/rap_wrfarw ../../../exec/rap_wrfarw
