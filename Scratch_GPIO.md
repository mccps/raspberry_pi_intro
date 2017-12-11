# Pi Class 2: Lighting Up and LED and Breadboards
## Scratch 2.0 GPIO

With the September 2015 release of Scratch for the Raspberry Pi,  there’s a new GPIO server to make driving LEDs, buzzers, HATS, and other devices and components easier.
![GPIO Pins](https://i.stack.imgur.com/yWGmW.png)
## Starting Scratch
Open up Scratch 2.0 on your Raspberry Pi (Programming > Scratch 2.0).

## Starting the server
Scratch 2.0 on the Raspberry Pi allows you to create code to control and respond to components connected to the Pi’s GPIO pins. This means that your Scratch projects can light LEDs, sound buzzers and use input from buttons and a range of sensors to control the behaviour of sprites. Interacting with GPIO pins use custom blocks for setting pin output and getting current pin state.

![Pi GPIO Exension](https://www.raspberrypi.org/app/uploads/2017/06/extension.png)

In the ‘More Blocks’ section you should now see the additional blocks for controlling and responding to your Pi GPIO pins. To give an example, the entire code for repeatedly flashing an LED connected to GPIO pin 2.0 is now:

![GPIO_Sequence](https://www.raspberrypi.org/app/uploads/2017/06/led.png)

To react to a button connected to GPIO pin 2.0, simply set the pin as input, and use the ‘gpio (x) is high?’ block to check the button’s state.

## Let's Light It Up
### Supplies
- 1 x LED
- 1 X 100 - 220 ohm resistor
- 2 X Male to Female jumper wires
- 1 X Breadboard

Let's get hands-on with electronics! This is where the Raspberry Pi comes in handy. You will program a light-emitting diode (LED) to flash. First you will need to make a circuit.
We will use a breadboard to quickly connect electronics into a circuit. The rows (bars) and columns (rails) have conductive metal strips that we can use to connect wires, LEDs, and other components.

![Breadboard](https://image.ibb.co/iepjSw/Screen_Shot_2017_12_07_at_10_01_07_AM.png)

The LED has a short leg and a long leg. Put the long leg (positive, anode) into one row of the breadboard and shorter leg (negative, cathode) into a different row. Put one end of the resistor into same row as the negative, shorter leg of the LED. Put the other end of the resistor in the negative rail of the breadboard. Take another jumper wire and slot one end onto the short leg of the LED. You should end up with something that looks like this:

![RPi_Breadboard](https://image.ibb.co/mzy8sw/Screen_Shot_2017_12_11_at_9_34_20_AM.png)

## Scratch
Once your circuit is wired up, we add code to Scratch to send power to the LED. In the diagram above we have the positive leg of the LED to GPIO pin #17 (even though it is the 6th pin from the top). Make sure you refer to the pin diagram at beginning to make sure you are using the correct pins (***Using the wrong pins can damage your Pi and electrical components***).

Drag the Scratch scripts shown below and connect them in order. Before running the code, can you predict what the LED will do?

![Scratch LED Sequence](https://image.ibb.co/d3N4zb/scratch_led_sequence.jpg)

## You've Made Light!
Now that you've mastered one led, can you:
- Flash your LED at different speeds, how fast can you make it flash?
- Can you make a dot (short flash) and dash (long flash) and use to make a distress beacon. S(...) O(---) S(...)
- Add more LEDs to create a set of traffic lights and program an appropriate sequence.



## Resources
[Scratch 2.0 on Raspberrypi.org](https://www.raspberrypi.org/blog/scratch-2-raspberry-pi/)
