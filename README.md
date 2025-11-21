# List of Android phones and their USB tethering protocols

| Phone                                               | Android version | Protocol |
| --------------------------------------------------- | --------------- | -------- |
| Google Pixel 6 and newer                            | Android 12+     | CDC NCM  |
| Samsung Galaxy A16                                  | Android 15      | RNDIS    |
| Samsung Galaxy S22 FE 5G                            | Android 16      | RNDIS    |
| Samsung Galaxy S25                                  | Android 15      | RNDIS    |
| Samsung Galaxy S25 FE                               | Android 16      | RNDIS    |
| Xiaomi Redmi Note 13                                | Android 14      | RNDIS    |

## Help with expanding this list
You can help expand this list! :)  
To check which tethering protocol your phone supports, connect it to your computer and enable USB tethering.

### Windows
You can check the network adapter name in **Device Manager**, **Task Manager**, or by searching for **View network connections** in the Start menu. The tethering protocol used by your device will typically be visible in the network adapter’s name (e.g., "Remote NDIS" or "CDC NCM").
### macOS
*macOS supports only CDC NCM tethering.*  
To check, open **System Settings -> Network**
- If your phone appears in the network list, it supports **CDC NCM**
- If your phone doesn’t appear, it supports **RNDIS**

### Linux
Todo; alternatively check **adb** section if you're using Linux

### adb
```adb shell svc usb getFunctions```
