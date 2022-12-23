**nova_regions** lets you divide the [Nova's](https://mosiaudio.com/products/nova) touchpanel into multiple regions to play multiple sounds.

To use:

  1. Download [Pd (Pure Data)](https://puredata.info/downloads/pure-data)
  2. Connect the Nova via USB.
  3. Open **nova_hor_split.pd**
  4. In Pd, go to Media -> MIDI Settings... and set:
       * Input Device: "USB MIDI Device" (the Nova)
       * Output Device: "IAC Driver" (Mac) OR use [loopmidi](https://www.tobias-erichsen.de/software/loopmidi.html) (Windows)
       * (Optional: Press "Save All Settings" to save between sessions.)
  5. Open a DAW that can receive multiple midi channels (Ableton, Logic, Reaper, etc.)
  6. Set the DAW's MIDI input to the IAC Driver (Mac) or loopmidi (windows), and make sure the Nova's MIDI input is *not* enabled in the DAW.
  7. Create several instruments and map each to a different midi channel.
  8. Play the Nova and the different areas of the touchpad should now route to different instruments in your DAW.

To customize the layout, check out [this video](https://youtu.be/6fuAdswDMgc).
