安装HRRR WPS
============

cd ~/rap/nwprod/hrrr.v1.0.6/sorc/hrrr_wrf.fd/ WPSV3.4.1
export WRF_DFI_RADAR=1
./clean –aa
./clean –a
./configure 
Select 19, edit configure.wrf as:
WRF_DIR = ../WRFV3.4.2
COMPRESSION_LIBS    = -L/g2/home/PANN/rap/nwprod/gempak/NAWIPS/os/linux64/lib -ljasper -lpng -lz
COMPRESSION_INC     = -I/g2/home/PANN/rap/nwprod/gempak/NAWIPS/os/linux64/include
./compile
cp ungrib.exe ../../../exec/hrrr_ungrib
cp metgrid.exe ../../../exec/hrrr_metgrid
