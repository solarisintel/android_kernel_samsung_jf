for SC04E

$ export ARCH=arm
$ export CROSS_COMPILE=~/arm-eabi-4.8/bin/arm-eabi-
$ make VARIANT_DEFCONFIG=jf_dcm_defconfig lineageos_jf_defconfig SELINUX_DEFCONFIG=selinux_defconfig
$ make -j4

modified files

drivers/barcode_emul/barcode_emul_ice4.c
arch/arm/configs/jf_dcm_defconfig
arch/arm/configs/Makefile

