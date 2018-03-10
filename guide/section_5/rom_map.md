# ROM Map

This is meant to visualize where all data in the rom is stored. Each bank is `16kb` in size, and can 
be swapped in as needed. The only exception is the PRG section, which is always loaded. It contains
library code that is always accessible, as well as banking code. 

Any banks marked as unused are great targets for your own code. You can also move things from other
banks into them by changing their associated `PRG_BANK_TYPE` define in the header file.


## PRG (always loaded)
- NESLib
- Main program loop
- prg/chr/etc banking routines
- Famitracker music library

## ROM_00
- Music data
- Sound effect data

## ROM_01
- Error handler screen

## ROM_02
- Title screen
- Various menus
- Pause Menu
- Level drawing logic
- Hud logic
- Player sprite/movement logic

## ROM_03
- Level data

## ROM_04
- Unused

## ROM_05
- Unused

## ROM_06
- Unused

## ROM_07
- Unused