# Pi Class 2a: Lighting Up and LED and Breadboards
## Python GPIO

## Let's Light It Up
### Supplies
- 1 x LED
- 1 X 100 - 220 ohm resistor
- 2 X Male to Female jumper wires
- 1 X Breadboard

Let's get hands-on with electronics! This is where the Raspberry Pi comes in handy. You will program a light-emitting diode (LED) to flash. First you will need to make a circuit.
We will use a breadboard to quickly connect electronics into a circuit. The rows (bars) and columns (rails) have conductive metal strips that we can use to connect wires, LEDs, and other components.

![Breadboard](https://image.ibb.co/bKpFpb/68747470733a2f2f696d6167652e6962622e636f2f6965706a53772f53637265656e5f53686f745f323031375f31325f30375f61745f31305f30315f30375f414d2e706e67.png)

The LED has a short leg and a long leg. Put the long leg (positive, anode) into one row of the breadboard and shorter leg (negative, cathode) into a different row. Put one end of the resistor into same row as the negative, shorter leg of the LED. Put the other end of the resistor in the negative rail of the breadboard. Take another jumper wire and slot one end onto the short leg of the LED. You should end up with something that looks like this:

![RPi_Breadboard](https://image.ibb.co/dhBW7w/RPi_LED_bb2.png)

## Starting Python 
Open up Python on your Raspberry Pi (Programming > Python 3). Once the Python IDLE window opens, go to File > New File to type your code.

## Python Code

```python
# Flashing LED
from gpiozero import led
from time import sleep

led = LED(17)

while TRUE:
	led.on()
	sleep(1)
	led.off()
	sleep(1)


```
## Other Code to Try
### Blink

```python
# Flashing LED

from gpiozero import LED

led = LED(17)

led.blink()
```
Try some other values in led.blink(), what would these do:
- led.blink(5)
- led.blink(2, 0.5)
- led.blink(0.1, 10)
- led.blink(0.5, 0.5, 5, False)

### Stoplight Challenge
Can you create a stoplight with additional LEDs and pin?
![Breadboard and Stoplight](https://image.ibb.co/kvKReb/Screen_Shot_2017_12_11_at_11_00_28_AM.png)


## Resources
[LED documentation](https://gpiozero.readthedocs.io)
