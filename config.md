# Details about the `example.cfg` file

2 Sections

## Section 1

6 values:
* First 3 are for RAM  - `ZP`, `OAM`, `RAM`
* Last 3 are for ROM - `HDR`, `PRG`, `CHR`

### Random Access Memory (RAM)

`ZP` - Size 256 bytes - Zero-Page Memory

`OAM` - Size 256 bytes - "Object Attribute Memory" - Special section of RAM - Sprite Definition Table Table contains the position, shape, and attributes of each of the sprites displayed on the screen

`RAM` - Size 1280 bytes - The remainder of the 2K (2048 RAM) 

### Read-Only Memory (ROM) 

`HDR` - Size 16 bytes - Special section of ROM - Added as a header on NES ROM file - Indicate to NES console emulators that the cartridge is an NES cartridge & allows some details of the features that the cartridge uses.

`PRG` - Size 32k bytes - Main ROM area - code & data for our program - 2 "banks" of 16K each for 32K total

`CHR` - Size 8k bytes - ROM - Contains the patterns for our tiles & sprites. Advantage of CHR tables is that we don't have to copy them into the graphic processor's video memory

## Section 2

This hosts the mapping of "labels" to their respective Memory definitions.
