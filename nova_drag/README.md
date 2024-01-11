**muse_drag** lets you change the [Nova's](https://mosiaudio.com/products/nova) default x/y CC output to a single drag-distance-based CC output.

To use:

  1. Download the [mosi patches](https://github.com/smoseson/mosi_patches/archive/refs/heads/main.zip)
  2. Install [Pd (Pure Data)](https://puredata.info/downloads/pure-data)
  3. Connect the Nova via USB.
  4. Open the **muse_drag.pd** mosi patch.
  5. In Pd, go to Media -> MIDI Settings... and set:
       * Input Device: "USB MIDI Device" (the Nova)
       * Output Device: "IAC Driver" (Mac - if you don't see it follow [these steps](https://support.apple.com/guide/audio-midi-setup/transfer-midi-information-between-apps-ams1013/mac#:~:text=In%20the%20Audio%20MIDI%20Setup,to%20turn%20on%20the%20driver.)) OR use [loopmidi](https://www.tobias-erichsen.de/software/loopmidi.html) (Windows)
       * Optional: Press "Save All Settings" to save between sessions.
  6. Open a DAW and set its MIDI input to the IAC Driver (Mac) or loopmidi (windows), and make sure the Nova's MIDI input is *not* enabled in the DAW.
  7. Load a VST instrument and midi-learn a parameter.
  8. Play the Nova and the parameter should change based on the drag distance.

Troubleshooting:

  * If "USB MIDI Device" is not shown in the Input drop-down then make sure the Nova is plugged in and powered on before opening Pd.
