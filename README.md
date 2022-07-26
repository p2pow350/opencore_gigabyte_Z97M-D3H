# Let's start!

I'm a long time real Mac user and I'm using my Macs for coding/working, and beside that, I had my previous High Sierra Clover installation broken and need to repair. 
This was my journey to OC I which I've spent two weeks trying to boot and install Monterey on my Desktop using OC on my Gigabyte Z97 motherboard using integrated Video and Audio and LAN.
Maybe this repo can be useful for someone to quick start.
The configuration is using OpenCore with debug enabled

## Hardware

- Motherboard Gigabyte Z97 D3H (https://www.gigabyte.com/Motherboard/GA-Z97M-D3H-rev-10#ov) with Integrated Audio ALC862 and Ethernet
- Intel i4790k with HD4600 Integrated Video
- Samsung SSD dedicated HD (not _NVMe_) 
- Case Bitfenix Prodigy (https://www.bitfenix.com/products/chassis/mini-itx/prodigy/)

## Software
- [GenSMBIOS] for generating unique serial number (https://github.com/corpnewt/GenSMBIOS)
- [OpenCore Configurator](https://mackie100projects.altervista.org/opencore-configurator/) for mounting EFI partition within USB bootable


# Instructions
- Run GenSMBIOS and generate serial for this spec iMac16,1
- Modify Serial number in text file under folder OC/config.plist
- Save and copy EFI folder into the USB mounted EFI partition
- Modify BIOS Settings to boot from EFI
- That's it!

## Working
- Audio, Video, LAN
- All USB Ports (USB2 /USB3, including USB3 in the front panel)

## Missing
- Wifi / Bluetooth (maybe I need to buy a Fenvi card)
