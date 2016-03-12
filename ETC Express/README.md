![ETC Express](http://www.etcconnect.com/uploadedImages/Main_Site/Images/Products/Consoles/Express72-144.jpg?n=5600)
# ETC Express Mobile Layout

Even though the [ETC Express](http://www.etcconnect.com/Support/Consoles/Legacy/Express/) is a legacy product, it is still being used. These layouts are to create a way to control the board very easily and wirelessly. As the age of the console disallows the current methods of wireless control used by the [ETC Eos Family](http://www.etcconnect.com/Products/Consoles/Eos-Family/), these layouts uses roundabout ways of control.

## Installation
### Requirements
* Computer running a version of [Windows](https://www.windows.com/),
* [ETC Express Lighting Console](http://www.etcconnect.com/Support/Consoles/Legacy/Express/)
* MIDI to USB adapter
* Mobile device capable of running [touchOSC](http://hexler.net/software/touchosc) ([iOS](http://www.apple.com/ios/) or [Android](https://www.android.com))

A non-Windows computer may possibly be used, but MIDI-OX has not been tested for alternative systems. (See To-Do section.)

### Instructions

1. Install [MIDI-OX](http://www.midiox.com), [touchOSC Bridge, and touchOSC Editor](http://hexler.net/software/touchosc) on the computer.
2. Buy and install touchOSC on the mobile device. ([App Store](https://itunes.apple.com/app/touchosc/id288120394), [Google Play](https://play.google.com/store/apps/details?id=net.hexler.touchosc_a), [Amazon](http://www.amazon.com/gp/product/B00GN83WHQ))
3. Connect the MIDI adapter from the MIDI i/o of the board into a USB port of the computer
4. Open touchOSC Bridge and touchOSC
5. Create new configuration in MIDI-OX connecting the Board (probably called USB or some variation) as output to touchOSC Bridge as input
6. Install interface on device and set output to computer. (Detailed instructions [here](http://hexler.net/docs/touchosc))
7. Create all macros as specified in `Macros.csv`
8. Enjoy.

## Further documentation

All the objects on both interfaces are documented in the `Interface Objects.csv` file. OSC programs can be made with the information.

* `/(Mobile Tab)/(OSC Name)` is the path for objects on the mobile interface, and
* `/1/(OSC Name)` is the path for objects on the iPad inteface.

## Contributions

Any contributions would be greatly appriciated to improve on the interface or to add functionality. Check the To-Do list for topics to investigate.

## To-do
[ ] Implement sliders as described on page 280 of the ETC Express manual using "Pitch Bend" messages
[ ] Add text-field in the interface as a command-line (OSC program needed)
[ ] Warnings when illegal (error) keypresses performed
[ ] Better use of space
[ ] Explore the use of Linux as proxy for console.
