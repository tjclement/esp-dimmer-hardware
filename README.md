# $5 ESP8266 WiFi LED Dimmer
Custom hardware designs for a super tiny WiFi LED dimmer module based on the ESP8266, to control your lights from any device. __Doesn't need any arduinos or raspberries to work, just the ESP__. If you like this, please give it a star!

__Update:__ The new module design for RGB (i.e. triple channel) LEDs is done. This new design can handle up to ~8.5A of current per channel! Its parts costs the same as the old design, and if you want only one channel, you could just not solder the 2nd and 3rd channel. This way you can use the beefed up design. :)

<p align="center">
<img width="40%" src="https://github.com/tjclement/esp-dimmer-hardware/blob/master/images/front.png" />
<img width="40%" src="https://github.com/tjclement/esp-dimmer-hardware/blob/master/images/back.png" />
</p>
<p align="center">
<img width="40%" src="https://github.com/tjclement/esp-dimmer-hardware/blob/master/images/first_preview.JPG" />
</p>

# Ordering the board
Choose whether you want a single or triple channel dimmer, and then send all files in [single_channel or triple_channel]/gerber_files/ to your PCB house, and all should be fine and dandy!

# Parts
After having ordered the print board, you're going to want to have these parts for every module (mind you, there's two panelized modules per board ordered!):
<table>
  <tr>
    <td colspan="2"><strong>Single Channel (old version)</strong></td>
    <td colspan="2"><strong>Triple Channel (new version)</strong></td>
  </tr>
  <tr>
    <td>Amount</td>
    <td>Description</td>
    <td>Amount</td>
    <td>Description</td>
  </tr>
  <tr>
    <td>1</td>
    <td>ESP8266, ESP-12(E) format</td>
    <td>1</td>
    <td>ESP8266, ESP-12(E) format</td>
  </tr>
  <tr>
    <td>1</td>
    <td>XM1584 Power converter (set to 3.3v!)</td>
    <td>1</td>
    <td>MP2307 MINI 360 Power converter (3.3v!)</td>
  </tr>
  <tr>
    <td>1</td>
    <td>FDS8896 PowerTrench MOSFET</td>
    <td>3</td>
    <td>FDS8896 PowerTrench MOSFET</td>
  </tr>
  <tr>
    <td>2</td>
    <td>KF350-2P screw terminal blocks</td>
    <td>4</td>
    <td>KF350-2P screw terminal blocks</td>
  </tr>
  <tr>
    <td>4</td>
    <td>10k resistors, 0603 format</td>
    <td>6</td>
    <td>10k resistors, 0603 format</td>
  </tr>
</table>

__Total cost: less than $5!__

I order most of it from China, sites like aliexpress.com will have everything you need.

# Firmware
Because this module is essentially a breakout for the ESP8266, you can use any firmware written for it.
I've written a bunch of cool things to get this module running as I want it to, check it out here: http://github.com/tjclement/esp-dimmer-software.

Just hook up a 12V power supply, connect it and the LED strip to the module, and the ESP will be able to control the LEDs. Awesome!

If you're looking for something else (or write your own firmware), have a look at http://esp8266.com for more resources.

You can use a loader like this one to load firmware onto the ESP: https://github.com/themadinventor/esptool.

# Modifying
You can open the .sch and .brd files in Eagle (V7.2+), and make any modifications you see fit. If you add something cool, please create a pull request so we can bring the awesomeness into the community!

# Credits
Heavily inspired by Quindor's original design over at http://blog.quindorian.org/2014/12/esp8266-wifi-led-dimmer-part-1-of-x.html/. We've been sharing design ideas back and forth ever since. Nice job mate!
