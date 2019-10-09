磁盘空间的清理
=================

因为RAP和HRRR系统在运行期间会产生大量的临时数据和产品，为了防止磁盘空间不足，可以在定时作业中加入以下定时作业，下面例子为每小时00分，删除2-3天前的所有数据文件。所以，请用户自行做好数据备份的工作

.. code-block:: bash

    $ cat /sya/u/gongying/LongRun/course/clean.ksh
    #!/bin/ksh -x
    #cd ${HOME}/LongRun/com/hrrr ; /bin/find . -type d -ctime +2 -exec /bin/rm -fr {} \;
    #cd ${HOME}/LongRun/com/rap ;  /bin/find . -type d -ctime +2 -exec /bin/rm -fr {} \;
    #cd ${HOME}/LongRun/com/gfs/prod ;  /bin/find . -type d -ctime +2 -exec /bin/rm -fr {} \;
    cd ${HOME}/LongRun/com/output ; /bin/find . -type f -mtime +2 -exec /bin/rm -fr {} \;
    cd ${HOME}/LongRun/com/logs ; /bin/find . -type f -mtime +1 -exec /bin/rm -fr {} \;
    cd ${HOME}/LongRun/nwges ; /bin/find . -type f -mtime +1 -exec /bin/rm -f {} \;
    #cd ${HOME}/LongRun/tmpnwprd1 ; /bin/find . -type f -mtime +1 -exec /bin/rm -f {} \;
    nice find ${HOME}/LongRun/com/output/prod/today -type f -mtime +1 -exec  rm -fr {} \; 1> /dev/null 2>&1
    nice find ${HOME}/LongRun/com/rap/prod -type d -mtime +3 -exec rm -fr {} \; 1> /dev/null 2>&1
    nice find  ${HOME}/LongRun/tmpnwprd1 -type d -mtime +1 -exec rm -fr {} \; 1> /dev/null 2>&1
    nice find  $HOME/dmsg -type f -mtime +5 -exec rm -fr {} \; 1> /dev/null 2>&1


在定时作业中加入:

.. code-block:: bash

    $ crontab -l
    0 0,12 * * * /sya/u/gongying/LongRun/course/clean.ksh
