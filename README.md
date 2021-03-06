# The Deployatron

The Deployatron is a peripheral button used to map a physical action to live software deployments. 

The Deployatron has an 'arm' switch which turns on the system. A series of LEDs will go from red to green assuming some conditions are met (which will be specified by the user such as if the latest version of the software is on test, for example). When armed, pressing the 'big red button' will trigger the deploy. 

The Deployatron is an exploration into the process of releasing software and is designed to create an event rather than just clicking a button on a web page etc. It is built from an Arduino Uno, physical button and switch and feedback is through a small speaker and LED lights.

#The Code

The code runs on an Arduino Uno and uses the [Adafruit NeoPixel library](https://github.com/adafruit/Adafruit_NeoPixel).

The pins are mapped to:

ID | description | Arduino pin
--- | --- | ---
SPEAKER_PIN | piezo sounder | 2
ARM_SWITCH_PIN | switch | 4
DEPLOY_BUTTON_PIN | big red button | 3
PIXELS_PIN | pixels data pin | 6
