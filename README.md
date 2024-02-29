# Andorid Virtual Camera
This app use the hook technology to replace the images captured by the system camera with video files, 
and support screenshot recording and video chat where the camera is used.
[video](https://xnxj.xyz)


## Prerequisite
1. You need to have a rooted with magisk android 10 or android 11 phone
2. It does not support emulators, cloud phones, virtual machines,vmos


## Support RTMP with OBS
1. Refer to this [tutorial](https://obsproject.com/forum/resources/how-to-set-up-your-own-private-rtmfp-server-using-monaserver.153/) and install the RTMP server on your PC.  <br>
2. Configure OBS with the properties below :
```
Streaming Service: Custom
Server: rtmp://127.0.0.1/live
Play Path/Stream Key: test
```
3. If the mobile phone and computer are  on the same network.<br/>Open floating window and type RTMP url in mobile phone
```
rtmp://<your pc ip>/live/test
```

If the mobile phone and computer are not on the same network，You can use adb streaming
### RTMP with USB cable transmission

1. Download [android platform tools](https://developer.android.com/tools/releases/platform-tools) and unzip to c:\adb
2. Open developer options on your phone and turn on USB debugging
3. Connect the phone to the computer via usb cable.<br/>
*When connecting to the computer for the first time, a dialog box will pop up asking if USB debugging is allowed.please allow it.*
4. In the c:\adb directory, open the command line and enter the following command
```
adb reverse tcp:1935 tcp:1935
```
5. Open floating window and type rtmp://127.0.0.1/live/test


## Download 
Please send mail with subject "virtual camera install apk" to mp4vcam@gmail.com to get the installation package.


