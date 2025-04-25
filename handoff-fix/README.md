# Handoff fix for Fenvi T919
For me Handoff didn't work right after installing macOS, so I needed to do some trickery to get it working. <br>
The fix was that macOS needs to generate a new Handoff key so your network card can communicate with your other devices and get data about what applications are open or what has been copied to the clipboard. <br>
To achieve this, you'll need to open the <i>Keychain Access</i> app, on the left hand side, select <i>'login'</i> and search for <i>'handoff-own-encryption-key'</i>, right click on it and click on delete.<br>
![](https://raw.githubusercontent.com/BenjaminStonawski/msi-b350m-pro-vd-plus-ryzen-7-5700x-hackintosh/refs/heads/main/screenshots/Screenshot_2024-03-11_at_AM_12.50.30.webp)
<br>At this popup, hit delete again.<br>
![](https://raw.githubusercontent.com/BenjaminStonawski/msi-b350m-pro-vd-plus-ryzen-7-5700x-hackintosh/refs/heads/main/screenshots/Screenshot_2024-03-11_at_AM_12.52.57.webp)
<br><i>Note: sometimes this popup window won't appear, if you experience the same issue, just try to relaunch the app or click "iCloud" on the left hand side and click on "login" again and try to search for the handoff-own-encryption-key and try to delete it again.</i><br><br>
After that, you'll need to sign out from Apple ID and reboot your system. <br> <i>Note: keep a copy of everything (like Calendar, etc.) if it's asked.</i><br>
## After reboot
After reboot, you just need to sign back in to your Apple ID, and Handoff should work now, if not, try restarting the system again.
