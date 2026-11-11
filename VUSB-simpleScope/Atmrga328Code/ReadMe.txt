// this scope is for tutorial purpose only, it does not generate precised waveform

Define the F_CPU in the main code and also in the 

project>[project name] properties > Toolchain > AVR/GNU Assembler > General

Assembler Flags: -DF_CPU=16000000

//-----------------------------------------------

also add the usbdrv folder (library) location to AVR\GNU C Compiler > Directories

include Paths(-l)

//----------------------------------
 This usbconfig.h is configured in such a way that the pc detects it as a HID > usb input device, where the commuication is always started or data is requested by the host/PC.
