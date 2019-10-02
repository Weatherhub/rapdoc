安装各种工具
===========

	Compile wgrib
cd ~/rap/nwprod/util/sorc/wgrib.cd
make clean
make
mv wgrib ../../exec/wgrib

	Compile wgrib2
cd ~/rap/nwprod/util/sorc/wgrib2.cd/grib2
make clean
make
cp wgrib2/wgrib2 ../../../exec/wgrib2

	Compile ndate
cd ~/rap/nwprod/util/sorc/ndate.fd
make 
cp ndate ../../exec/ndate

	Compile copygb2
cd ~/rap/nwprod/util/sorc/copygb2.fd
make clean
make
cp copygb2 ../../exec/copygb2

	Compile cnvgrib
cd ~/rap/nwprod/util/sorc/cnvgrib.fd 
cp cnvgrib ../../exec/.

	Compile cwordsh
cd ~/rap/nwprod/util/sorc/cwordsh.fd
make clean
make
cp cwordsh ../../exec/cwordsh

	Compile debufr
cd ~/rap/nwprod/util/sorc/debufr.fd
make clean
make
cp debufr ../../exec/debufr

	Compile grb2index
cd ~/rap/nwprod/util/sorc/grb2index.fd
make clean
make
cp grb2index ../../exec/grb2index

	Compile grbindex
cd ~/ rap/nwprod/util/sorc/grbindex.fd
make clean
make
cp grbindex ../../exec/grbindex

	Compile tocgrib2
cd ~/rap/nwprod/util/sorc/tocgrib2.fd
make clean
make
cp tocgrib2 ../../exec/tocgrib2

	Compile tocgrib
cd ~/rap/nwprod/util/sorc/tocgrib.fd
make clean
make
cp tocgrib ../../exec/tocgrib
