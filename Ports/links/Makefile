include ../../Library/GNU.mk

Title=		Links
Name=		links
Version=	2.8
Site=		http://links.twibright.com/
Source=		http://links.twibright.com/download/$(Name)-$(Version).tar.bz2
License=	GPL

define test_hook
$(BinDir)/links -version | grep $(Version)
endef
