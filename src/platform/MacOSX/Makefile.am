if MACOS
if CLIENT_INCLUDED
noinst_LTLIBRARIES = libMac.la
endif
endif

libMac_la_LDFLAGS = -static

if HAVE_SDL

libMac_la_SOURCES =			\
	MacDataPath.cxx

else

libMac_la_SOURCES =			\
	MacDataPath.cxx			\
	MacDisplay.cxx			\
	MacDisplay.h			\
	MacMedia.cxx			\
	MacMedia.h			\
	MacPlatformFactory.cxx		\
	MacPlatformFactory.h		\
	MacVisual.cxx			\
	MacVisual.h			\
	MacWindow.cxx			\
	MacWindow.h

endif

AM_CPPFLAGS = -I$(top_srcdir)/src/platform $(SDL_CFLAGS) $(CONF_CPPFLAGS)
AM_CFLAGS = $(CONF_CFLAGS)
AM_CXXFLAGS = $(CONF_CXXFLAGS)

MAINTAINERCLEANFILES = Makefile.in

EXTRA_DIST =				\
	mkplist.cxx
