#
# Copyright (C) 2011-2015 Entware
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

all: .done

.done:
	patch -d $(TOP) -p3 -i $(CURDIR)/fix-path.patch
	mkdir -p ../../../openwrt_trunk/feeds/oldpackages/utils/cksfv/patches
	cp -f ./010-debian-612741.patch ../../../openwrt_trunk/feeds/oldpackages/utils/cksfv/
	@touch $@

clean:
	@rm -f .done

.PHONY: clean
