ev3dev-crosstool-ng
===================

Crosstool-NG configurations for ev3dev cross compilers.


Maintainer Notes
----------------

How to do a release:

    ct-ng defconfig DEFCONFIG=config_${TARGET_ARCH}
    ct-ng build.6 RELEASE_NAME=gcc-ev3dev-${TARGET_GCC_VERSION}-${PACKAGE_VERSION}-${HOST_ARCH}
    cd dist
    tar -czf ${RELEASE_NAME}_${TARGET_TUPLE}.tar.gz ${RELEASE_NAME}_${TARGET_TUPLE}
