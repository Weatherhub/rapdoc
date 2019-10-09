时间标识的建立
=============

整个RAP-HRRR系统的运行是依靠 :code:`/sya/g2/gongying/LongRun/com/date` 下的时间标识文件来告诉系统运行哪个时刻.

.. code-block:: bash

  $ mkdir –p /sya/g2/gongying/LongRun/com/date

在定时作业中加入如下的脚本，每个整点更新时间标识文件:

.. code-block:: bash

  $ crontab –e:
  0 * * * * /sya/u/gongying/LongRun/course/lr_touchtime.py

