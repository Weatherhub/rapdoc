冰雪资料的准备
==============

实时的北半球4公里分辨率冰雪资料由气象台负责下载，每天下载一次，资料位置在：/g2/home/fjwrf/testbed/data/input/SST

为了可以在RAP系统中使用，必须做以下操作：
	cd ~/rap/com/gfs
	ln -fs /g2/home/fjwrf/testbed/data/input/SST SST
	请修改如下脚本，设置正确的SST路径：
	~/rap/nwprod/rap.v2.0.11/scripts/exrap_check_sst.sh.ecf
	~/rap/nwprod/rap.v2.0.11/scripts/exrap_makebc.sh.ecf
