### Installing Shizuku for permanent on-device rootless system privileges and ADB access

1. In Settings app > Security, disable Secure App Spawning
2. Reboot phone
2. Install the Shizuku app from: https://apt.izzysoft.de/fdroid/index/apk/moe.shizuku.privileged.api
2. Enabled Developer options in the Settings app by tapping About Phone, scroll to the bottom, then tap Build Number seven times
3. (Recommended option is to start Shizuku using wireless debugging by...)
4. Connect to a trusted Wifi network
5. In Settings app > System > Developer settings, enable USB Debugging, then enable Wireless Debugging, and accept the wifi network as trusted.
6. Open the Shizuku app and follow instructions for Wireless ADB pairing
7. Once paired, press Start in the Shizuku app
8. Once Shizuku has successfully started, you can disable Wireless Debugging and disconnect from Wifi. 
9. **Do not disable USB Debugging. If USB Debugging is disabled, or if the phone is rebooted, Shizuku must be restarted by repeating Steps #4, #5, #7, and #8.**
