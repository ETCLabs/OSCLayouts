Hi, so here's what to do:

Buy yourself a Korg nanoKONTROL2. Go download the nanoKONTROL2 editor software from Korg's website, then load the cobalt.nktrl2_data file using that software.



If you want to use pd (Windows users, or people who don't want to pay the small amount of money for OSCulator)
==============================================================================================================
Install pd (puredata.info). You'll want Pd-extended. Pd is not for the faint-of-heart. Run this patch. You'll probably have to muck about and set it up so that pd sees the Korg device as the MIDI input. If the patch is seeing MIDI, you'll see values changing live. In the patch, you always want to disconnect first, before connecting.

Run Eos as normal, setting it up to receive OSC as documented in the manual/Show Control user guide. Once it's working and you've put in all of the right IP addresses and ports and whatnot, you should have the Korg sliders moving Eos subs.



If you want to use OSCulator (Mac users)
========================================
Download and run OSCulator (osculator.net). Open the file in this zip. You may have to set up some parameters in the program.

Run Eos as normal, setting it up to receive OSC as documented in the manual/Show Control user guide. Once it's working and you've put in all of the right IP addresses and ports and whatnot, you should have the Korg sliders moving Eos subs.



Good luck!
Luke
lukedelwiche@gmail.com
