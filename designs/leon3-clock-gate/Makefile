GRLIB=../..
TOP=leon3mp
BOARD=gr-pci-xc2v
#BOARD=gr-cpci-xc2v
include $(GRLIB)/boards/$(BOARD)/Makefile.inc
DEVICE=$(PART)-$(PACKAGE)$(SPEED)
UCF=$(GRLIB)/boards/$(BOARD)/$(TOP).ucf
QSF=$(GRLIB)/boards/$(BOARD)/$(TOP).qsf
EFFORT=std
XSTOPT=""
VHDLSYNFILES=config.vhd ahbrom.vhd clkgate.vhd leon3mp.vhd
VHDLSIMFILES=testbench.vhd
SIMTOP=testbench
SDCFILE=$(GRLIB)/boards/$(BOARD)/default.sdc
BITGEN=$(GRLIB)/boards/$(BOARD)/default.ut
CLEAN=soft-clean

TECHLIBS = unisim simprim
LIBSKIP = tmtc gsi fmf dare gleichmann hynix openchip cypress \
	ihp core1553bbc core1553brt core1553brm corePCIF gr1553 \
	spansion 
DIRSKIP = b1553 usb ddr crypto ata satcan slink ascs pwm haps coremp7 gr1553b iommu \
	eon3ft leon4 leon4b64 l2cache pcif spi ac97 hcan

include $(GRLIB)/bin/Makefile
include $(GRLIB)/software/leon3/Makefile


##################  project specific targets ##########################

