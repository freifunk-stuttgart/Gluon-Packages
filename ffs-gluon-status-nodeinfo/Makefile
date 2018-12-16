include $(TOPDIR)/rules.mk

PKG_NAME:=ffs-gluon-status-nodeinfo
PKG_VERSION:=1

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(TOPDIR)/../package/gluon.mk

PKG_CONFIG_DEPENDS += $(GLUON_I18N_CONFIG)


define Package/ffs-gluon-status-nodeinfo
  SECTION:=gluon
  CATEGORY:=Gluon
  TITLE:=Expose nodeinfo over HTTP as JSON
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ffs-gluon-status-nodeinfo/install
	$(INSTALL_DIR) $(1)/lib/gluon/status-page/www/cgi-bin
	$(INSTALL_BIN) ./files/lib/gluon/status-page/www/cgi-bin/nodeinfo $(1)/lib/gluon/status-page/www/cgi-bin/nodeinfo
endef

$(eval $(call BuildPackage,ffs-gluon-status-nodeinfo))
