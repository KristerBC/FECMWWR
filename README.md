# FECMWWR - Firmware for ESP82xx Controllers using MQTT, WIFI and Wireless remotes

### Description
This is a lightweight firmware that can be used on devices containing a ESP82xx chip such as the Arilux LCxx series.

### Functionalities on first release(November 4th 2018)
 - Programmable Single Button RF remote actions when you click the remote in using a pattern
 - Programmable Multi Button RF remote actions
 - MQTT
 - WIFI
 - OTA(Over-The-Air Programming)
 
### Functionalities in future releases
 - Hotspot with DHCP server in case the home WIFI is down
 - Lightweight grid between each devices
 - Scheduled state changes
 - Linking the state of multipe devices - assuring the multiple devices are always in the same state
 
### How to install
This repository contains an entire PlatformIO project. In short, find a flash guide in the [The Tasmota Firmware](https://github.com/arendst/Sonoff-Tasmota "Repository of the Tasmmota Firmware") repository for your device, and upload the firmware in the same way that you upload a Tasmota firmware.
If you are still lost(which is plausible do to the lacking install guide), please feel free to contact me.
 
### Why yet another ESP firmware?
Even though I am a big fan of [The Tasmota Firmware](https://github.com/arendst/Sonoff-Tasmota "Repository of the Tasmmota Firmware"), I find it too heavy for some applications. Do to the many functionalities, RF reception and function button usage is rather slow and sometimes unresponsive.
The goal with this new firmware, is to be able to use your device without having to rely on an secondary server, your home WIFI or other things which can make your entire home automation unresponsive. Each device should be able to work independantly and even a person with no technical knownledge should be able to control the devices, once they a installed.
That said, I suggest that you take a look on [The Tasmota Firmware](https://github.com/arendst/Sonoff-Tasmota "Repository of the Tasmmota Firmware") in order to make your own decision. I still use Tasmota to some applications, because of all the features it has. 

### Can I participate somehow?
Everybody are welcome to participate in this project. If you have a script you will like to include in a future realease, please make sure that it is modular, performant, cleanly coded and deactivatable from the config file.
Please feel free to contact me for any questions.
 
#### Dictionary
 State changes - When one of the pins in the device change state(ex. when changing colors)
