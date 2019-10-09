作业系统的启动
=============

* 建立日志文件输出目录:

.. code-block:: bash

  $ mkdir –p /sya/g2/gongying/LongRun/com/output/prod/today
  $ mkdir –p /sya/g2/gongying/LongRun/com/logs/jlogfiles

* 载入作业集:

.. code-block:: bash

  $ cd /sya/g2/gongying/LongRun/course
  $ ecflow_client --load sy_nwp_rap_v201908.def

* 打开ecflowview

.. code-block:: bash
  
  $ ecflowview&
  
.. figure:: ../images/ecflowview-load.JPG
   :scale: 60%
   :align: center
   :alt:  ecflowview截图
     
   ecflowview截图

* 启动作业集:

.. code-block:: bash

  $ cd /sya/g2/gongying/LongRun/course
  $ ecflow_client --begin sy_nwp_rap
  
ecflowview中的任务图标会变成蓝色

.. figure:: ../images/ecflowview-begin.JPG
   :scale: 60%
   :align: center
   :alt:  ecflowview suite开始截图
     
   ecflowview suite开始截图
