#
# Makefile
#

CIRCLEHOME = ../Circle

OBJS	= main.o kernel.o oscws28xx.o

INCLUDE	+= -I ./include
INCLUDE	+= -I ../lib-osc/include -I ../lib-ws28xx/include
INCLUDE	+= -I ../lib-lightset/include  -I ../lib-ledblink/include
INCLUDE	+= -I ../lib-network/include
INCLUDE	+= -I ../include 

LIBS = ../lib-osc/libosc.a ../lib-ws28xx/libws28xx.a ../lib-network/libnetwork.a ../lib-properties/libproperties.a ../lib-lightset/liblightset.a ../lib-ledblink/libledblink.a

LIBS +=	$(CIRCLEHOME)/addon/SDCard/libsdcard.a \
	$(CIRCLEHOME)/addon/fatfs/libfatfs.a \
	$(CIRCLEHOME)/lib/fs/libfs.a \
	$(CIRCLEHOME)/lib/usb/libusb.a \
	$(CIRCLEHOME)/lib/input/libinput.a \
	$(CIRCLEHOME)/lib/net/libnet.a \
	$(CIRCLEHOME)/lib/sched/libsched.a \
	$(CIRCLEHOME)/lib/libcircle.a

include $(CIRCLEHOME)/sample/Rules.mk
