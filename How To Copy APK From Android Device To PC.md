#Copy APK from device to PC then install to another device

- Use ADB to list all packages and save to a text file
  - `adb shell pm list packages -f > F:\Android\p.txt`
- Find the package you want in the list
  - `/data/app/com.partnersfirst.mobilebanking-1.apk`
- Copy the APK
  - `adb pull /data/app/com.partnersfirst.mobilebanking-1.apk F:\Android\` 
- Install on the new devie
  - `adb install <path_to_apk>`
