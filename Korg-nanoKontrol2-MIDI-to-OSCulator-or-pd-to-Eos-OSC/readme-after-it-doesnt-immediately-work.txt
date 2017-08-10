Do you have a Korg nanoKONTROL2 USB MIDI panel and want to run Eos-family faders? You might want to consider using Luminosis instead of either method below. The pd and OSCulator methods below were created/documented before Luminosis existed - but it is a far cleaner and easier solution than either pd or OSCulator. It is purpose-built for doing exactly this. Luminosis is on the ETC Labs github site.

https://github.com/ElectronicTheatreControlsLabs/LuminosusEosEdition

But maybe you are bringing in other signals with pd or OSCulator, and want to also have the MIDI panel as part of that setup? Read on!

Hardware and panel setup
==============================================================================================================
Buy yourself a Korg nanoKONTROL2. Go download the nanoKONTROL2 editor software from Korg's website, then load our included cobalt.nktrl2_data file using that software. There is nothing particularly special about this layout except that it gives you a panel mapping which is compatible with the pd and OSCulator files included. This mapping is also directly compatible with Cobalt ETCnomad via USB MIDI. You could leave the Korg panel at factory defaults and then adjust pd/OSCulator to suit that mapping.


If you want to use pd (Windows users, or people who don't want to pay the small amount of money for OSCulator)
==============================================================================================================
Install pd (puredata.info). You'll want Pd-extended. Note that Pd is not for the faint-of-heart! If you aren't very technical but you have a relative or friend who watches Doctor Who and has strong opinions about Star Trek TNG vs DS9, you might want to get them involved. Run this patch. You'll probably have to muck about and set it up so that pd sees the Korg device as the MIDI input. If the patch is seeing MIDI, you'll see values changing live. In the patch, you always want to disconnect first, before connecting.

Run Eos as normal, setting it up to receive OSC as documented in the manual/Show Control user guide. Once it's working and you've put in all of the right IP addresses and ports and whatnot, you should have the Korg sliders moving Eos subs.


If you want to use OSCulator (Mac users)
========================================
Download and run OSCulator (osculator.net). Open the file in this zip. You may have to set up some parameters in the program.

Run Eos as normal, setting it up to receive OSC as documented in the manual/Show Control user guide. Once it's working and you've put in all of the right IP addresses and ports and whatnot, you should have the Korg sliders moving Eos subs.

Protip: OSCulator likes to automatically change its target when it discovers new OSC-capable devices, e.g. an iPad running TouchOSC. This will drive you crazy. Set the Eos as the secondary but default target.

Good luck!
Luke
lukedelwiche@gmail.com
