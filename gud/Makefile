MODULE_MAME = gud_drm
 
SRCS = gud_drm_pipe.c gud_drm_connector.c gud_drm_drv.c
 
OBJS =  $(SRCS:.c=.o)
 
obj-m += $(MODULE_MAME).o
$(MODULE_MAME)-y = $(OBJS)
 
all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
