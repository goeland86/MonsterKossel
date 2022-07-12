### Monster Kossel: the firmware

At time of writing, the Monster Kossel has never been run with Marlin.

There's no reason it can't. A good SKR board and some finagling with Marlin will get you there for sure.

However I have been a long-time fan and contributor to the [Intelligent-Agent](https://github.com/intelligent-agent/) series of boards for the firmware.

Versions 1 and 2 of the Monster Kossel have run on the original Replicape + Beaglebone Black combo. Then when it was made available to me for beta testing, I switched it over to a Recore.
This means that I've only run two firmwares on this delta: Redeem (abandoned firmware for the Replicape), and Klipper.

Because I have never tried (nor wanted to) run it on any other board, I can only provide my Klipper configuration file for Recore for my delta.

# WARNING!

If you do not use Recore, the klipper config may be deprecated. That is because Recore is currently running its own fork of Klipper.
While it was developed specifically for Klipper usage, some new chip supports were needed in the base code, and as far as I know this hasn't yet merged upstream.

If you're using Recore and are building a 350mm bed, with 1000mm tall extrusions, this should be nearly plug & play. Simply make sure to re-measure your delta rod lengths and re-run the calibration routine.

Obviously if you're diverging from the BOM listed for the design, you'll need to adjust the config accordingly.
