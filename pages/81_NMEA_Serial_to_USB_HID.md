# NMEA Serial to USB HID

There are several ways that this may be accomplished.  In Linux, there are simple commands (if you know what they are) to pipe all the serial data to the keyboard input.  The following bash script is what I have used for the LTI 360B laser.

``` bash
 #!/bin/bash

 stty -F /dev/ttyUSB0 speed 4800 cs8 -cstopb -parenb
 while true; do
   cat /dev/ttyUSB0 | while read LINE; do
     echo debug: $LINE
     echo $LINE | xdotool type --file -
   done
 done
```

This will only accept input from the device and direct it to the keyboard.  However,  not all computers are Linux and I have found it far more difficult in Windows and other OSes to do this.  The clear solution is a hardware device of some kind.

This will require the use of some soldering and programming.  I believe that the basic supplies that will be needed can be found at SparkFun.com.

* Pro Micro - 5V/16MHz - DEV-12640
* SparkFun Transceiver Breakout - MAX3232 - BOB-11189

The required connections will be (LTI to Transceiver to Micro):

* (1) Ground          --- Ground           --- Ground
* (2) Remote Trigger  <-- (R2Out <-- R2In) <-- Digital Pin
* (3) Serial In (Rx)  <-- (R1Out <-- R1In) <-- Tx0
* (4) Serial Out (Tx) --> (T1In --> T1Out) --> Rx1

This setup should allow for bi-directional communications.  As a standard HID (keyboard) only one-way communications will be initially implemented.  However, the addition of a button to a digital pin could allow for the remote trigger to operate properly if this is a requirement of the end user.

Code:

[[Category:FastMap|Adapter]]
