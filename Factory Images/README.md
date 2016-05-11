# Factory Images
Factory Images for Rigado BMD-300 and BMD-200 modules

This repository contains simple Windows-based programmers that will return the BMD-300 and BMD-200 modules to their factory programmed state. Select the folder with the device you wish to program, and then select the firmware code and programming type you wish to use.

Firmware Image 'AD' with a new MAC address for the BMD-200-Eval board: \Factory Images\BMD-200-EVAL\BMD-200-EVAL\_AD\_wMAC

###*Note about MAC addresses*

Any MAC address can be assigned, however Rigado provides a unique MAC address for every module. Rigado MAC addresses are always 94:54:93:XX:XX:XX, with the last 6 digits physically located on the module's label in human-readable text and in 2D barcode format (Data Matrix).

####Programming Options:

* BMD-300 - Requires a MAC address be entered before programming is allowed. The factory programmed MAC address cannot be automatically saved and reprogrammed. Because readback protection disables the debug interface, the UICR location where the MAC address is saved is inaccessible. The desired MAC address can be typed or scanned into the program.
* BMD-200 - Two options are provided; either the MAC address can be automatically saved or a new MAC address can be typed or scanned and then programmed.


*A Segger JLink programmer is required to use these utilities.*