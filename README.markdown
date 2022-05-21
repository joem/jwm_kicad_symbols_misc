jwm_kicad_symbols_misc
======================

This is a collection of miscellaneous symbols for [KiCad](https://kicad.org). Currently, this is my only custom symbols library, but it's also a holding library before I can break symbols out into separate specialized libraries.

(You might also be interested in my related [misc footprints library](https://github.com/joem/jwm_kicad_footprints_misc.pretty) and [misc 3D models library](https://github.com/joem/jwm_kicad_3dmodels_misc.3dshapes) for KiCad.)

Symbols included in this library:

Symbol name | Description
----------- | -----------
74VHC4046N_LZX | a 74VHC4046N IC, made to look like the ones found in LZX's Cadet schematics
Eurorack_Header_LZX | a Eurorack synth power header, made to look like the ones found in LZX's Cadet schematics (see note 1)
Eurorack_Header_LZX_NC-5vCvGate | same as Eurorack_Header_LZX, but with +5V, CV, and Gate permanently not connected
Eurorack_Header_LZX_NC-CvGate | same as Eurorack_Header_LZX, but with CV and Gate permanently not connected
Eurorack_Header_LZX_NC-5v | same as Eurorack_Header_LZX, but with +5V permanently not connected
INA3221_Module | an INA3221 module, controlled by I2C
INA3221_Module_NoVPU | an INA3221 module, controlled by I2C, without a VPU pin
LMH1980 | a LMH1980 sync separator IC
LT1251_LZX | a LT1251 IC, made to look like the ones found in LZX's Cadet schematics
SSD1306_I2C_OLED_Module | an SSD1306 I2C OLED module
SW_DPDT_LZX | a DPDT switch, made to look like the ones found in LZX's Cadet schematics
Sync_Header_LZX | a LZX 14-pin sync header, made to look like the ones found in LZX's Cadet schematics

Note 1: Due to the way the pin stacking works in `Eurorack_Header_LZX`, if you use NC flag on any of the pins, the ERC will give you a warning that pins marked NC are connected. To get around this, use one of the `_NC-...` variations that have a permanent NC on certain pins built in to the symbol.

(Yes, so far they're mostly made to look like symbols from LZX's Cadet schematics which were made in Diptrace. As I work on more circuits in the future, I'll be adding more that are not emulating LZX's parts.)

For an easy preview of what these symbols look like, look in the [images](images/) folder.

Please feel free to use these symbols as you'd like in your own projects. If they help you, I'm glad.

