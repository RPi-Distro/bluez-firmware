
firmwaredir = $(libdir)/firmware
brcmdir = $(firmwaredir)/brcm

firmware_DATA = \
	broadcom/BCM2033-MD.hex \
	broadcom/BCM2033-FW.bin \
	st/STLC2500_R4_00_03.ptc \
	st/STLC2500_R4_00_06.ssf \
	st/STLC2500_R4_02_02_WLAN.ssf \
	st/STLC2500_R4_02_04.ptc

brcm_DATA = \
	broadcom/BCM43430A1.hcd \
	broadcom/BCM4345C0.hcd \
	broadcom/BCM4345C5.hcd

EXTRA_DIST = $(firmware_DATA) \
	$(brcm_DATA) \
	broadcom/BCM2033-2.13-FW.bin \
	broadcom/BCM2033-2.14-FW.bin \
	broadcom/BCM2033-2.15-FW.bin \
	broadcom/BCM2033-2.16-FW.bin \
	broadcom/bcm_changeba \
	broadcom/bcm_changeid \
	broadcom/bcm_hex2bin

MAINTAINERCLEANFILES = Makefile.in \
	aclocal.m4 configure config.h.in \
	depcomp missing install-sh mkinstalldirs
