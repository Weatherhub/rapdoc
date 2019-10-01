作业系统的启动
=============

* 建立日志文件输出目录:

.. code-block:: bash

  $ mkdir –p ~/rap/com/output/prod/today
  $ mkdir –p ~/ rap/com/logs/jlogfiles

* 载入作业集:

.. code-block:: bash

  $ ecflow_client --load rap_fcyc_v4.def

* 启动作业集:

.. code-block:: bash

  $ ecflow_client --begin operation_suite_v4
