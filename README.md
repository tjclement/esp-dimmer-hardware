# ESP8266 WiFi LED Dimmer
Custom hardware designs for a super tiny WiFi LED dimmer module based on the ESP8266, to control your lights from any device. If you like this, please give it a star!

# Order
Send all files in /gerber_files/5x5/ to your PCB house, and all should be fine and dandy!

# Put it together!
After having ordered the print board, you're going to want to have these parts for every module (mind you, there's two panelized modules per board ordered!):
- 1x ESP8266, ESP-12 format
- 1x XM1584 Power converter (set to 3.3v!)
- 1x FDS8896 PowerTrench MOSFET
- 2x KF350-2P screw terminal blocks
- 4x 10k resistors, 0603 format

I order most of it from China, sites like aliexpress.com will have them all.

# Having fun
Because this module is essentially a breakout for the ESP8266, you can use any firmware written for it.
I've written a bunch of cool things to get this module running as I want it to, check it out here: http://github.com/tjclement/esp-dimmer-software.
If you're looking for something else (or write your own firmware), have a look at http://esp8266.com for more resources.

# Modifying
You can open the .sch and .brd files in Eagle (V7.2+), and make any modifications you see fit. If you add something cool, please create a pull request so we can bring the awesomeness into$

