# Pinecil BLE web interface (dark mode)

Bluetooth web client for Pinecil V2 - Utilizes [web-bluetooth](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API)

* Live demo: https://pips801.github.io/pinecil/ <- click to launch.
* Wiki: https://github.com/joric/pinecil/wiki



![Pinecil web ui](/pinecil_web.png)

## Compatibility
- Windows: try latest Chrome (does not work on Firefox)
- Android: try latest Chrome
- Linux: try Enabling “web-bluetooth*” flags in chrome://flags
- MacOS: try Bluefy browser (not guaranteed to work).

## Issues
- If your Pinecil is set to display the teperature as F instead of C, the webview will interpret F as C. Please Switch your Pinecil display temp to C until this is fixed.
- Webpage does not send keep-awake to the computer while connected. Your phone/laptop will go to sleep, even when fullscreen. 
