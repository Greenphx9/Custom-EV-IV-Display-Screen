# Custom-EV-IV-Display-Screen
Customizable Base Stat, EV, and IV checker for Pokemon Fire Red.
Original by Acimut (https://github.com/Acimut/Custom-EV-IV-Display-Screen)
Black/White styled background by Versekr Dark.
Translated to English by me (original is in Spanish)

The files inside the src \ include \ folder were taken from pokefirered.
 
Features
-
+ Changable background using Gale Wings and Tilemap Studio. It is automatically injected to the rom.
+ You can change the coordinates of the Pokémon sprite, as well as the text (attack, def, etc)
+ The color of the IVs statistic changes according to nature.
+ Shows base statistics of Pokemon
+ Shows IVs and EVs of the Pokemon
+ Shows how many steps a Egg will hatch in.
+ For Pokemon Fire Red

Bugs
-
+ Weird pinkish purple colour on top right of display

***Notes:***

-DevkitARM required to build.

- Gbagfx.exe and preproc.exe also required.

- Put Fire Red 1.0 rom called BPRE0.gba and run make in command prompt

- Open the Makefile file, find and change ff0000 of the following line to insert to a different offset (more than 0x2000 bytes):
        `export INSERT_INTO: = 0x08ff0000`

- Use in a `callasm` script followed by offset + 1 where they inserted the code.
         `Example: callasm 0x08ff0001 (where you inserted +1)`

- Will make the rom "rom.gba" when inserted.

- Files inside the include folder were taken from pokefirered.

- The incbin.h file is taken from the following repository: https://github.com/graphitemaster/incbin

