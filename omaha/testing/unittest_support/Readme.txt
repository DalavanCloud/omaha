This directory contains binaries, etc. needed for the unit tests.

In particular, the "test" project is not currently built by default, so the test .msi files aren't necessarily available for unit tests.
setup_foo_v1.0.101.0.msi is built from ..\..\test\test_foo.wxs.xml.

SaveArguments.exe must be updated periodically to keep its signature from being more than N days old where N is defined in google_update_recovery.cc.

* omaha_1.0.x contains files from the last official release of Omaha 1.0.x.
  - One use is testing the legacy quiet mode (shutdown) event.
* omaha_1.1.x contains files from the last version of Omaha 1.1.x.
  - One use is testing the quiet mode (shutdown) event.
* omaha_1.2.x contains an older version of Omaha 1.2.x.
  - One use is testing the shutdown event works with older versions.
* omaha_1.3.x contains an older version of Omaha 1.3.x.
  - One use is testing the shutdown event works with older versions.
* omaha_1.3.x_newer contains a version that is newer than any expected build.
  - GoogleUpdate.exe was generated by hardcoding the four version values in generated_resources_en.rc and building.
  