# SPDX-License-Identifier: GPL-3.0-only
#
# Copyright (C) 2019-2022 Tianling Shen <cnsztl@immortalwrt.org>

include $(TOPDIR)/rules.mk

LUCI_TITLE:=LuCI support for UnblockNeteaseMusic (JavaScript)
LUCI_DEPENDS:=+dnsmasq-full +node \
	+PACKAGE_firewall:ipset \
	@(PACKAGE_libustream-mbedtls||PACKAGE_libustream-openssl||PACKAGE_libustream-wolfssl)
LUCI_PKGARCH:=all

PKG_NAME:=luci-app-unblockneteasemusic
PKG_VERSION:=3.1
PKG_RELEASE:=4

PKG_MAINTAINER:=Tianling Shen <cnsztl@immortalwrt.org>

define Package/luci-app-unblockneteasemusic/conffiles
/etc/config/unblockneteasemusic
endef

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature
