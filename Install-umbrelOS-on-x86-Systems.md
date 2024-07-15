> [!NOTE]
> umbrelOS is specifically built for [Umbrel Home](https://umbrel.com/umbrel-home). Support for other devices is best-effort and not guaranteed. Compatibility issues may arise due to the differences in hardware, drivers, and such.

## Minimum System Requirements

- **CPU:** Dual-core 64-bit Intel or AMD processor. (Quad-core or higher recommended)
- **RAM:** 4GB. (8GB+ recommended)
- **Storage:** 32GB. (Storage needs depend on your use case. For instance, running a Bitcoin node typically requires 1TB or more, while file/media storage needs can be estimated based on your cloud services usage.)

## How to install

#### Step 1: Prepare a bootable USB stick
- Download the [latest umbrelOS USB installer](https://download.umbrel.com/1.2.1/umbrelos-amd64-usb-installer.iso) on your computer.
- Download and install [Balena Etcher](https://www.balena.io/etcher/) on your computer.
- Plug a USB stick (at least 4GB) into your computer. Ensure that it doesn't contain any important data as it will be formatted.
- Use Balena Etcher to flash the `umbrelos-amd64-usb-installer.iso` file to the USB stick.
![image](https://github.com/getumbrel/umbrel/assets/10330103/b67f31f5-95d0-4ad5-8945-76bf32b1b8e3)

#### Step 2: Boot from USB stick
- Remove the USB stick from your computer, and insert it into your device.
- Connect a display and keyboard to your device (for desktops or NUCs/Mini PCs). 
- Plug an Ethernet cable into your device and connect it to your internet router.
- Turn on the device. It should automatically boot from the USB stick.
> If your device doesn't automatically boot from the USB stick, you might need to change the boot priority order in its BIOS settings.

#### Step 3: Install umbrelOS on internal storage
- After the system boots up, it will present you with the following screen:
![umbrelos-usb-installer-3](https://github.com/getumbrel/umbrel/assets/10330103/e8c23d0e-230d-48e0-a77a-a1ffc2d5293c)
- Identify the correct internal storage device where you intend to install umbrelOS, and note its corresponding number. For instance, in the above screenshot, if we want to install it on the 'ATA' drive, which has a capacity of '238.5G', we'd type '1' (without the quotes) and press Enter.

#### Step 4: Finalize installation

- After the flashing process is complete, turn off the device by pressing any key.
- Remove the USB stick, keyboard, and display.

#### Step 5: Boot up!

- **Important:** Ensure that the USB stick is no longer connected to the device. Also, double-check that the Ethernet cable is connected between your device and the router.

- Turn on your device.

- The first boot will take ~5 minutes. After booting up, you can access umbrelOS by navigating to [http://umbrel.local](http://umbrel.local) on any device connected to the same network.

> [!NOTE]
> **Important**: If you have a display connected to your device, you might notice the `umbrel login` prompt in the terminal output. This prompt is for terminal access only. To use umbrelOS, there is no need to log in via the terminal. Instead, simply open [http://umbrel.local](http://umbrel.local) on any device that is connected to the same network to access the user interface.


> [!TIP]
> If you cannot access [http://umbrel.local](http://umbrel.local), and you are using a Windows computer, try accessing [http://umbrel](http://umbrel). Alternatively, use your router's admin dashboard or a network scanning tool like 'Fing' to find your device's IP address on your local network. If needed, you can connect a display and a keyboard to your device, log in, and run `hostname -I` to find its IP address. Then, enter this IP address directly into a web browser to access umbrelOS.

## Support

To get support or share your experience with others, please join our [community forum](https://community.umbrel.com) and [Discord server](http://discord.gg/efNtFzqtdx).