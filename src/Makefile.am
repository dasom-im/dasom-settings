gsettings_SCHEMAS = org.freedesktop.Dasom.dasom-settings.gschema.xml
@GSETTINGS_RULES@

bin_PROGRAMS = dasom-settings

dasom_settings_SOURCES = dasom-settings.c
dasom_settings_CFLAGS  = -Wall -Werror -DG_LOG_DOMAIN=\"dasom\" $(GTK3_CFLAGS)
dasom_settings_LDFLAGS = $(GTK3_LIBS)

DISTCLEANFILES = Makefile.in
