# Portable-Linux-Tails
Personal setup and operational notes for an amnesic security environment on a USB drive.

[**PT-BR**](./docs/README.pt-br.md)

## Dependencies
- [Tails OS](https://tails.net/install/download/index.en.html)

## Getting Started
<details>
  <summary>Starting Linux Tails</summary>

  - Plug in the USB drive and reboot your system.
  - Press **F12** (or your hardware-specific key) during boot to open the Boot Menu.
  - Select the **UEFI** partition from the USB drive.
  - On the `Welcome to Tails` screen, navigate to `Additional Settings` (+ icon) and set an **Administration Password** if root access (sudo) is required.
</details>

<details>
  <summary>Connect to the Tor network</summary>
  
  - In the `Tor Connection Assistant`, select the option **"Hide to my local network that I'm connecting to Tor"** for enhanced obfuscation.
  - [Request a bridge](https://bridges.torproject.org/options) and enter the credentials manually or via QR code.
  - Ensure the system time is synchronized with **UTC**. If the connection fails, you may need to adjust the **BIOS/Hardware Clock** to UTC to allow the Tor handshake.
</details>

## Security Recommendations
  - **Keep the OS Updated**: Always upgrade to the latest stable version as soon as it is available. Outdated versions may contain vulnerabilities or obsolete bridge protocols that compromise your security.
  - **No Persistent Storage**: Do not create a persistent partition. This ensures that no session data, downloaded files, or configurations are saved to the physical hardware, leaving zero trace after shutdown.
