# re_install_ubuntu
If you want to reinstall Ubuntu 18.04.xx when you have Ubuntu 18.04 and Windows 10 installed!

Note: This procesure is ok even if you do not have Windows 10 installed (single boot). I wrote my PC info here at the time of doing the following steps just for my own reference.

## Pc Info
Name: Dell Alienware
CPU:  Intel Core i7 @ 2.6 GHz
GPU:  Geforce RTX 2070
OS type: 64-bit
Disk: 1Tb SSD

## Target:
Current: Have both Ubuntu 18.04.4 LTS and Windows 10 installed, but Ubuntu is not working well.
Target:  Re-install Ubuntu 18.04.4 LTS alongside Windows 10

Note:    I want to have encrypted ubuntu install (for security). Don't worry, it's easy!

## Procedure
### Backup all the important things from your current PC if you can (Optional) e.g.:
1. Github Key
2. .bashrc, .bash_ros, .bash_history
3. Task, COMMANDS
4. List of all the additional pkgs in the ~/app, ~/home

### Make a live boot USB of "Ubuntu Desktop"
1. Download "Ubuntu 18.04.5 Image" --> 64-bit PC (AMD64) desktop image (https://releases.ubuntu.com/18.04.5/)
2. Create a bootable USB stick on Ubuntu using "Startup Disk Creator":
  - We’re going to use an application called ‘Startup Disk Creator’ to write the ISO image to your USB stick. This is installed by default on Ubuntu.
  - Insert your USB stick (select ‘Do nothing’ if prompted by Ubuntu)
  - On Ubuntu 18.04 and later, use the bottom left icon to open ‘Show Applications’
  - In older versions of Ubuntu, use the top left icon to open the dash
  - Use the search field to look for 'Startup Disk Creator'
  - Select Startup Disk Creator from the results to launch the application
  - ![01](images/01_bionic-search-apps.png)
  - When launched, Startup Disk Creator will look for the ISO files in your Downloads folder, as well as any attached USB storage it can write to. It’s likely that both your Ubuntu ISO and the correct USB device will have been detected and set as ‘Source disc image’ and ‘Disk to use’ in the application window. If not, use the ‘Other’ button to locate your ISO file and select the exact USB device you want to use from the list of devices. Click Make Startup Disk to start the process.
  - ![02](images/02_bionic-make-startup-disk.png)
  - Before making any permanent changes, you will be asked to confirm the USB device you’ve chosen is correct. This is important because any data currently stored on this device will be destroyed. After confirming, the write process will start and a progress bar appears.
  - ![03](images/03_bionic-usb-progress.png)
  - Installation complete. That’s it! You now have Ubuntu on a USB stick, bootable and ready to go.
  - ![04](images/04_bionic-usb-complete.png)

3. Run `python line_fit_video.py`.
4. 
