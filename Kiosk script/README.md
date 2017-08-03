## Kiosk Script and start up options

#### 1. Install firefox as web-browser:
	- sudo apt-get install firefox-esr
###

#### 2. Install R-Kiosk adds-on on firefox.
	- restart firefox and make sure R-Kiosk in enabled.
###

#### 3. Create a simple script to open firefox:
	- #!bin/bash
	- firefox http://example.com
	- exit 0
###

#### 4. Make the script executable:
	- sudo chmod +x script-name
	- test the script:
		- sh script-name
###

#### 5. Options to run the script on start up:
	- Simply add the executing command to start up
	- Create an Alias for the script and call the Alias in rc.locals
	- Create an Alias for the script and call the Alias in init.d/rc.local
