# RPiThermalPrinter
<h3>Project Overview</h3>
<p>Using a thermal printer with a raspberry pi to print images taken with an attached logitech webcam.</p>

---

<h3>Installing the Printer Libraries</h3>
These steps are for the tiny thermal printer from Adafruit(Which I'd like to add was a rip off. Just buy from China - Model: DP-EH400).  
1. Start the pi - Assuming Raspberry Pi has been already been setup with Raspbian (Wheezy or Jessie).  
2. The tiny thermal printer has the option to use USB so that's what I used. Plug in the USB to the printer and a port on the pi.  
3. **Important:** Plug in the ground and 5V (red and black wires to the GPIO Header **first**.  For RPi2 the pin numbers were 2 and 6.  **Then** plug it into the printer, this way there is less chance to accidentally plug in the wrong pins on the pi and blow something up.  
4. Cool, now open the terminal and type `echo -e "Testing my cool printer." > /dev/ttyUSB0` to print a test. You might have to click the button to feed the paper to see if it printed.  

If it doesn't work:

+ check connections to power on RPi. If it is getting power there will be an LED indicating that it's being powered.</li>
+ check if there is thermal paper in the printer.</li>
+ google the problem because I don't know what else could go wrong.

If it worked: 

We get to install some stuff!
