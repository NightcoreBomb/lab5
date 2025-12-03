ifneq ($(KERNELRELEASE),)
# kbuild part of makefile

obj-m := hello1.o hello2.o
ccflags-y += -I$(src)/inc

else
# normal makefile

KDIR ?= /home/nighcore/repos/linux-stable

default:
	$(MAKE) -C $(KDIR) M=$(PWD) modules

clean:
	$(MAKE) -C $(KDIR) M=$(PWD) clean

endif

