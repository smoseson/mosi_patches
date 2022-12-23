**muse_drag** lets you change the [Nova's](https://mosiaudio.com/products/nova) default x/y CC output to a single drag-distance-based CC output.

To use:

  1. Download [Pd (Pure Data)](https://puredata.info/downloads/pure-data)
  2. Connect the Nova via USB.
  3. Open **muse_drag.pd**
  4. In Pd, go to Media -> MIDI Settings... and set:
       * Input Device: "USB MIDI Device" (the Nova)
       * Output Device: "IAC Driver" (Mac) OR use [loopmidi](https://www.tobias-erichsen.de/software/loopmidi.html) (Windows)
       * (Optional: Press "Save All Settings" to save between sessions.)
  5. Open a DAW and set its MIDI input to the IAC Driver (Mac) or loopmidi (windows), and make sure the Nova's MIDI input is *not* enabled in the DAW.
  7. Load a VST instrument and midi-learn a parameter.
  8. Play the Nova and the parameter should change based on the drag distance.

Troubleshooting:

  * If "USB MIDI Device" is not shown in the Input drop-down then make sure the Nova is plugged in and powered on before opening Pd.
