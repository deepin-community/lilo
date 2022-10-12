# -*- makefile -*-
#
# Copyright 2010-2014 Joachim Wiedorn
#
# Licensed under the terms of the GPL-2 or any later version.
# On Debian systems, the complete text of the GNU General Public License
# version 2 can be found in the file `/usr/share/common-licenses/GPL-2'.


BASE     := /etc
POSTINST := kernel/postinst.d
PREINST  := kernel/preinst.d
PRERM    := kernel/prerm.d

all:

install:
	@echo Install kernel hook scripts
	mkdir -p $(BASE)/$(POSTINST)
	mkdir -p $(BASE)/$(PREINST)
	mkdir -p $(BASE)/$(PRERM)
	install -m 0755 $(POSTINST)/chattr-lilo  $(BASE)/$(POSTINST)
	install -m 0755 $(PREINST)/chattr-lilo  $(BASE)/$(PREINST)
	install -m 0755 $(PRERM)/chattr-lilo  $(BASE)/$(PRERM)

uninstall:
	@echo Uninstall kernel hook scripts
	rm $(BASE)/$(POSTINST)/chattr-lilo
	rm $(BASE)/$(PREINST)/chattr-lilo
	rm $(BASE)/$(PRERM)/chattr-lilo

