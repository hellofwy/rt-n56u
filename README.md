### Newifi mini custom firmware using padavan/rt-n56u ###

*Use at your own risk.*
I don't have solid knowledge about routers, so there may be errors in my changes. 

This project is forked from padavan/rt-n56u, and the `newifi_mini` branch is created for Newifi mini router. Only Newifi mini'specific board settings are added, nothing more.

GPIO settings of LED, USB and RESET are from [hiboyhiboyhiboy's firmware](www.right.com.cn/forum/thread-161324-1-1.html)  which also based on padavan's firmware.

### How to compile ###
After compiled the tool chains following the [HowToMakeFirmware's](https://bitbucket.org/padavan/rt-n56u/wiki/EN/HowToMakeFirmware) instructions, compile the firmware for newifi mini with:

```
cd /opt/rt-n56u/trunk
cp configs/templates/newifi_mini.config .config
./clear_tree
./build_firmware
```
The firmware will be in the `images` folder.
You can customize the components of firmware by editing the `newifi_mini.config`.


--------------------The original README is below:--------------------

# README #

Welcome to the rt-n56u project

This project aims to improve the rt-n56u and other supported devices on the software part, allowing power user to take full control over their hardware.
This project was created in hope to be useful, but comes without warranty or support. Installing it will probably void your warranty. 
Contributors of this project are not responsible for what happens next.

### How do I get set up? ###

* [Get the tools to build the system](https://bitbucket.org/padavan/rt-n56u/wiki/EN/HowToMakeFirmware) or [Download pre-built system image](https://bitbucket.org/padavan/rt-n56u/downloads)
* Feed the device with the system image file (Follow instructions of updating your current system)
* Perform factory reset
* Open web browser on http://my.router to configure the services

### Contribution guidelines ###

* To be completed
