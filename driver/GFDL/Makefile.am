# This is the main automake file for GFDL_atmos_cubed_sphere
# driver/GFDL directory.
# Ed Hartnett 7/26/2019

# Include .h and .mod files.
# AM_CPPFLAGS = -I${top_srcdir}/include

# Build this uninstalled convenience library. Does not work due to
# missing atmos_co2_mod. See github issue
# https://github.com/NOAA-GFDL/GFDL_atmos_cubed_sphere/issues/3.
#noinst_LTLIBRARIES = libatmosphere.la

# The convenience library depends on its source.
#libatmosphere_la_SOURCES = atmosphere.F90

# Mod file depends on its o file, is built and then installed.
#atmosphere_mod.mod: atmosphere.$(OBJEXT)

# Some mods are dependant on other mods in this dir.
#atmosphere.$(OBJEXT): atmos_co2_mod.mod

#BUILT_SOURCES = atmosphere_mod.mod
#include_HEADERS = atmosphere_mod.mod

CLEANFILES = *.mod
