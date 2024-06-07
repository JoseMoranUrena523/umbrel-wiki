> [!NOTE]
> Booting from NVMe or USB instead of a microSD card is only supported on Raspberry Pi 5 for umbrelOS 1.2.0 and later. Raspberry Pi 4 is not supported.

umbrelOS 1.2.0 and later supports booting umbrelOS from NVMe or USB on Raspberry Pi 5. This allows you to run umbrelOS without a microSD card.

The steps to install umbrelOS in this configuration are similar to [installing umbrelOS from a microSD card](https://umbrel.com/umbrelos#install), with the exception that you need to flash the umbrelOS image to an NVMe drive or USB drive instead of a microSD card, and you may need to update the bootloader firmware on your Raspberry Pi 5.

## What you will need
- Raspberry Pi 5
- Either an NVMe drive + hat or USB drive (depending on your preference)
- Official Raspberry Pi power supply
- Ethernet cable

## Steps
> [!NOTE]
> If you have an early Raspberry Pi 5 model, you may need to update the bootloader firmware in order to be able to boot from NVMe. If this is the case, please follow the official Raspberry Pi documentation on how to update the bootloader firmware: https://www.raspberrypi.com/documentation/computers/raspberry-pi.html#bootloader_update_stable

1. Download the latest [umbrelOS image](https://download.umbrel.com/release/1.2.0-beta.1/umbrelos-pi5.img.zip) for Rasberry Pi 5.

2. Download [Balena Etcher](https://etcher.balena.io/) on your computer. It is required to flash the umbrelOS image that you downloaded in the previous step to your NVMe or USB drive.

3. Attach your NVMe drive or USB drive to your computer. For the NVMe drive, you will need to use a USB adapter to connect it to your computer.

4. Flash the umbrelOS image to your NVMe drive or USB drive using Balena Etcher. Once the flashing process is complete, safely eject the drive from your computer.

5. Attach the NVMe drive or USB drive to your Raspberry Pi 5.

6. Connect your Raspberry Pi 5 to your network using an Ethernet cable.

7. Power on your Raspberry Pi 5 using the official Raspberry Pi power supply.

8. And that's it! Wait for a few minutes for umbrelOS to boot up. You can access umbrelOS by navigating to http://umbrel.local on any device connected to the same network.

> [!WARNING]
> The boot order on your Raspberry Pi 5 is set to boot from a microSD card preferentially before booting from NVMe or USB. Make sure that you do not have a bootable microSD card inserted when booting from NVMe or USB. If you have a microSD card inserted, the Raspberry Pi 5 will boot from the microSD card instead of the NVMe or USB drive.