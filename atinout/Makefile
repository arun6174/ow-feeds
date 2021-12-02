include $(TOPDIR)/rules.mk

PKG_NAME:=atinout
PKG_VERSION:=0.9.1
PKG_RELEASE:=1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=git://git.code.sf.net/p/atinout/code
PKG_SOURCE_VERSION:=4976a6cb5237373b7e23cd02d7cd5517f306e3f6
PKG_MIRROR_HASH:=efa4e5b029a976dd45180a96494218f2a22417d8981e59c670128a4dae38eb4f

PKG_FIXUP:=autoreconf

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
	SECTION:=net
	CATEGORY:=Network
	TITLE:=atinout
	DEPENDS:=
endef

define Package/$(PKG_NAME)/description
	Executes AT commands in sequence and captures the response from the modem.
endef

define Package/$(PKG_NAME)/install
	$(INSTALL_DIR) $(1)/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/atinout $(1)/bin/
endef


$(eval $(call BuildPackage,$(PKG_NAME)))
