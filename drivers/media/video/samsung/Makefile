ccflags-y := -O3 -fgcse-lm -fgcse-sm -fsched-spec-load -fforce-addr -fsingle-precision-constant -mtune=cortex-a8 -marm -march=armv7-a -mfpu=neon -ftree-vectorize -mvectorize-with-neon-double

obj-$(CONFIG_VIDEO_FIMC)	+= fimc/
obj-$(CONFIG_VIDEO_MFC50)	+= mfc50/
obj-$(CONFIG_VIDEO_JPEG_V2)	+= jpeg_v2/
#obj-$(CONFIG_VIDEO_ROTATOR)	+= rotator/
obj-$(CONFIG_VIDEO_TV20)        += tv20/
#obj-$(CONFIG_VIDEO_G2D)		+= g2d/
#obj-$(CONFIG_VIDEO_TSI)		+= tsi/

EXTRA_CFLAGS += -Idrivers/media/video

