obj-m += nailgun.o


KERNELDIR := ~/CS315-NailgunDefense/CS315-NailgunDefense/codes/modulespath/lib/modules/4.14.114-v7+/build

CROSS_COMPILE=/home/irakatz/CS315-NailgunDefense/CS315-NailgunDefense/codes/tools/arm-bcm2708/gcc-linaro-arm-linux-gnueabihf-raspbian-x64/bin/arm-linux-gnueabihf-


all:
	make ARCH=arm -C $(KERNELDIR) M=$(PWD) CROSS_COMPILE=~/CS315-NailgunDefense/CS315-NailgunDefense/codes/tools/arm-bcm2708/gcc-linaro-arm-linux-gnueabihf-raspbian-x64/bin/arm-linux-gnueabihf- modules

clean:
	make -C $(KERNELDIR) M=$(PWD) clean
