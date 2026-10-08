# Y2JB Relapse Autoloader

**Y2JB-Upload** is an ELF payload that allows you to replace YouTube's `download0.dat` with the modified **Relapse Autoloader**.

The payload automatically detects your installed YouTube region and replaces the appropriate file, so it works with **EU, JP, and US** versions of YouTube.

## Requirements

- A compatible console with payload/ELF loading support
- The appropriate YouTube PKG installed
- The latest modified `download0.dat` from **itsPLK**
- A USB drive
- `y2jb-upload.elf`

## Installation

1. Install the appropriate YouTube PKG on your console, if you haven't already.
2. Download the most recent modified `download0.dat` from **itsPLK**.
3. Place `download0.dat` on the **root of your USB drive**.
4. Place `y2jb-upload.elf` on the USB drive as well.
5. Connect the USB drive to your console.
6. Load `y2jb-upload.elf` using **AutoLoader** or manually through **Payload Manager**.
7. Select **`Flash y2jb`**.
8. The payload will automatically detect your YouTube region and install the appropriate version.

## Region Detection

You don't need to manually select your YouTube region.

**Y2JB-Upload automatically detects the installed YouTube version and selects the appropriate location for `download0.dat`.**

Supported regions:

- 🇪🇺 EU
- 🇯🇵 JP
- 🇺🇸 US

This means the same ELF payload can be used regardless of which supported regional YouTube PKG you have installed.

## Usage

The expected USB layout is:

```text
USB Root/
├── download0.dat
└── y2jb-upload.elf
```
Load y2jb-upload.elf on the console and select Flash y2jb.


##Credits
Gezine - creator of the original Y2JB
shahrilnet, null_ptr - Referenced many codes from Remote Lua Loader
BenNoxXD - ClosePlayer reference
ntfargo - Thanks for providing V8 CVEs and CTF writeups
abc and psfree team - Lapse implementation
matem6 - P2JB implementation
edisnord - Relapse implementation
flat_z and LM - Helping implement GPU rw using direct ioctl
john-tornblom and EchoStretch - Providing elfldr.elf payload
hammer-83 - Various BD-J PS5 exploit references
zecoxao, idlesauce, and TheFlow - Helping troubleshoot dlsym
Dr.Yenyen and PS5 R&D community - Testing Y2JB
Rush - Creating Y2JB backup file
Feyzee61 - download0.dat generator workflow
ufm42 - kexp used for PS5 post JB all-in-one shellcode
itsplk - ps5-y2jb-autoloader
