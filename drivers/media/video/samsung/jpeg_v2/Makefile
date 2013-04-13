ccflags-y := -O3 -fgcse-lm -fgcse-sm -fsched-spec-load -fforce-addr -fsingle-precision-constant -mtune=cortex-a8 -marm -march=armv7-a -mfpu=neon -ftree-vectorize -mvectorize-with-neon-double

obj-$(CONFIG_VIDEO_JPEG_V2)	+= jpg_mem.o jpg_misc.o jpg_opr.o s3c-jpeg.o
EXTRA_CFLAGS += -Idrivers/media/video

