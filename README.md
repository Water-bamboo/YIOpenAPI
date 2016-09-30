# YI Open API
YI Open API provides a set of APIs in the form of SDKs of different languages for software developers and hardware makers to build cool apps and products with YI 4K Action Camera. 

This repository contains the libraries, samples and documentation for using the APIs.

The following is the tree structure of this repository:

* /bin -- firmware and config file for VR/360
* /sdk -- SDKs of different languages
* /sdk/java -- YI Open API Java SDK
* /sdk/java/doc -- documentation
* /sdk/java/libs -- SDK library for building your applications
* /sdk/java/samples -- samples demonstrating the use of SDK APIs
* /specs -- reference specs

## Features

The APIs currently provide support to the following 4 areas

- camera control (start/stop recording video, capture photo, turn on/off viewfinder, etc)
- camera settings (datetime, video resolution, photo size, video standard, etc)
- camera state (record started/completed, video finder started etc)
- media management (browse files stored on media, download, delete file)

## VR/360/multi-camera system

If you have a VR/360 rig or a multi-cameras system, you can have the cameras connected to a wi-fi network or a hotspot, and then control the cameras from your application (built using the YI Open API SDK), by following the steps below: 

1. update firmware (/bin/{country code}/firmware.bin)
   * copy firmware.bin onto a microSD card
   * start the camera with the microSD card
   * wait until the sound of starting music

2. setup config file (/bin/{country code}/sta.conf)
   * provide correct SSID and password for accessing the Wi-Fi network or the hotspot
   * give each camera a different device name
   * set the correct country code (e.g. CN for China, US for United States etc)
   * save the changes to sta.conf and copy it onto the microSD card
   * start the camera with the microSD card

3. turn on wifi on camera
   * go to camera settings -> Wi-Fi
   * pick the Wi-Fi frequency matching to the one broadcasting from your Wi-Fi network or hotspot
   * turn on Wi-Fi (note that the ON button is green)
    
4. tryout YI360Demo sample (/sdk/{java, swift}/samples/YI360Demo)
   * build and launch the sample app

## Join the YI Open API community

* Website: https://www.facebook.com/groups/YIOpenAPI/

## Signup for YI Open API email updates and news

* Website: http://www.yiopen.com/

## License

The YI Open API SDKs are licensed as described in LICENSE. To download and use YI Open API SDKs, you hearby agree YI Technologies, Inc. End User License Agreement (EULA) as described in EULA.
