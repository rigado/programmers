# Factory Images
Factory Images for Rigado BMD-300 and BMD-200 modules

This repository contains simple Windows-based programmers that will return the BMD-300 and BMD-200 modules to their factory programmed state. Select the folder with the device you wish to program, and then select the firmware code and programming type you wish to use.

Firmware Image 'AD' with a new MAC address for the BMD-200-Eval board: \Factory Images\BMD-200-EVAL\BMD-200-EVAL\_AD\_wMAC

### *Note about MAC addresses*

Any MAC address can be assigned, however Rigado provides a unique MAC address for every module. Rigado MAC addresses are always 94:54:93:XX:XX:XX, with the last 6 digits physically located on the module's label in human-readable text and in 2D barcode format (Data Matrix).

#### Programming Options:

* BMD-300 - AA and AB - Requires a MAC address be entered before programming is allowed. The factory programmed MAC address cannot be automatically saved and reprogrammed. Because readback protection disables the debug interface, the UICR location where the MAC address is saved is inaccessible. The desired MAC address can be typed or scanned into the program.
* BMD-300 - AC and AD - Requires a MAC address be entered before programming is allowed. However, readback protection is no longer enabled by default, and the MAC addresses can be read out with a JLink programmer. Readback protection is now automatically enabled by the bootloader when an encryption key is loaded.
* BMD-200 - Two options are provided; either the MAC address can be automatically saved or a new MAC address can be typed or scanned and then programmed.

*A Segger JLink programmer is required to use these utilities.*

### *Note about firmware version codes*

Firmware codes are assigned by product family; i.e. BMD-200 and BMD-300 codes do NOT refence the same bootloader and BMDware versions.

### BMD-200 Codes

* AA: Nordic S110 SoftDevice v6.0.0, Rigado RigDFU v1.0.0, and a factory test application
* AB: Nordic S110 SoftDevice v8.0.0, Rigado RigDFU v3.0.0, and BMDware v2.0.5
* AC: Nordic S110 SoftDevice v8.0.0, Rigado RigDFU v3.1.0, and BMDware v3.0.0
* AD: Nordic S110 SoftDevice v8.0.0, Rigado RigDFU v3.2.1, and BMDware v3.1.1

### BMD-300 Codes

* AA: Nordic S132 SoftDevice v2.0.0, Rigado RigDFU v3.2.0, and BMDware v3.1.0
* AB: Nordic S132 SoftDevice v2.0.0, Rigado RigDFU v3.2.1, and BMDware v3.1.1
* AC: Nordic S132 SoftDevice v2.0.0, Rigado RigDFU v3.2.2, and BMDware v3.1.1 (not readback protected, not used in factory production)
* AD: Nordic S132 SoftDevice v3.1.0, Rigado RigDFU v3.3.1, and BMDware v3.2.0 (not readback protected)