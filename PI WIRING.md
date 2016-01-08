# Wiring Map / Methodology for the RPi

## Initial Thoughts
- Battery powered system.  Battery in this case is a smart charge battery pack, capable of pass through charging.  The charger for the battery pack would be a two-port 120V, 4.0+ amp wall charger.  One of those ports is connected via micro USB cable to the battery pack's charge port.  A second micro USB cable is connected from the battery pack to the Raspberry Pi.  A third cable is cut, and the red +5V wire is connected to one of the GPIO pins on the Raspberry Pi.  A process is written that polls the IO pin every 5000 ms.  If the power is found to be off, it starts a timer, which can be customized based on the battery pack available.  If the timer exceeds that threshold value, it sends the appropriate HALT signals to all processes, including the FermentPi system, which should be constantly logging it's state anyway. 
  - A comment was found on the RPi Stach Exchange that seems to indicate GPIO Pin 5 will boot the RPi if applied to ground.  Further research also reveals the possibility of using the P6 header and momentarily shorting those 2 pins.  Test these, and come up with a circuit to allow for that.
  
## GPIO

