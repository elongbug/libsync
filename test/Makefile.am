noinst_PROGRAMS  = sync_test

sync_test_CFLAGS = -I$(top_srcdir)/include \
				   -pthread

sync_test_SOURCES = $(top_srcdir)/include/linux/sync.h    \
					$(top_srcdir)/include/linux/sw_sync.h \
					$(top_srcdir)/include/sw_sync.h       \
					$(top_srcdir)/include/sync/sync.h     \
					$(top_srcdir)/src/strlcpy.c           \
					$(top_srcdir)/src/sync.c              \
					sync_test.c
