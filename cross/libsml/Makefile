PKG_NAME = libsml
PKG_VERS = master
PKG_EXT = zip
PKG_DIST_NAME = $(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = https://github.com/volkszaehler/libsml/archive/
PKG_DIR = $(PKG_NAME)-$(PKG_VERS)

DEPENDS = cross/libuuid

HOMEPAGE = https://github.com/volkszaehler/libsml
COMMENT  = libSML is a library which implements the Smart Message Language (SML) protocol specified by VDE's Forum Netztechnik/Netzbetrieb (FNN). It can be utilized to communicate to FNN specified Smart Meters or Smart Meter components (EDL/MUC).
LICENSE  = GPLv3

CONFIGURE_TARGET = nop
#INSTALL_TARGET = myInstall
GNU_CONFIGURE = 0

include ../../mk/spksrc.cross-cc.mk

.PHONY myInstall:

myInstall:

	mkdir -p $(STAGING_INSTALL_PREFIX)/usr/lib/pkgconfig

        #echo $(WORK_DIR)/$(PKG_DIR)/sml/lib/libsml.* $(STAGING_INSTALL_PREFIX)/usr/lib/

	echo  $(WORK_DIR)/$(PKG_DIR)/sml.pc $(STAGING_INSTALL_PREFIX)/usr/lib/pkgconfig/