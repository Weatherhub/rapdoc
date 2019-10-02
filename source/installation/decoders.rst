安装decoders
================

.. code-block:: bash

  $ cd ~/rap/nwprod/decoders/decod_shared
  $ cd include
  $ ln -fs ../../../gempak/NAWIPS/Gemenviron.profile .gempak
  $ cd ../lib
  $ cd crex
  # edit makecrex.sh for the correct path
  $ rm libcrex.a
  $ ./makecrex.sh
  $ cd ..
  $ ln -sf crex/libcrex.a libcrex.a
  $ cd madis/src
  $ make clean
  $ make
  $ cd ../..
  $ ln -sf madis/lib/madislib.a libmadis.a
  $ cd decod_ut
  # edit makedecod_ut.sh to make the path correct
  $ rm libdecod_ut.a
  $ ./makedecod_ut.sh
  $ cd ..
  $ ln -sf decod_ut/libdecod_ut.a libdecod_ut.a
  $ ln -fs ~/rap/nwprod/gempak/NAWIPS/os/linux64/lib/rsl.a librsl.a

  $ cd ~/rap/nwprod/gempak/NAWIPS/os/linux64/lib
  $ ln -fs bridge.a libbridge.a
  $ ln -fs gemlib.a libgemlib.a
  $ ln -fs cgemlib.a libcgemlib.a
  $ ln -fs gplt.a libgplt.a
  $ ln -fs device.a libdevice.a
  $ ln -fs gn.a libgn.a

  $ cd ~/rap/nwprod/decoders/decod_shared/include
  $ edit make_defns.cmn.mk for the correct path
  $ ./make_all_decoders.sh
  $ ecod_dccrad is not compiled due to the rsl.a

  $ cd ~/rap/nwprod/sorc/bufr_tranjb.fd
  $ make clean
  $ make
  $ cp bufr_tranjb ../../exec/.
