dnl Process this file with autoconf to produce a configure script.

AC_INIT(dasom-settings, 0.1, https://github.com/dasom-im/dasom-settings/issues)

AC_CONFIG_HEADERS([config.h])
AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_AUX_DIR([build-aux])

AM_INIT_AUTOMAKE([-Wall -Werror])
AM_MAINTAINER_MODE([disable])
AM_SILENT_RULES([yes])

AC_PROG_CC

dnl ***************************************************************************
dnl Internationalization
dnl ***************************************************************************

IT_PROG_INTLTOOL(0.35.0)
GETTEXT_PACKAGE=dasom-settings
AC_DEFINE_UNQUOTED(GETTEXT_PACKAGE, "$GETTEXT_PACKAGE", [gettext package name])
AC_SUBST(GETTEXT_PACKAGE)
AM_GLIB_GNU_GETTEXT
AM_GLIB_DEFINE_LOCALEDIR(DASOM_SETTINGS_LOCALE_DIR)

LT_INIT([disable-static])

PKG_CHECK_MODULES(GTK3, [gtk+-3.0])

GLIB_GSETTINGS

AC_OUTPUT([
  Makefile
  src/Makefile
  po/Makefile.in
])
