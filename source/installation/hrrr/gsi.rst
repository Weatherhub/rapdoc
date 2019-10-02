安装HRRR GSI和GSI-HM
====================

cd ~/rap/nwprod/hrrr.v1.0.6/sorc/hrrr_gsi.fd/src
make -f Makefile clean
make –f Makefile
cp hrrr_gsi ../../../exec/hrrr_gsi
make -f Makefile lib
cd ../lib/GSD/gsdcloud
make -f Makefile clean
make -f Makefile
cd ../../../../hrrr_gsi_hm.fd/
make -f Makefile clean
make -f Makefile
cp hrrr_gsi_hm ../../exec/hrrr_gsi_hm
