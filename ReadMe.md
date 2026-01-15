 # **EmuProm** -- A Universal EPROM Emulator for 2716, 2732, 2764, 27128 and 27256

This repo documents a universal EPROM plug-in emulator which I designed and built in July 1985. It found good use from 1985 onwards when I was interactively designing the Z80 firmware for my Phoenix MIDI computer, my 'Colossus Control Computer' and the rewritten Exceltronix Multiflex VT52 terminal.

<div style="text-align:center">
<img src="/Images/Img1.jpg" alt="" style="width:75%; height:auto;">
</div>

This would interface to one of my four main Z80 computers via my own "Universal I/O Port" which I had added to each of the machines. The pinout can be found at the end of [this page](https://github.com/rcl9/Cypher-Z80-68000-Single-Board-Computer----Expansion-Board).

It allows for an in-circuit EPROM chip to be replaced with one of two specialized programmable modules:

<div style="text-align:center">
<img src="/Images/Img3.jpg" alt="" style="width:45%; height:auto;">   <img src="/Images/Img4.jpg" alt="" style="width:45%; height:auto;">
</div>

## Source Code

The Z80 assembler source code is contained in the main [.asm](/src/EmuProm.mac) file.

## Schematics - Main Logic Board

The main logic board provides this functionality:

- 16 2kx8 static memory chips providing 32k of memory
- Buffering to the memory from both the **Universal I/O Bus** and the **Plug-In Module**

<div style="text-align:center">
<img src="/Schematics/EPROM emulator module schematics -2.jpg" alt="">
</div>

## Schematics - Plug-In Module for 2716, 2732 and 2532

The two plug-in modules allow the EPROM-in-circuit to connect up with the buffered shared memory.

<div style="text-align:center">
<img src="/Schematics/EPROM emulator module schematics -4.jpg" alt="">
</div>

## Schematics - Plug-In Module for 2764, 27128 and 27256

<div style="text-align:center">
<img src="/Schematics/EPROM emulator module schematics -1.jpg" alt="">
</div>

## Schematics - Board and Pin Layouts

<div style="text-align:center">
<img src="/Schematics/EPROM emulator module schematics -3.jpg" alt="">
</div>
