ecFlow系统设置
========================

ecFlow的启动
--------------------

.. code-block:: bash

  $ cd /sya/g2/gongying/LongRun/course
  $ ecflow_start.sh -d `pwd` -v -p 2506
  Wed Oct  9 07:35:04 GMT 2019

  User "4020107" attempting to start ecf server on "sya05n01" using ECF_PORT "2506" and with:
  ECF_HOME     : "/sya/g2/gongying/LongRun/course"
  ECF_LOG      : "sya05n01.2506.ecf.log"
  ECF_CHECK    : "sya05n01.2506.check"
  ECF_CHECKOLD : "sya05n01.2506.check.b"
  ECF_OUT      : "sya05n01.2506.ecf.out"

  client version is Ecflow version(4.0.5) boost(1.53.0) compiler(aix 1210) protocol(TEXT_ARCHIVE) Compiled on Feb 28 2015 08:19:43
  Checking if the server is already running on sya05n01 and port 2506
  [07:35:05 9.10.2019] Request( --ping :gongying ), Failed to connect to sya05n01:2506. After 2 attempts. Is the server running ?


  Backing up check point and log files

  OK starting ecFlow server...

  Placing server into RESTART mode...

  To view server on ecflowview - goto Edit/Preferences/Servers and enter
  Name        : <unique ecFlow server name>
  Host        : sya05n01
  Port Number : 2506

执行:

.. code-block:: bash

  $ ecflow_client --ping
应该有如下回应:

.. code-block:: bash

  ping server(sya05n01:2506) succeeded in 00:00:00.007362  ~7 milliseconds

RAP作业集的生成
---------------------

以下是如何产生RAP的作业集供ecFlow调用：

.. code-block:: bash

  $ cd /sya/g2/gongying/LongRun/course
  $ rm -fr sy_nwp_rap_v201908.def
  $ ./sy_nwp_rap_v201908.py
 
其产生的 :code:`sy_nwp_rap_v201908.def` 为整个作业集的ecFlows描述

重新更换已有的作业集
----------------------------

.. code-block:: bash

  $ ecflow_client --suites
  sy_nwp_rap
  
  $ ecflow_client --replace=/sy_nwp_rap sy_nwp_rap_v201908.def false force
