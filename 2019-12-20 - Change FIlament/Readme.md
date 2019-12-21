# 2019-12-20 - Filament Change Enablement

This firmware build was based on `Marlin bugfix-2.0` at the repository commit [`bbe0ffb2fafad854457390540ca47165e62986b9`](https://github.com/MarlinFirmware/Marlin/commit/bbe0ffb2fafad854457390540ca47165e62986b9)

It contains all the changes from `Configuration.h`, `Configuration_adv.h` and `platformio.ini` from the Bigtreetech SKR Mini E3 repo at commit [`7ad2aaf2305f28dd521490a7a08886f3fac09ab3`](https://github.com/bigtreetech/BIGTREETECH-SKR-mini-E3/commit/7ad2aaf2305f28dd521490a7a08886f3fac09ab3)

It contains the following additional changes:

- Uncommenting of the `NOZZLE_PARK_FEATURE` to enable filament changing from LCD and GCode
- Uncommenting of the `ADVANCED_PAUSE_FEATURE` to enable filament changing from LCD and GCode
- Correction of some definition names as warned by the compiler:
  -  `FILAMENT_UNLOAD_RETRACT_LENGTH` to `FILAMENT_UNLOAD_PURGE_RETRACT`
  -  `FILAMENT_UNLOAD_DELAY` to `FILAMENT_UNLOAD_PURGE_RETRACT`

_All changes can be found in the patch.diff file_