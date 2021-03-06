# v01-03-01

* 2017-06-30 Andre Sailer ([PR#6](https://github.com/iLCSoft/DDKalTest/pull/6))
  - CMake: Drop dependency on DDkalTestLibDeps.cmake

# v01-03

* 2017-05-09 Andre Sailer ([PR#3](https://github.com/iLCSoft/DDKalTest/pull/3))
  - Dropped support for root version < 6

* 2017-06-20 Andre Sailer ([PR#4](https://github.com/iLCSoft/DDKalTest/pull/4))
  - Adapt to namespace changes in DD4hep

* 2017-06-29 Andre Sailer ([PR#5](https://github.com/iLCSoft/DDKalTest/pull/5))
  - CMake Configuration cleanup: Remove linking against Geant4
  - Require CMake 3.3 (same as DD4hep)

# v01-02

* 2017-04-07 Emilia Leogrande ([PR#2](https://github.com/iLCSoft/DDKalTest/pull/2))
  - DDKalTestConf replaced by LCTrackerConf

# v01-01
A.Sailer
* DDKalTest::CellIDEncoding: implement set_encoding_string and add access protection.

F.Gaede
* fix treatment of ROOT in CMakeLists.txt

# v01-00-01
A.Sailer
* DDParallelPlanarMeasLayer: protect against basically infinite loop if phi value is very very large
* DDKaltest: Ignore warnings from external header files
 
# v01-00
F.Gaede
* fixed the sorting policy for zdisks -> major improvement in forward track fitting
* crosscheck of energy loss from aidaTT commented out
* made compatible with c++11 and ROOT6
* added DDSurfaces::ISurface* surface() and some debug output
* remove hard coded muon mass for track fits

# v00-03
F.Gaede
* use new (faster) standalone helix intersection methods
* workaround for hits that are smeared off the DDRec::surface in the old digitizer
* added DDConeMeasLayer
* fixed bug in energy loss and multiple scattering for non-planar surfaces ( compute normal at x'ing point)
* distinguish between zplanes, disks and generic planes for sorting policy
* switch back to use SurfaceHelper class in order to get all insensitive surfaces ( lost in SurfaceMap )
* fixed some compiler warnings
 
# v01-00

F.Gaede
* added DDSurfaces::ISurface* surface() and some debug output 
* remove hard coded muon mass for track fits 
* fixed the sorting policy for zdisks -> major improvement in forward track fitting
* crosscheck of energy loss from aidaTT
* commented out 
* made compatible with c++11 and ROOT6


# v00-03
 F.Gaede
* adjusted some loge levels for debug ...
* use new (faster) standalone helix intersection methods
* workaround for hits that are smeared off the DDRec::surface in the old digitizer
* added DDConeMeasLayer
* fixed bug in energy loss and multiple scattering for non-planar surfaces ( compute normal at x'ing point)
* distinguish between zplanes, disks and generic planes for sorting policy
* replaced WARNING w/ DEBUG for debug printout
* switch back to use SurfaceHelper class in order to get all insensitive suirfaces ( lost in SurfaceMap )
* fixed some compiler warnings

# v00-02
* changed to just use abstract ISurface and ICylinder

# v00-01
* first release with basic functionality
