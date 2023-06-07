# dewocomputer
Boot to Recovery

Open Terminal and enable the root user and give it a password:

Enter the command below and press Enter

dscl -f /Volumes/Macintosh\ HD\ -\ Data/private/var/db/dslocal/nodes/Default localhost -passwd /Local/Default/Users/root

There might be a slight directory difference between Intel/Silicon. If the command above does not work try using one of these variations:

 /Volumes/Macintosh\ HD\ -\ Data/ or /Volumes/Data/ 

Enter a new password for root user. Note * If you choose a simple password be aware that the root user will be available as a user that can log into macOS which could present a risk to the security of the device.

Once complete click the Apple logo -> Reboot or in Terminal type Reboot then press Enter and let macOS start-up.

Show the hidden menubar and go to System Settings when the Setup Assistant begins by pressing Command + Option + Control + T together.

Click the Apple logo > System Settings -> Users & Groups

Create an admin user with your username and password then click Add Account. The authentication window will appear and autofill the username as user "System Setup". Change this to "root" and use the password you created earlier in Terminal.

Use the Apple menu and select Reboot and if this does not work, force off your Mac by holding the power button down at least 10 seconds.

Boot to Recovery again.

Open Terminal and enter the command below and press Enter.

touch /Volumes/Macintosh\ HD\ -\ Data/private/var/db/.AppleSetupDone

Then type Reboot and press Enter or force off your Mac again using the steps above.
