include $(TOPDIR)/rules.mk

PKG_NAME:=casaos-debugger
PKG_VERSION:=0.0.5
PKG_RELEASE:=1

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://github.com/CorrectRoadH/CasaOS-Debugger/releases/download/v$(PKG_VERSION)
PKG_HASH:=7f77bb1276a71d971fb6f62e05f64d96de2546ef969f72d5ad5dfc5925887459

include $(INCLUDE_DIR)/package.mk

define Package/casaos-debugger
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=casaos-debugger
  URL:=GitHub - CorrectRoadH/CasaOS-Debugger
endef

define Package/casaos-debugger/description
  CasaOS Debugger
endef

define Build/Compile
endef

define Package/casaos-debugger/install
	$(INSTALL_DIR) $(1)/var/lib/extensions
	$(CP) $(PKG_BUILD_DIR)/casaos-debugger.raw $(1)/var/lib/extensions
endef

$(eval $(call BuildPackage,casaos-debugger))