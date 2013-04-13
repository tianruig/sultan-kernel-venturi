ccflags-y := -O3 -fgcse-lm -fgcse-sm -fsched-spec-load -fforce-addr -fsingle-precision-constant -mtune=cortex-a8 -marm -march=armv7-a -mfpu=neon -ftree-vectorize -mvectorize-with-neon-double

obj-$(CONFIG_VIDEO_FIMC)	+= fimc_dev.o fimc_v4l2.o fimc_capture.o fimc_output.o fimc_overlay.o fimc_regs.o
obj-$(CONFIG_VIDEO_FIMC_MIPI)	+= csis.o

ifeq ($(CONFIG_CPU_S5PV210),y)
EXTRA_CFLAGS += -DCONFIG_MIPI_CSI_ADV_FEATURE
endif

EXTRA_CFLAGS += -Idrivers/media/video

ifeq ($(CONFIG_VIDEO_FIMC_DEBUG),y)
EXTRA_CFLAGS += -DDEBUG
endif
