	Compile HRRR smartinit
cd ~/rap/nwprod/hrrr.v1.0.6/sorc/hrrr_smartinit.fd
make clean
make
cp hrrr_smartinit_conus ../../exec/hrrr_smartinit_conus

	Compile HRRR sndp
cd ~/rap/nwprod/hrrr.v1.0.6/sorc/hrrr_sndp.fd
make clean
make
cp hrrr_sndp ../../exec/hrrr_sndp

	Compile HRRR wrfbufr
cd ~/rap/nwprod/hrrr.v1.0.6/sorc/hrrr_wrfbufr.fd
make clean
make
cp hrrr_wrfbufr ../../exec/hrrr_wrfbufr

	Compile HRRR process_cloud
cd ~/rap/nwprod/hrrr.v1.0.6/sorc/hrrr_process_cloud.fd
make clean
make
cp hrrr_process_cloud ../../exec/hrrr_process_cloud

	Compile HRRR process_mosaic
cd ~/rap/nwprod/hrrr.v1.0.6/sorc/hrrr_process_mosaic.fd
make clean
make
cp hrrr_process_mosaic ../../exec/hrrr_process_mosaic

	Compile HRRR ref2tten
cd ~/rap/nwprod/hrrr.v1.0.6/sorc/hrrr_ref2tten.fd
make clean
make
cp hrrr_ref2tten ../../exec/hrrr_ref2tten
