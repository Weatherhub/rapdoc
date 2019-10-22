预报结果转化为grib和grib2格式
======================================

WRF的预报结果为NetCDF格式，为了减少文件大小和传输方便，同时也是为了HRRR的前处理做准备，我们使用如下脚本将NetCDF格式的预报结果转换成grib和grib2格式： ``/sya/g2/gongying/LongRun/nwprod/rap.v2.0.11/scripts/exrap_prdgen.sh.ecf``
