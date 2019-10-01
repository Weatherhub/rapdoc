时间标识的建立
=============

整个$RAP-HRRR系统的运行是依靠

.. code-block:: bash

  $ mkdir –p $HOME/rap/com/date

在定时作业中加入，使用:

.. code-block:: bash

  $ crontab –e:
    00 * * * * /g2/home/PANN/rap/scripts/touchtime.py

