GFS资料的准备
=============

实时的0.5度的GFS资料由气象台负责下载，每天4个时次：00Z, 06Z, 12Z, 18Z；资料位置在：/g2/home/fjwrf/testbed/data/input/GFS0p5
间隔三小时，一直到96小时。

为了可以在RAP系统中使用，必须做以下操作：
	cd ~/rap/com
	mkdir gfs
	cd gfs
	ln -fs /g2/home/fjwrf/testbed/data/input/GFS0p5 prod

