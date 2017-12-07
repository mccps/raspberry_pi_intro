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

To react to a button connected to GPIO pin 2.0, simply set the pin as input, and use the ‘gpio (x) is high?’ block to check the button’s state. In the example below, the Scratch cat will say “Pressed” only when the button is being held down.

## Let's Light It Up
### Supplies
- 1 x LED
- 1 X 100 - 220 ohm resistor
- 2 X Male to Female jumper wires
- 1 X Breadboard

Let's get hands-on with electronics! This is where the Raspberry Pi comes in handy. You will program a light-emitting diode (LED) to flash. First you will need to make a circuit.

The LED has a short leg and a long leg. Put the long leg (positive, anode) into one row of the breadboard and shorter leg (negative, cathode) into a different row. Slot the resistor into the other end of the same jumper wire. Add another jumper wire the other end of the resistor. Take another jumper wire and slot one end onto the short leg of the LED. You should end up with something that looks like this:

## Resources
[Scratch 2.0 on Raspberrypi.org](https://www.raspberrypi.org/blog/scratch-2-raspberry-pi/)
