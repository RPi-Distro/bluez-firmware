#
#  $Id: Makefile.am,v 1.2 2004/07/26 22:17:36 holtmann Exp $
#

firmwaredir = /lib/firmware

firmware = \
	broadcom/BCM-LEGAL.txt \
	broadcom/BCM2033-MD.hex \
	broadcom/BCM2033-FW.bin

EXTRA_DIST = $(firmware)

MAINTAINERCLEANFILES = Makefile.in \
	aclocal.m4 configure config.h.in \
	missing install-sh mkinstalldirs

install-data-local: $(firmware)
	$(mkinstalldirs) $(DESTDIR)$(firmwaredir)
	list='$?'; \
	for i in $$list; do \
		$(INSTALL_DATA) $(srcdir)/$$i $(DESTDIR)$(firmwaredir); \
	done

uninstall-local: $(firmware)
	list='$(notdir $?)'; \
	for i in $$list; do \
		rm -f $(DESTDIR)$(firmwaredir)/$$i; \
	done
