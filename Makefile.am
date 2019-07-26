# This is the main automake file for GFDL_atmos_cubed_sphere.
# Ed Hartnett 7/22/2019

# This directory stores libtool macros, put there by aclocal.
ACLOCAL_AMFLAGS = -I m4

# Find the constants_mod.mod file.
#AM_CPPFLAGS=-I${top_builddir}/driver/SHiELD

# Make targets will be run in each subdirectory. Order is significant.
#SUBDIRS = driver GFDL_tools model model_nh tools
#SUBDIRS = driver .

# Build these uninstalled convenience libraries.
noinst_LTLIBRARIES = driver/SHiELD/liblin_cld_microphys.la		\
driver/SHiELD/libconstants.la model/libfv_arrays.la			\
tools/libfv_diagnostics.la tools/libfv_eta.la tools/libexternal_ic.la	\
tools/libexternal_sst.la tools/libfv_grid_tools.la tools/libfv_io.la	\
tools/libfv_mp_mod.la tools/libfv_nggps_diag.la tools/libfv_nudge.la	\
tools/libfv_restart.la tools/libfv_surf_map.la tools/libfv_timing.la	\
tools/libinit_hydro.la tools/libsim_nc_mod.la				\
tools/libsorted_index.la tools/libtest_cases.la model/liba2b_edge.la	\
model/libboundary.la model/libdyn_core.la model/libfv_cmp.la		\
model/libfv_control.la model/libfv_current_grid.la			\
model/libfv_dynamics.la model/libfv_fill.la model/libfv_grid_utils.la	\
model/libfv_mapz.la model/libfv_nesting.la model/libfv_sg.la		\
model/libfv_tracer2d.la model/libfv_update_phys.la			\
model/libsw_core.la model/libtp_core.la

#The convenience libries depends on their source.
driver_SHiELD_libconstants_la_SOURCES = driver/SHiELD/constants.F90
driver_SHiELD_liblin_cld_microphys_la_SOURCES = driver/SHiELD/lin_cloud_microphys.F90
tools_libtest_cases_la_SOURCES = tools/test_cases.F90
tools_libsorted_index_la_SOURCES = tools/sorted_index.F90
tools_libsim_nc_mod_la_SOURCES = tools/sim_nc_mod.F90
tools_libinit_hydro_la_SOURCES = tools/init_hydro.F90
tools_libfv_timing_la_SOURCES = tools/fv_timing.F90
tools_libfv_surf_map_la_SOURCES = tools/fv_surf_map.F90
tools_libfv_restart_la_SOURCES = tools/fv_restart.F90
tools_libfv_nudge_la_SOURCES = tools/fv_nudge.F90
tools_libfv_nggps_diag_la_SOURCES = tools/fv_nggps_diag.F90
tools_libfv_mp_mod_la_SOURCES = tools/fv_mp_mod.F90
tools_libfv_io_la_SOURCES = tools/fv_io.F90
tools_libfv_grid_tools_la_SOURCES = tools/fv_grid_tools.F90
tools_libfv_eta_la_SOURCES = tools/fv_eta.F90
tools_libfv_diagnostics_la_SOURCES = tools/fv_diagnostics.F90
tools_libexternal_sst_la_SOURCES = tools/external_sst.F90
tools_libexternal_ic_la_SOURCES = tools/external_ic.F90
model_libtp_core_la_SOURCES = model/tp_core.F90
model_libsw_core_la_SOURCES = model/sw_core.F90
model_libfv_update_phys_la_SOURCES = model/fv_update_phys.F90
model_libfv_tracer2d_la_SOURCES = model/fv_tracer2d.F90
model_libfv_sg_la_SOURCES = model/fv_sg.F90
model_libfv_nesting_la_SOURCES = model/fv_nesting.F90
model_libfv_mapz_la_SOURCES = model/fv_mapz.F90
model_libfv_grid_utils_la_SOURCES = model/fv_grid_utils.F90
model_libfv_fill_la_SOURCES = model/fv_fill.F90
model_libfv_dynamics_la_SOURCES = model/fv_dynamics.F90
model_libfv_current_grid_la_SOURCES = model/fv_current_grid.F90
model_libfv_control_la_SOURCES = model/fv_control.F90
model_libfv_cmp_la_SOURCES = model/fv_cmp.F90
model_libfv_arrays_la_SOURCES = model/fv_arrays.F90
model_libdyn_core_la_SOURCES = model/dyn_core.F90
model_libboundary_la_SOURCES = model/boundary.F90
model_liba2b_edge_la_SOURCES = model/a2b_edge.F90

# Mod file depends on its o file, is built and then installed.
driver/SHiELD/constants_mod.mod: driver/SHiELD/constants.$(OBJEXT)
driver/SHiELD/lin_cld_microphys_mod.mod: driver/SHiELD/lin_cloud_microphys.$(OBJEXT)
model/fv_arrays_mod.mod: model/fv_arrays.$(OBJEXT)
tools/external_ic_mod.mod: tools/external_ic.$(OBJEXT)
tools/test_cases_mod.mod: tools/test_cases.$(OBJEXT)
tools/sorted_index_mod.mod: tools/sorted_index.$(OBJEXT)
tools/sim_nc_mod.mod: tools/sim_nc_mod.$(OBJEXT)
tools/init_hydro_mod.mod: tools/init_hydro.$(OBJEXT)
tools/fv_timing_mod.mod: tools/fv_timing.$(OBJEXT)
tools/fv_surf_map_mod.mod: tools/fv_surf_map.$(OBJEXT)
tools/fv_restart_mod.mod: tools/fv_restart.$(OBJEXT)
tools/fv_nudge_mod.mod: tools/fv_nudge.$(OBJEXT)
tools/fv_nggps_diag_mod.mod: tools/fv_nggps_diag.$(OBJEXT)
tools/fv_mp_mod.mod: tools/fv_mp_mod.$(OBJEXT)
tools/fv_io_mod.mod: tools/fv_io.$(OBJEXT)
tools/fv_grid_tools_mod.mod: tools/fv_grid_tools.$(OBJEXT)
tools/fv_eta_mod.mod: tools/fv_eta.$(OBJEXT)
tools/fv_diagnostics_mod.mod: tools/fv_diagnostics.$(OBJEXT)
tools/external_sst_mod.mod: tools/external_sst.$(OBJEXT)
model/a2b_edge_mod.mod: model/a2b_edge.$(OBJEXT)
model/tp_core_mod.mod: model/tp_core.$(OBJEXT)
model/sw_core_mod.mod: model/sw_core.$(OBJEXT)
model/fv_update_phys_mod.mod: model/fv_update_phys.$(OBJEXT)
model/fv_tracer2d_mod.mod: model/fv_tracer2d.$(OBJEXT)
model/fv_sg_mod.mod: model/fv_sg.$(OBJEXT)
model/fv_nesting_mod.mod: model/fv_nesting.$(OBJEXT)
model/fv_mapz_mod.mod: model/fv_mapz.$(OBJEXT)
model/fv_grid_utils_mod.mod: model/fv_grid_utils.$(OBJEXT)
model/fv_fill_mod.mod: model/fv_fill.$(OBJEXT)
model/fv_dynamics_mod.mod: model/fv_dynamics.$(OBJEXT)
model/fv_current_grid_mod.mod: model/fv_current_grid.$(OBJEXT)
model/fv_control_mod.mod: model/fv_control.$(OBJEXT)
model/fv_cmp_mod.mod: model/fv_cmp.$(OBJEXT)
model/dyn_core_mod.mod: model/dyn_core.$(OBJEXT)
model/boundary_mod.mod: model/boundary.$(OBJEXT)

# Some mods are dependant on other mods in this dir.
tools/external_ic.$(OBJEXT): tools/external_sst_mod.mod			\
tools/fv_diagnostics_mod.mod tools/fv_io_mod.mod tools/fv_mp_mod.mod	\
tools/fv_surf_map_mod.mod tools/fv_timing_mod.mod			\
tools/init_hydro_mod.mod tools/fv_eta_mod.mod tools/sim_nc_mod.mod	\
tools/test_cases_mod.mod model/boundary_mod.mod
tools/fv_diagnostics.$(OBJEXT): model/fv_arrays_mod.mod	\
model/fv_mapz_mod.mod model/a2b_edge_mod.mod		\
tools/fv_surf_map_mod.mod model/fv_sg_mod.mod
model/fv_mapz.$(OBJEXT): model/fv_grid_utils_mod.mod model/fv_fill_mod.mod model/fv_cmp_mod.mod
model/fv_grid_utils.$(OBJEXT): tools/fv_eta_mod.mod tools/fv_timing_mod.mod
tools/fv_eta.$(OBJEXT): tools/fv_mp_mod.mod
tools/test_cases.$(OBJEXT): tools/fv_grid_tools_mod.mod
tools/fv_grid_tools.$(OBJEXT): tools/sorted_index_mod.mod

# The modfiles are built in the order listed here, also honoring the
# dependencies of each mod file, specified above.
MODFILES = driver/SHiELD/constants_mod.mod				\
driver/SHiELD/lin_cld_microphys_mod.mod model/fv_arrays_mod.mod		\
tools/external_ic_mod.mod tools/external_sst_mod.mod			\
tools/fv_diagnostics_mod.mod tools/fv_eta_mod.mod			\
tools/fv_grid_tools_mod.mod tools/fv_io_mod.mod tools/fv_mp_mod.mod	\
tools/fv_nggps_diag_mod.mod tools/fv_nudge_mod.mod			\
tools/fv_restart_mod.mod tools/fv_surf_map_mod.mod			\
tools/fv_timing_mod.mod tools/init_hydro_mod.mod tools/sim_nc_mod.mod	\
tools/sorted_index_mod.mod tools/test_cases_mod.mod			\
model/a2b_edge_mod.mod model/boundary_mod.mod model/dyn_core_mod.mod	\
model/fv_cmp_mod.mod model/fv_control_mod.mod				\
model/fv_current_grid_mod.mod model/fv_dynamics_mod.mod			\
model/fv_fill_mod.mod model/fv_grid_utils_mod.mod			\
model/fv_mapz_mod.mod model/fv_nesting_mod.mod model/fv_sg_mod.mod	\
model/fv_tracer2d_mod.mod model/fv_update_phys_mod.mod			\
model/sw_core_mod.mod model/tp_core_mod.mod
BUILT_SOURCES = ${MODFILES}
include_HEADERS = ${MODFILES}

CLEANFILES = *.mod

EXTRA_DIST = README.md LICENSE.md
