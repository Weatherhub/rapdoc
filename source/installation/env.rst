环境变量设置
-----------

在 ``$HOME/.bashrc`` 中加入以下设置：

.. code-block:: bash


  #For MPI compiler
  $ export MPI_PATH=/public/software/mpi/mvapich2/2.1/intel
  $ export PATH=$MPI_PATH/bin:$PATH
  $ export LD_LIBRARY_PATH=$MPI_PATH/lib:$LD_LIBRARY_PATH
  $ export MANPATH=$MPI_PATH/share/man:$MANPATH
  $ export MV2_SMP_USE_CMA=0

  #For NCL
  $ export NCARG_ROOT=/public/software/mathlib/ncl_ncarg/6.2.0/gnu
  $ export PATH=$NCARG_ROOT/bin:$PATH
