for SC04E  

$ export ARCH=arm  
$ export CROSS_COMPILE=~/arm-eabi-4.8/bin/arm-eabi-  
$ make lineageos_jfdcm_defconfig  
$ make -j4  

modified files  

arch/arm/mach-msm/board-jf_dcm.c  
drivers/barcode_emul/barcode_emul_ice4.c  
arch/arm/configs/lineageos_jfdcm_defconfig  
init/main.c  


RR Oreo kernel for SC04E   

git clone -b aosp-8.1-vend https://github.com/JDCTeam/platform_kernel_samsung_jf.git  

Difference between i9505 (EUR) and SC04E (DCM)  

・Camera  
　board-jf_euc.c, board_jf_dcm.c

・Power LED  
  jf_eur-gpio.h   
 
・Camera's voltages  
  board-8064-camera.c  
  board-8064-regulator.c

・Thermistor  
  board-fusion3-battery.c  
  fusion3-thermistor.c  

・Earphone, Mic  
  board-jf_euc.c, board_jf_dcm.c  




