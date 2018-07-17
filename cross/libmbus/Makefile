PKG_NAME = libmbus
PKG_VERS = 0.8.0
PKG_EXT = tar.gz
PKG_DIST_NAME = $(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = https://github.com/rscada/libmbus/archive/
PKG_DIR = $(PKG_NAME)-$(PKG_VERS)

DEPENDS = 

HOMEPAGE = https://github.com/rscada/libmbus
COMMENT  = libmbus is an open source library for the M-bus (Meter-Bus) protocol.
LICENSE  = BSD 3-Clause License

GNU_CONFIGURE = 1
CONFIGURE_ARGS =
CONFIGURE_TARGET = build_sh
#COMPILE_TARGET = nop

include ../../mk/spksrc.cross-cc.mk

.PHONY build_sh:
build_sh:
	cd $(WORK_DIR)/$(PKG_DIR);chmod +x build.sh;./build.sh