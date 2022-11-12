# BPI-M2-Berry
The Banana pi m2 berry can be very hard to boot.
To boot arch linux:
- Download arch linux for arm for Cubieboard 2 https://archlinuxarm.org/platforms/armv7/allwinner/cubieboard-2
- Follow the instructions to install arch linux
- There will be no display output so you need to ssh into the banana pi

If that doesn't work build u-boot from scratch.
You will need to have the gcc cross compiler installed (arm-linux-eabi).

```
	git clone https://github.com/u-boot/u-boot.git
	cd u-boot
	make Bananapi_M2_Ultra_defconfig
	make -j4 CROSS_COMPILE=arch-linux-eabi-
```



