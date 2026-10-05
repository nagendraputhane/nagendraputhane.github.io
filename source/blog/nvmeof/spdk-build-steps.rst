================
SPDK Build Steps
================

Steps to build SPDK from source.

.. code-block:: bash

   git clone https://github.com/spdk/spdk.git
   cd spdk
   git checkout v26.01
   git submodule update --init
   ./scripts/pkgdep.sh
   ./configure --with-rdma
   make -j"$(nproc)"
