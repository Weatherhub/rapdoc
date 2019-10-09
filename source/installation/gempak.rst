安装gempak
=============

.. code-block:: bash

  $ cd /sya/g2/gongying/LongRun/nwprod/gempak/NAWIPS
  $ edit Gemenviron.profile for correct paths
  $ . Gemenviron.profile
  $ make distclean 
  $ edit gempak/source/gemlib/gg/ggrwsp.c , change gg_rwsp_ to gg_rwsp
  $ make all |& tee make.log
  $ make install; make clean
