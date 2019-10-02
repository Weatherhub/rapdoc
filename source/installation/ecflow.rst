ecflow的安装
============

从 ecFlow_ 的官网下载 ``boost_1_53_0.tar.gz`` 和 ``ecFlow-4.0.9-Source.tar.gz``

.. _ecFlow: https://confluence.ecmwf.int/display/ECFLOW

.. code-block:: bash

  $ cd ecflow_build/
  $ tar xvf ~/boost_1_53_0.tar.gz 
  $	tar xvf ~/ecFlow-4.0.9-Source.tar.gz 
  $	cd boost_1_53_0/
  $	export BOOST_ROOT=`pwd`
  $	cd ../ecFlow-4.0.9-Source/
  $	export WK=`pwd`
  $	cd $BOOST_ROOT 
  $	./bootstrap.sh 
  $	/tmp/ecflow_build/ecFlow-4.0.9-Source/build_scripts/boost_1_53_fix.sh 
  $	/tmp/ecflow_build/ecFlow-4.0.9-Source/build_scripts/boost_build.sh
  $	cd $WK
  $	mkdir build; cd build
  $	cmake .. -DCMAKE_INSTALL_PREFIX=/g2/home/PANN/ecflow409
  $	make –j4
  $	make check
  $	make install

在 ``~/.bashrc`` 中加入：

.. code-block:: bash

  $	export PATH=/g2/home/PANN/ecflow409/bin:$PATH
  $	export PYTHONPATH=/g2/home/PANN/ecflow409/lib/python2.7/site-packages/ecflow:$PYTHONPATH
