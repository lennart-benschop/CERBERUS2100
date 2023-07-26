# CERBERUS 2100™
The amazing multi-CPU, BASIC-programmable microcomputer with powerful, generic expansion capabilities! CERBERUS 2100™ is the successor of <a href="https://github.com/TheByteAttic/CERBERUS2080">CERBERUS 2080™</a>, which is now obsolete.

![IMG_0601 Background Removed small](https://github.com/TheByteAttic/CERBERUS2100/assets/69539226/88f6fabf-902e-4ba8-89cf-b806ca0061c0)

CERBERUS 2100™ is an educational multi-processor 8-bit computer, featuring both Z80 and 6502 CPUs, plus an AVR processor as I/O controller. Built with CPLDs, CERBERUS 2100™ is fully programmable even with respect to its hardware, at the individual gate and flip-flop level. It runs BASIC interpreters for both CPUs, but can also be used in a 'bare metal' mode through its built-in BIOS. It can even be extended through its expansion slot, which comes paired with a powerful, generic communications protocol that allows for Direct Memory Access (DMA). A detailed description of CERBERUS 2100™ is available in the <a href="https://github.com/TheByteAttic/CERBERUS2100/blob/main/CERBERUS%202100%20Hardware%20Manual.pdf">Hardware Manual</a>.<br><br>
CERBERUS 2100™ is a collaboration of three developers: Alexander Sharikhin (<a href="https://github.com/nihirash/cerberus-w65c02s-basic">6502 BASIC interpreter</a>, BIOS optimizations, and test code optimizations), Dean Belfield (<a href="https://github.com/breakintoprogram/cerberus-bbc-basic">Z80 BASIC interpreter</a> and BIOS optimizations), and myself (hardware, original test code, and original BIOS code). The <a href="https://github.com/TheByteAttic/CERBERUS2100/blob/main/CERBERUS%202100%20Hardware%20Manual.pdf">Hardware Manual</a> does not document the software, so you should visit <a href="https://github.com/nihirash/cerberus-w65c02s-basic">Alexander's</a> and <a href="https://github.com/breakintoprogram/cerberus-bbc-basic">Dean's</a> repositories for that.<br><br>
The applications in the directory <a href="https://github.com/TheByteAttic/CERBERUS2100/tree/main/Cerberus%20uSD%20card%20files">Cerberus uSD card files/</a> contain code from Alexander and Dean, but also software developed by others, namely: a <a href="https://github.com/lennart-benschop/cerberus-z80-forth">FORTH interpreter for CERBERUS 2100's Z80 CPU</a>, ported by Lennart Benschop, and the <a href="https://github.com/envenomator/cerberus2080-sokoban">SOKOBAN game ported to CERBERUS 2100's 6502 CPU</a>, by Jeroen Venema.<br><br>
CERBERUS 2100's BIOS code uses a modified version of the <a href="https://github.com/PaulStoffregen/PS2Keyboard">Arduino PS/2 Keyboard Library by Paul Stoffregen</a>, which we gratefully acknowledge.<br><br>
The directories in this repository are as follows:
<UL>
  <LI><a href="https://github.com/TheByteAttic/CERBERUS2100/tree/main/CAT">CAT</a>: constains the BIOS code for FAT-CAT, CERBERUS 2100's I/O controller. This code is simply an Arduino sketch written in C and resides in FAT-CAT's on-board flash memory.</LI>
  <LI><a href="https://github.com/TheByteAttic/CERBERUS2100/tree/main/CERBERUS%20Applications%20Source%20Code">CERBERUS Applications Source Code</a>: contains the assembly source codes of four test programs, which illustrate how assembly code can be written for CERBERUS 2100™, including communication between CPU and I/O processor.</LI>
  <LI><a href="https://github.com/TheByteAttic/CERBERUS2100/tree/main/CPLD_Files">CPLD_Files</a>: contains the design and JEDEC files for the three CPLDs used in CERBERUS 2100™ as its custom chipset.</LI>
  <LI><a href="https://github.com/TheByteAttic/CERBERUS2100/tree/main/Cerberus%20uSD%20card%20files">Cerberus uSD card files</a>: contains the files users should copy to a class-10 (or higher), FAT32-formatted micro SD card to be inserted in CERBERUS 2100™ prior to starting it up. The files contain the character set definitions, both BASIC interpreters, BASIC programs, test code, and other applications.</LI>
  <LI><a href="https://github.com/TheByteAttic/CERBERUS2100/tree/main/Design">Design</a>: contains the design files of the CERBERUS 2100™ board, including schematics and PCB design files.</LI>
  <LI><a href="https://github.com/TheByteAttic/CERBERUS2100/tree/main/Manufacturing">Manufacturing</a>: contains the files needed to have CERBERUS 2100™ boards made by your favorite PCB manufacturer. The files include the Gerber set, Bill of Materials, and Pick & Place (a.k.a. centroid) specifications.</LI>
  <LI><a href="https://github.com/TheByteAttic/CERBERUS2100/tree/main/Photos">Photos</a>: contains high-resolution, properly illuminated photos of a correctly assembled CERBERUS 2100™ unit. These photos can be used as reference for manual assembly, or to illustrate articles on CERBERUS 2100™. If you are a journalist, member of the media, or tech blogger, please feel free to use these photos without need to request explicit authorization from me.</LI>
</UL>
<br>
Copyright © 2023 by Bernardo Kastrup. All rights reserved. Provided under <a href="https://github.com/TheByteAttic/CERBERUS2100/blob/main/LICENSE">license</a>.
<br>
<hr>
<b>CHANGE HISTORY:</b><br><br>
  <UL>
    <LI><b>26 July 2023:</b> Corrections and extensions to the Hardware Manual.</LI>
    <LI><b>26 July 2023:</b> Full initial commit.</LI>
  </UL>
