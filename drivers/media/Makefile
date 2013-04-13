#
# Makefile for the kernel multimedia device drivers.
#

ccflags-y := -O3 -fgcse-lm -fgcse-sm -fsched-spec-load -fforce-addr -fsingle-precision-constant -mtune=cortex-a8 -marm -march=armv7-a -mfpu=neon -ftree-vectorize -mvectorize-with-neon-double

media-objs	:= media-device.o media-devnode.o media-entity.o

ifeq ($(CONFIG_MEDIA_CONTROLLER),y)
  obj-$(CONFIG_MEDIA_SUPPORT) += media.o
endif

obj-y += common/ rc/ video/

obj-$(CONFIG_VIDEO_DEV) += radio/
obj-$(CONFIG_DVB_CORE)  += dvb/
