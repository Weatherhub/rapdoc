ecFlow系统设置
==============

.. code-block:: bash

  $ cd ~/rap/course
  $ ecflow_start.sh -d `pwd` -v -p 3141

执行:

.. code-block:: bash

  $ ecflow_client –ping

应该有如下回应:

.. code-block:: bash

  $ ping server(localhost:3141) succeeded in 00:00:00.003079  ~3 milliseconds

RAP作业集的生成
==============

以下是如何产生RAP的作业集供ecFlow调用：

.. code-block:: bash

  $ cd ~/rap/course
  $ rm -fr operation_suite_v4
  $ ./operation.v4.py
 
 其产生的`rap_fcyc_v4.def`为整个作业集的`ecFlow`描述

