include ../../Library/GNU.mk

Title=		Fish Shell
Name=		fish
Version=	2.5.0
Site=		http://fishshell.com
Source=		http://fishshell.com/files/$(Version)/$(Name)-$(Version).tar.gz
License=	GPLv2

ReadMeFile=	$(SourceDir)/README.md
LicenseFile=	$(SourceDir)/COPYING

define install_post_hook
mv $(DestDir)$(SysConfDir)/fish/config.fish \
	$(DestDir)$(SysConfDir)/fish/config.fish.default
endef

define test_hook
$(BinDir)/fish 2>&1  --version | grep $(Version)
endef
