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
	- Chaging the default local settings:
		- sudo raspi-config (From the config tool menu select option #4).
		- select option 1 (change local).
		- change the default (en_GB.UTF-8 UTF8) to (en.US.UTF-8 UTF8) and select ok.
		- pop up message for system environment select (en.US.UTF-8 UTF8).
		- on main menu select finish.
		- sudo reboot
	- Configuring timezone:
		- sudo raspi-config (From the config tool menu select option #4).
		- select option 2 (change Timezone).
		- select your timezone.
		- select ok, and finish on main menu.
###

#### 7. Installing XFCE on Raspbian:
	- Installing Xorg Display Server:
		- sudo apt-get install --no-install-recommends xserver-xorg
		- sudo apt-get install --no-install-recommends xinit
		- xinit is needed to launch xorg using scripts or terminal.
	- Installing XFCE Gui:
		- sudo apt-get install xfce4
		- sudo apt-get install xfce4-terminal
	- Start the XFCE:
		- startx
###

#### 8. Everytime pi boots, it automatically uses terminal, for using GUI:
	- Installing LightDM login manager:
		- sudo apt-get install lightdm
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	