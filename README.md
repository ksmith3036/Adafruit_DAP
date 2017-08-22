# Adafruit_DAP
Port of Free-DAP + edbg CMSIS-DAP controller software to Arduino

This is a library that allows you to program Stmel Cortex M0 chips that support programming via DAP from an arduino-compatible board. Tested with a Metro M0 / Arduino Zero as the 'host' and with ATSAMD21's as the client but in theory any 3.3V Arduino board will work as host (just slower)

Works completely stand-alone, firmware is read from an SD card and uploaded directly from chip-to-chip. There are no computers required!

This is mostly a re-mix of Alex Taradovs excellent Free-DAP code @ https://github.com/ataradov/free-dap - we just put both halves into one library and wrapped it up in Arduino compatibility

Other ARM chips should be (easily?) supportable. Copy Adafruit_DAP_SAM to a new file and make changes to support your favorite SWD-programmable chip.