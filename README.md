# Pinecil BLE web interface

Bluetooth web client for Pinecil V2 - Utilizes [web-bluetooth](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API)

* Live demo: https://joric.github.io/pinecil/ <- click to launch.
* Wiki: https://github.com/joric/pinecil/wiki



![Pinecil web ui](/pinecil_web.png)

## How to use

* Download [Pinecilv2_EN.bin](https://github.com/joric/IronOS/releases/latest/download/Pinecilv2_EN.bin) (this is the latest [IronOS BLE](https://github.com/ralim/IronOS/tree/BLE) binary hosted in my repository)
* Download Blisp flasher binaries: [Windows](https://github.com/joric/blisp/releases/latest/download/blisp-win64.zip), [Linux](https://github.com/joric/blisp/releases/latest/download/blisp-linux.tgz) (also latest hosted locally, original repo is [here](https://github.com/pine64/blisp))
* Hold "-" button, connect to USB; flash firmware with `blisp write -c bl70x --reset Pinecilv2_EN.bin`.
* Open https://joric.github.io/pinecil press connect button, choose "Pinecil"
* You can also save and open the page locally, it's a single page with no dependencies

Video:

[![](http://img.youtube.com/vi/damRcWwXpbA/hqdefault.jpg)](https://youtu.be/damRcWwXpbA)



## Compatibility
- Windows: try latest Chrome (does not work on Firefox)
- Android: try latest Chrome
- Linux: try Enabling “web-bluetooth*” flags in chrome://flags
- MacOS: try Bluefy browser (not guaranteed to work).

## Troubleshooting
* If it doesn't show up in the browser explorer - check device name, unpair/disconnect it from elsewhere.
* See https://wiki.pine64.org/wiki/Pinecil#Firmware for other firmware (BLE branch should be compatible).
* To roll back changes, flash stock [pinecilv2-release-2.18.zip](https://github.com/joric/IronOS/releases/download/v2.18/pinecilv2-release-2.18.zip) or [dev-2.20](https://github.com/joric/IronOS/releases/tag/dev-1444f9).

## Issues
- If your Pinecil is set to display the teperature as F instead of C, the webview will interpret F as C. Please Switch your Pinecil display temp to C until this is fixed.
- Webpage does not send keep-awake to the computer while connected. Your phone/laptop will go to sleep, even when fullscreen. 

## References

* https://wiki.pine64.org/wiki/Pinecil Pine64 official wiki (check out Development Projects section)
* https://github.com/NordicSemiconductor/bluetooth-numbers-database Nordic BLE database, may be useful
* https://ralim.github.io/IronOS/ official IronOS repository (usually in sync so you can try releases from there)
* https://pine64.com/product/pinecil-smart-mini-portable-soldering-iron/ Buy Pinecil V2 here
* https://github.com/Ralim/IronOS/discussions/1257 all Aliexpress's pinecils are conterfeit/not V2
* https://pinecil.pine64.org/ Pinecil V2 authenticity checker
* https://www.jbctools.com/jbcsoftware.html BLE-enabled JBC b-Iron (direct links to APK/iOS software)
