KERNELDIR := /lib/modules/$(shell uname -r)/build
# CFLAGS_genltest.o := -O0
obj-m += genltest.o

all:
	$(MAKE) -C $(KERNELDIR) V=0  M=`pwd` modules
clean:
	#$(MAKE) -C $(KERNELDIR)  M=`pwd` clean
	@rm -f *.ko *.o modules.order Module.symvers *.mod.? *~
	@rm -rf .tmp_versions .cache.mk *.ur-safe *.mod

