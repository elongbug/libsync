module_LTLIBRARIES = libsync.la
moduledir = $(libdir)

AM_CFLAGS = $(GCC_CFLAGS)

libsync_includedir = $(includedir)/sync
libsync_include_HEADERS = $(top_srcdir)/include/sync/sync.h

libsync_la_CFLAGS = $(AM_CFLAGS)            \
					-I$(top_srcdir)/include

libsync_la_LDFLAGS = -module -avoid-version
libsync_la_LIBADD =

libsync_la_SOURCES = $(top_srcdir)/include/linux/sync.h    \
					 $(top_srcdir)/include/linux/sw_sync.h \
					 $(top_srcdir)/include/sw_sync.h	   \
					 $(top_srcdir)/include/sync/sync.h     \
					 strlcpy.c \
					 sync.c
