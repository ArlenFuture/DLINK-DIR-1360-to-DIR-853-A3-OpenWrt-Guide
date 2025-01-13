# DIR-1360 A1 to DIR-853 A3 OpenWrt Unofficial Installation Guide  

## Introduction  
This guide is specifically for D-Link DIR-1360 A1 users, showing you how to flash it into a DIR-853 A3. These two devices share the same PCB design. After the process, your router will function as a DIR-853 A3 and support OpenWrt firmware upgrades for enhanced functionality!  

## Installation Steps  

### 1. Enter Recovery Mode  
1. Ensure the router is powered on.  
2. Press and hold the **RESET button** on the back of the router until the orange LED starts blinking.  

### 2. Flash the Modified Firmware via D-Link Recovery GUI  
1. Open a browser and navigate to the D-Link Recovery GUI (commonly `192.168.0.1`).  
2. Download the **DIR-853 A3 firmware** with a modified header provided by Lucky1:  
   [Firmware Download Link](https://forum.openwrt.org/t/adding-openwrt-support-for-dir-1360/98590/33)  
3. Upload the firmware to the Recovery GUI and wait for the flashing process to complete.  

### 3. Future Firmware Upgrades  
1. Once the flashing process is complete, the device will operate as a DIR-853 A3.  
2. You can download and upgrade future firmware directly from OpenWrt for DIR-853 A3:  
   [DIR-853 A3 OpenWrt Firmware Download](https://openwrt.org/toh/hwdata/d-link/d-link_dir-853_a3)  

## Test Results  
Based on tests with OpenWrt 23.05.5:  
- **Wireless Network**: Needs to be restarted after setup to work correctly.  
- **2.4G Wi-Fi**: Persistent issues, may not work stably.  
- **5G Wi-Fi**: Works normally and stably.  

## Notes  
- This guide involves unofficial operations. Flashing firmware carries risks—proceed at your own discretion.  
- It is strongly recommended to back up your router settings before flashing to prevent data loss.  

## References  
- [DIR-1360 and DIR-853 A3 PCB Details](https://forum.dd-wrt.com/phpBB2/viewtopic.php?t=321874&sid=140829221456a3b23eae63c231ac58d9)  
- [Lucky1 Modified Firmware Discussion Thread](https://forum.openwrt.org/t/adding-openwrt-support-for-dir-1360/98590/33)  
- [DIR-853 A3 OpenWrt Official Info](https://openwrt.org/toh/hwdata/d-link/d-link_dir-853_a3)  

## Contribution  
Found an issue or have suggestions? Feel free to submit them via Issues or Pull Requests to improve this guide!  

## License  
This project is licensed under the MIT License. For more details, refer to the [LICENSE](LICENSE).  
