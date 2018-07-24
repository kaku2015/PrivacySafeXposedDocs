### Device Owner (Non ROOT) Mode Setup

### Notice:
- Due to limitations of the MIUI system such as Xiaomi, Hide App feature may be invalid. Please activate it with caution.
- The latest test version (354) of the Huawei EMUI system for non-intra-mobile push updates. After activating the ADB, there may be a problem that the mobile phone restarts and loses individual system apps. Please activate it with caution. If this problem occurs, uninstall the app and restart the phone to restore it.
- Please clear the lock screen password before Samsung S8+ Android8.0 is activated. After ADB is activated, it may cause the administrator to lock and inaccessible after booting, and may cause problems such as facial recognition unusable. Please activate it with caution.

### Setup steps:
1. Make sure your phone running Android  6.0+ and you know how to use [ADB](https://www.xda-developers.com/install-adb-windows-macos-linux/) clearly.
2. Go to "Settings > Accounts", remove **all accounts** including your Google account.
3. If multi-user or guest mode has been set on your device, also need to be closed or deleted.
4. Run ```adb shell dpm set-device-owner com.hld.anzenbokusuxposed/com.hld.anzenbokusu.receiver.DPMReceiver``` on your computer.
5. If you see the words Success, you can open the One Vision to use (may need to restart your phone) , then you can add your accounts and guest mode back.

### FAQ

- **Q: It shows "no devices/emulators found"**
- A: USB debugging is not turned on, or the USB is not connected properly.

- **Q: It shows "Not allowed to ... already several accounts on the device"**
- A: Please follow step 2 and remove ALL accounts. PS: Pulling out SIM card may be required for Xperia and ZUK devices.
</br>**Added: You can use the command ```adb shell pm list users``` view the accounts, use the command ```adb shell pm remove-user user id``` to delete the account.**

- **Q: It shows "Not allowed to ... already several users on the device"**
- A: Please follow step 3 and remove the guest mode or multi app/private mode.

- **Q: It shows "Trying to set the device owner, but device owner is already set"**
- A: You have set up other app using Device Owner mode, please cancel the settings of other app.

- **Q：After removing the account, you are prompted "Your administrator will not allow this change"**
- A：Please remove the fingerprint and lock screen password before removing the account.

- **Q: It shows "Sets the given component as active admin..."**
- A: Please reboot your phone.

- **Q: After all the above operation still shows "xxx"**
- A: Please reboot your phone.

- **Q: There is "Device is managed by your organization" on my notification center after setting up. Why?**
- A: That is how One Vision works.

- **Q: How to uninstall One Vision?**
- A: Just select "Uninstall" in the settings of One Vision.


