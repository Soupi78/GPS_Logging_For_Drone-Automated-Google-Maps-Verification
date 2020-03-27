# GPS_Logging_For_Drone-Automated-Google-Maps-Verification
This is my midterm project for ECE 387 at Miami University. 

In brief, this midterm was aimed to provide GPS loging capabilities for a drone by mounting an Arduino directly to it during flight. Then after a flight the user can unmount their SD from the Arduino and run my Python code to autmatically pull up the Drone's logged location on google maps to check where it went. Images of the hardware setup can be found here: http://imgur.com/a/RzmR9   

This project requires using the Arduino Uno, the Adafruit Ultimate GPS Logger Pro, a MicroSD and an external powersource for the Arduino. 
A detailed setup and explanation of the Adafruit Ultimate GPS Logger Pro can be found at: https://learn.adafruit.com/adafruit-ultimate-gps-logger-shield.  Additionally I've provided explanatory comments in both the Arduino and Python codes. Please note Shield_SDlog.in is an example code from the Adafruit standard GPS library, my code _387_gps_project.in_ is a mild modification of this code to better sync with my Python code and specefic needs, I have provided both as reference. 

Once initial soldering is completed and direct and serial connection have both been estblashed, you should be able to open the Arduino code provided (_387_gps_project.in_ not Shield_SDlog.in) and upload it to your board. At this point you can mount your Arduino and Shield to your drone for flight. Make sure your sure you've inserted your SD and checked the charge of your battery source to ensure getting valid data onto your SD. Also, ensure you've attahced your board to a place your drone can support the weight of the board, in my case I unmounted the camera from my DJI Phantom 3 Pro so the arduino was directly in the center of the drone and out of contact with any of the propellers.   

Once flight is completed, insert the SD into your computer. You should now be able to simply run the python code provided and have it automatically open a google map of the first logged location of the drone. If you run into issue with the python check your Chromedriver path. Provided is the Selenium driver for Google Chrome however this assumes you already have the base Selenium driver instaled on your machine as well as Google Chrome. In addition to having the library installed, you must also ensure that the python code is pointing to the correct loaction for this driver on your machine as my code is setup for my specefic library hierarchy. 

Provided you've done everything above you should now have both a log of your flight locations as well as a method to validate that data using Google Maps. 

THIS IS A TEST TO SEE HOW OCTOBOT SHOWS CHANGED FILES
