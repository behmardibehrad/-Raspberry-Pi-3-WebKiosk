## Installing Raspbian Lite and XFCE on Raspberry-Pi-3 

#### 1. Download Raspbian Lite:
	- https://www.raspberrypi.org/downloads/raspbian/
###

#### 2. Download Etcher:
	- https://etcher.io/
###

#### 3. Fromat the SD card and burn Raspbian Lite on SD using Etcher.

###

#### 4. Insert the SD into Raspberry Pi, and Boot up.

###

#### 5. Log in using default credintials:
	- The username is pi and the password is raspberry.
###

#### 6. Initial configuration:
	- Expanding the file system so Raspbian takes full use of SD:
		- sudo raspi-config (From the config tool menu select option #7).
		- Select option #A1 (Expand Filesystem).
		- Back to main menu, select Finish.
		- From pop up message for reboot, select yes.
	- Installing updates and upgrades:
		- sudo apt-get update
		- sudo apt-get upgrade
		- sudo apt-get dist-upgrade
		- sudo apt-get clean
	- 