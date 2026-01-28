# reason for test
Partial update not implemented for this display in the following Arduino libraries  
- <https://github.com/ZinggJM/GxEPD2>
- <https://github.com/Seeed-Studio/Seeed_GFX>

# origin of example
Downloaded code from  
<https://www.good-display.com/product/533.html> ->  
`Download` ->  
`GDEP073E01 ESP32 Sample Code (Full update within a specified area)` ->  
`Download`

or

<https://www.good-display.com/companyfile/1908.html> ->  
`Download`

# changes
adapted for Seeedstudio reTerminal E1002 and platformio

# commands
- compile
```
$ pio run
```
- compile and upload
```
$ pio run -t upload
```
- serial monitor
```
$ pio run -t monitor
Processing seeed_xiao_esp32s3 (platform: espressif32; board: seeed_xiao_esp32s3; framework: arduino)
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Esp32ExceptionDecoder: ROM ELF found at /home/alex/.platformio/packages/tool-esp-rom-elfs/esp32_rev0_rom.elf

Please build project in debug configuration to get more details about an exception.
See https://docs.platformio.org/page/projectconf/build_configurations.html


--- Terminal on /dev/ttyUSB0 | 115200 8-N-1
--- Available filters and text transformations: colorize, debug, default, direct, esp32_exception_decoder, hexlify, log2file, nocontrol, printable, send_on_enter, time
--- More details at https://bit.ly/pio-monitor-filters
--- Quit: Ctrl+C | Menu: Ctrl+T | Help: Ctrl+T followed by Ctrl+H
10:31:24.064 > ESP-ROM:esp32s3-20210327
10:31:24.064 > Build:Mar 27 2021
10:31:24.064 > rst:0x1 (POWERON),boot:0x29 (SPI_FAST_FLASH_BOOT)
10:31:24.064 > SPIWP:0xee
10:31:24.064 > mode:DIO, clock div:1
10:31:24.064 > load:0x3fce2820,len:0x116c
10:31:24.064 > load:0x403c8700,len:0xc2c
10:31:24.064 > load:0x403cb700,len:0x3108
10:31:24.064 > entry 0x403c88b8
10:31:24.202 > Setup started
10:31:24.203 > SPI initialized
10:31:25.007 > start
10:31:25.008 > done
10:31:30.007 > Chessboard initialized
10:31:30.007 > Displaying initial chessboard
10:31:50.103 > Chessboard displayed
10:31:55.103 > Updating (2, 2) to RED
10:32:14.460 > Partial window updated
10:32:14.460 > Manual partial update completed
10:32:19.461 > Updating (4, 4) to YELLOW
10:32:38.825 > Partial window updated
10:32:38.825 > Manual partial update completed
10:32:43.826 > Clearing display
10:33:03.915 > Display cleared
10:33:05.915 > Program finished
```

# links
- [YouTube:Watch 7.3" E Ink Spectra 6 Instantly Refresh Just a Section (No Flashing!) | Full-Color EPaper](https://www.youtube.com/watch?v=PXS-hDX7hjo)
- https://github.com/ZinggJM/GxEPD2/discussions/161
