Building custom packages with OpenWrt SDK
=========================================

1. Go to ``./feeds/`` and create folder with Makefile
2. ~~~~FILL here example makefiles~~~
3. In ./package/feeds/{your_feeds_name_eg_company}/
4. ln -s to a folder with Makefile from point 1
5. In {sdk_main_path}:
6. make menuconfig
7. Check if <M> or {M} is set for you app
8. exit menuconfig
9. build package::

    make package/{package_name}/{clean,compile}