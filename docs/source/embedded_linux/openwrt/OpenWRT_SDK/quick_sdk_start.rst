Quick OpenWRT SDK start
=======================

More detailed tutorial is `here <https://openwrt.org/docs/guide-developer/helloworld/chapter1>`_ 

Download sdk
~~~~~~~~~~~~
::

    git clone https://git.openwrt.org/openwrt/openwrt.git source
    git checkout v21.02.3 # checkout to last release

Update and install feeds
~~~~~~~~~~~~~~~~~~~~~~~~
::

    ./scripts/feeds update -a
    ./scripts/feeds install -a

Run graphical configuration menu
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
::

    make menuconfig

Run make to build your firmware
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
::

    make

Adjust the Path variable
~~~~~~~~~~~~~~~~~~~~~~~~

Suppose that you sdk folder is located here ``/home/user/openwrt-sdk/openwrt-sdk-21.02.3``

Just add following path to PATH::

    export PATH=/home/comarch_user/openwrt-sdk/openwrt-sdk-21.02.3/staging_dir/host/bin:$PATH
    
