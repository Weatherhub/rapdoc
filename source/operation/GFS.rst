GFS资料的准备
==================

实时的0.5度的GFS资料由气象台负责下载，每天4个时次：00Z, 06Z, 12Z, 18Z；
资料位置在： :code:`/sya/g3/wrf/data/gfs/2019`
间隔6小时，一直到240小时。

为了可以在RAP系统中使用，必须做以下操作:

.. code-block:: bash

    $ cd /sya/g2/gongying/LongRun/com
    $ mkdir -p gfs/prod
    $ cd gfs/prod
    $ ln -fs /sya/g3/wrf/data/gfs/2019 2019

