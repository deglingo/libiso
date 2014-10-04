AC_INIT([libiso], [0.0.0])
AM_INIT_AUTOMAKE

: ${CFLAGS:=-g -O0 -Wall}

AC_SUBST([pkgconfigdir], ['${libdir}/pkgconfig'])

AC_PROG_CC
AM_PROG_CC_C_O
LT_INIT

PKG_CHECK_MODULES([LOS], [los])

# test suite
AM_PIFTEST_SUITE([test])

AC_CONFIG_FILES([ \
  Makefile \
  libiso/Makefile \
  test/Makefile \
])
AC_CONFIG_FILES([libiso.pc])
AC_OUTPUT
