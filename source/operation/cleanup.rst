磁盘空间的清理
=================

因为RAP和HRRR系统在运行期间会产生大量的临时数据和产品，为了防止磁盘空间不足，可以在定时作业中加入以下定时作业，下面例子为每小时00分，删除2-3天前的所有数据文件。所以，请用户自行做好数据备份的工作

.. code-block:: bash

    $ cat /g2/home/PANN/rap/crl_scripts/clean.ksh
    #!/bin/ksh -x
    #cd $HOME/rap/com/hrrr ; /bin/find . -type d -ctime +2 -exec /bin/rm -fr {} \;
    cd $HOME/rap/com/rap ;  /bin/find . -type d -ctime +3 -exec /bin/rm -fr {} \;
    #cd $HOME/rap/com/gfs/prod ;  /bin/find . -type d -ctime +3 -exec /bin/rm -fr {} \;
    cd $HOME/rap/com/output ; /bin/find . -type f -mtime +2 -exec /bin/rm -fr {} \;
    cd $HOME/rap/com/logs ; /bin/find . -type f -mtime +2 -exec /bin/rm -fr {} \;
    cd $HOME/rap/nwges ; /bin/find . -type f -mtime +2 -exec /bin/rm -f {} \;
    cd $HOME/rap/tmpnwprd1 ; /bin/find . -type f -mtime +2 -exec /bin/rm -f {} \;

在定时作业中加入，使用 ``crontab –e``:

.. code-block:: bash

    00 * * * * /g2/home/PANN/rap/scripts/clean.ksh
