# -*- makefile -*-
#
# Copyright 2010-2014 Joachim Wiedorn
#
# Licensed under the terms of the GPL-2 or any later version.
# On Debian systems, the complete text of the GNU General Public License
# version 2 can be found in the file `/usr/share/common-licenses/GPL-2'.

# Make a test floppy
# this floppy will boot a machine and display the output of some diagnostic
# programs to give you information on configuring LILO


floppy: disk.com bootsect.b
	@echo Copy image onto boot floppy
	cat bootsect.b disk.com | dd of=/dev/fd0 bs=512
	
