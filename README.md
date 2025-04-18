# bazzite-bluetooth-ds4-ds5-workaround

## Description
Workaround for https://github.com/ValveSoftware/steam-for-linux/issues/8678  
  
This script monitors connected PS4 and PS5 gamepad devices and disconnects  
the Bluetooth connection if specific button combinations are detected (Home and Triangle buttons).  
The script handles background processes for each device and maintains a record of process IDs  
to ensure proper cleanup of processes associated with devices that are no longer present.

## Usage

  ```bash
  [sudo] ./bazzite-bluetooth-ds4-ds5-workaround [-d] [--install] [--uninstall]
  -d: Enable debug mode
  --install: Install and enable the systemd service
  --uninstall: Uninstall the systemd service
