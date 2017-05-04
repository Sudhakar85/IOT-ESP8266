The purpose of the project to create Webserver  for IOT using ESP8266 Wemos D1 board.

You need below things to get started

1. Arduino IDE
2. ESP8266 Wemos D1 Board . </br>
http://www.ebay.com/itm/172579194166?_trksid=p2057872.m2749.l2649&var=471417281616&ssPageName=STRK%3AMEBIDX%3AIT

![ESP8266](/Images/ESP8266_Wemos_D1.jpg?raw=true "ESP8266")

3. Micro USB Cable

# Arduino IDE

1. Download and install arduino IDE version 1.8.2 from below link </br>
   https://www.arduino.cc/en/Main/Software.

# Install library for ESP8266

Once the IDE installed, the additional ESP8266 library has to be installed to program the chip

1. Create new folder name called "Portable" in Arduino installed directory which has lib and Bin like below
This steps solves some of the compilation issues in the ESP8266 library

![Portable](/Images/ArduinoDirectory.jpg?raw=true "Portable")

2. Open File-> Preferences and Enter the below package link <br>
http://arduino.esp8266.com/stable/package_esp8266com_index.json

![Preference](/Images/Preference.jpg?raw=true "Preference")

3. Now download and install the ESP8266 board

Choose Tools -> Board -> Board Manager and then select ESP8266 library like the last one in the screen shot and click install.
This will download around 150MB file and install. Once the installation is completed then close the the Arduino IDE and reopen.

![Board Manager](/Images/BoardManager.jpg?raw=true "Board Manager")

3. Now choose Tools - Board -> ESP8266 D1 or Wemos D1 ( Retaired ) to set the current board for programming


# Program ESP8266

1. Install the driver for the USB drive CH340 USB to UART driver from below link <br>

https://www.wemos.cc/downloads

2. Connect ESP8266 board to the computer with Micro USB

3. Go to device manager in your computer and check the detected new device and the Port number. You can see the blue LED lights up in ESP8266

4. Open the Arduino IDE and set the Port number using Tools -> Port Menu

5. Create new program by choosing File -> New and Copy the code from WIFISetup.ino from this repository to your program

6. Modify the below line to include your WIFI SSID and Password

		const char* ssid = "sudhakar"; <br>
		const char* password = "xxxxx";

7. Choose Sketch -> upload to upload the file to your ESP8266

8. Once uploaded, choose Tools -> Serial Monitor to see all the serial print message in the board. </B>
	You can also see connected IP Address of the Server

9. Open the browser and enter the ip address to see the Hello World Message

10. All the best and let me know if you have any questions.... 


# References

	https://www.wemos.cc/product/d1.html
	


