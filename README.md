## Introduction

Your Commodore 64/128 machine can join the growing ranks of Internet  capable systems by installing the 64NIC+ Ethernet interface. 64NIC+  offers inexpensive Ethernet connectivity and more. Based on the Crystal  CS8900 10 megabit Ethernet interface engine, the interface emulates the  popular RR-NET solution as well as the NET64 and TFE systems.

Designed by RETRO Innovations initially as a fundraiser for the  Cincinnati Commodore Computer Club (CCCC), 64NIC+ allows the Commodore  user to experience online connectivity in true 8-bit glory. Play online Ethernet games, telnet to your favorite BBSes, and tweet from your  Commodore!

In addition to Ethernet capabilities, the system also includes an  optional on board ROM socket that can be loaded with up to 16 cartridge  images.  With the appropriate ROM, the 64NIC+ can autoboot and load  your favorite games and utilities via TCP/IP, no disk drive required.

Main features include:

- Self contained functionality. No pieces to disconnect
- 10 Mbit Ethernet connectivity
- RR-NET compatibility
- NET64/TFE compatibility
- C64 and C128 compatibility

Technical Features include:

- The ubiquitous RESET switch!
- Onboard optional ROM socket for autoboot functionality
- ROM socket can accommodate up to 256kB ROMs
- Optional rotary switch can select 1 of 16 ROM images
- Cartridge can be configured to reside in either IO1 or IO2 address spaces
- Cartridge can be configured to reside in any 16 byte address bank within the IO address space.

The 64NIC+ began as a fundraiser for the Cincinnati Commodore  Computer Club (C4), who felt a low-cost basic Ethernet cartridge would  be welcomed by the community. RETRO Innovations designed the cartridge, incorporating Eric Pratt’s 64NIC and Till Harbaum’s NET64 designs. A  ROM socket and associated configuration switches were added to maximize  use of PCB space.

## Options

64NIC+ comes in 4 variations:

1. base unit without case
2. base unit with case
3. unit with ROM-selecting rotary switch and no case
4. unit with ROM-selecting rotary switch and case

Network operation remains the same in all variants.

## Requirements

- 10Mbit capable Ethernet connection
- Ethernet cable
- C64/64C/C128/C128D/C128DCR/SX64
- 64NIC+, RR-NET, or NET64 compatible software (the product does not come with software on disk). A [software disk image](http://www.go4retro.com/downloads/64nic+/c64nic.d64) with software is available from the Cincinnati Commodore Computer Club web site

## Purchase

64NIC+ models can be purchased in the [RETRO Innovations Online Store](http://store.go4retro.com/products/64NIC%2b.html).

Units come with a 30 days return policy and 1 year warranty.

## Technical Details

64NIC+ interfaces the ISA-bus-compatible Crystal (Cirrus Logic)  CS8900A embedded ethernet controller with the C64/C128 bus. As the  CS8900A requires only 16 address locations, support logic allows the  base address to reside on any 16 byte boundary in the IO address space.  A toggle switch on the side of the unit selects IO1 or IO2 address  range. To support a normal mapping of the registers into the address  space and a “flipped” register setup as used by the RetroReplay RR-NET  interface, another switch changes the register configuration. The  remaining 2 switches enable the onboard 32-pin EPROM socket and select  whether 64 or 128 mode for the EPROM. Finally, the 16 position rotary  switch allows selection of 16kB banks of data from the EPROM.

Toggle switches are as follows, listed from switch located furthest from cartridge port edge connector:

| Switch | Function (Up)                 | Function (Down)        |
| ------ | ----------------------------- | ---------------------- |
| 1      | RR-NET Register Configuration | Standard Configuration |
| 2      | EPROM socket disabled         | EPROM socket enabled   |
| 3      | 128 mode for EPROM            | 64 mode for EPROM      |
| 4      | IO1 Usage                     | IO2 Usage              |

## Support

Any 5V JEDEC standard 28 or 32 pin EPROM, FLASH, or EEPROM IC can be  installed int the ROM socket. However, if a 28 pin IC is used, the  connection on the JP4 pads labeled “32” must be opened and the “28” pads must be shorted.

Jp5 normally allows the rotary switch to control all ROM banks.  However, by opening the pins marked “ROTARY” and closing the pads marked “TOGGLE”, the 128/64 toggle switch then controls the lowest bank  address pin of the EPROM. Thus, in each set of 2 banks, the lowest 16kB would contain a 64-compatible application, while the higher 16kB would  contain a 128-compatible application.

JP3 (located on bottom of cartridge PCB) can be opened to allow use  of 8kB ROM banks. However, note that only the lower 8kB of each 16kB  can be used without modification of the bank switching wiring.

JP1 configures the 16 byte register bank within the selected IO  region. In essence, it’s the upper 4 address lines of the register  bank. The default is ‘0000’, or all shorting blocks present. Removal  of a shorting block will set that address line high.

Pre-production and production unit photos are available at the [64NIC+ Photo Gallery](http://www.jbrain.com/vicug/gallery/nic/) and more information is available at the and the [Wiki Page](http://www.c64-wiki.com/index.php/C64NIC%2B).