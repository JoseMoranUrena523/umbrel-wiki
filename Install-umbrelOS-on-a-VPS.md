> [!NOTE]
> You’ll be installing Umbrel 0.5.4, as most VPS providers do not support booting from an ISO. Please be aware that this version is now deprecated. We recommend using the latest version of [UmbrelOS](https://umbrel.com/umbrelos#install) to benefit from the most recent security updates and bug fixes.

## Minimum System Requirements

- **CPU:** Dual-core 64-bit Intel or AMD processor (Quad-core or higher recommended).
- **RAM:** 2GB (4GB+ recommended).
- **Storage:** 1GB+ (Storage requirements vary based on use case. For example, running a Bitcoin node typically requires 1TB or more, while file/media storage needs can be estimated based on your cloud services usage).
- **Operating System:** Debian or Ubuntu.

## How to Install

#### Step 1: Install Ubuntu or Debian onto your VPS
You can use any VPS provider, such as [Google Cloud](https://cloud.google.com/), [Microsoft Azure](https://azure.microsoft.com/), [Amazon Web Services](https://aws.amazon.com/), [DigitalOcean](https://digitalocean.com/), etc. Choose a VPS with the desired specifications.

#### Step 2: SSH into Your VPS
- Download an SSH client like [PuTTY](https://www.putty.org/) or [Termius](https://termius.com/), or use your computer's built-in terminal with the `ssh` command.
- **IF USING AN SSH CLIENT:** Enter the information provided by your VPS provider (IP address, username, password, SSH key, etc.) into the SSH client.
- **IF USING A BUILT-IN TERMINAL:** Use the `ssh` command to securely access your VPS. For password-based access, run `ssh user@ip` and enter your password when prompted. For SSH key-based access, run `ssh -i ~/.ssh/ssh_key_name user@ip`.

#### Step 3: Install UmbrelOS
- After your system boots up, run the following command:
```bash
curl -L https://raw.githubusercontent.com/getumbrel/umbrel/913ff567bd6a5136586f0040e80fc99ae310fba9/scripts/install | bash
```

#### Step 4: Finalize Installation
- Once the installation process is complete, visit [http://umbrel.local](http://umbrel.local) or your VPS IP address. Enter any username and password to complete the installation.

> [!TIP]  
> If you cannot access [http://umbrel.local](http://umbrel.local) and are using a Windows computer, try accessing [http://umbrel](http://umbrel). Alternatively, use your router's admin dashboard or a network scanning tool like 'Fing' to find your device's IP address on your local network. If necessary, you can connect a display and keyboard to your device, log in, and run `hostname -I` to find its IP address. Enter this IP address directly into a web browser to access UmbrelOS.

## Support

For support or to share your experience with others, join our [community forum](https://community.umbrel.com) and [Discord server](http://discord.gg/efNtFzqtdx).
