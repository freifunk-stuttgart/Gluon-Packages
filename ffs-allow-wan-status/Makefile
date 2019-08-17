include $(TOPDIR)/rules.mk

PKG_NAME:=ffs-allow-wan-status
PKG_VERSION:=1

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(TOPDIR)/../package/gluon.mk

PKG_CONFIG_DEPENDS += $(GLUON_I18N_CONFIG)


define Package/ffs-allow-wan-status
  SECTION:=gluon
  CATEGORY:=Gluon
  TITLE:=Allow status page to be accessed over WAN
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ffs-allow-wan-status/install
	$(INSTALL_DIR) $(1)/lib/gluon/upgrade
	$(INSTALL_BIN) ./files/lib/gluon/upgrade/141-allow-wan-status $(1)/lib/gluon/upgrade/141-allow-wan-status
endef

$(eval $(call BuildPackage,ffs-allow-wan-status))
