m4_define([sync_major], 0)
m4_define([sync_minor], 0)
m4_define([sync_micro], 0)

m4_define([sync_version], [sync_major.sync_minor.sync_micro])

AC_PREREQ([2.64])
AC_INIT([sync], [sync_version], [kk.moon@samsung.com])

AC_SUBST([SYNC_VERSION_MAJOR], [sync_major_version])
AC_SUBST([SYNC_VERSION_MINOR], [sync_minor_version])
AC_SUBST([SYNC_VERSION_MICRO], [sync_micro_version])
AC_SUBST([SYNC_VERSION], [sync_version])

AC_CONFIG_HEADERS([config.h])
AM_INIT_AUTOMAKE([1.11 foreign no-dist-gzip dist-xz])
AM_SILENT_RULES([yes])

AC_PROG_CC
PKG_PROG_PKG_CONFIG

LT_PREREQ([2.2])
LT_INIT([static shared])
#LT_INIT([disable-static])

if test "x$GCC" = "xyes"; then
GCC_CFLAGS="-Wall -Wextra -Wno-unused-parameter \
			-Wno-missing-field-initializers -g \
			-Wstrict-prototypes -Wsign-compare"
fi
AC_SUBST(GCC_CFLAGS)

# Output files
AC_CONFIG_FILES([
Makefile
src/Makefile
test/Makefile
])

AC_OUTPUT
