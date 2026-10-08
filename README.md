Y2JB Relapse Autoloader
Y2JB-Upload is an ELF payload that allows you to replace YouTube's download0.dat with the modified Relapse Autoloader.
The payload automatically detects your installed YouTube region and replaces the appropriate file, so it works with EU, JP, and US versions of YouTube.
Requirements
A compatible console with payload/ELF loading support
The appropriate YouTube PKG installed
The latest modified download0.dat from itsplk
A USB drive
y2jb-upload.elf
Installation
Install the appropriate YouTube PKG on your console, if you haven't already.
Download the most recent modified download0.dat from itsplk.
Place download0.dat on the root of your USB drive.
Place y2jb-upload.elf on the USB drive as well.
Connect the USB drive to your console.
Load y2jb-upload.elf using AutoLoader or manually through Payload Manager.
Select Flash y2jb.
The payload will automatically detect your YouTube region and install the appropriate version.
Region Detection
You don't need to manually select your YouTube region.
Y2JB-Upload automatically detects the installed YouTube version and selects the appropriate location for download0.dat.
Supported regions:
🇪🇺 EU
🇯🇵 JP
🇺🇸 US
This means the same ELF payload can be used regardless of which supported regional YouTube PKG you have installed.
Usage
The expected USB layout is:
USB Root/
├── download0.dat
└── y2jb-upload.elf

Load y2jb-upload.elf on the console and select Flash y2jb.
Credits
Relapse Autoloader — modified download0.dat
itsplk — latest download0.dat
Y2JB-Upload — ELF payload and automatic region detection
Disclaimer
Use this software at your own risk. Make sure you have the appropriate YouTube package installed before attempting to flash the modified download0.dat.
