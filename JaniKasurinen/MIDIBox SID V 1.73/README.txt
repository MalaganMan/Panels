"MIDI Box SID panel for anyone else who might still use this old PIC and version 1
- 2024 July 28th: Tryed to rationalize the panel, so that others can use it too =)
- 2024 July 29th: Completing as much as possible and added a functionality to get all patch names from the bank sysex dump.
- 2024 August 03th: Bug in patch name fetcing fixed and function simplified by using only string.format function.
- 2024 August 09th: Bug fixes in sysex dump handling.
- 2026 January 22nd: Saving = dumping the patch to SID 1.73 is still not working easily with all parameters. Still working to find out what's the correct procedure the get the edited patch to be saved with all parameters into to MIDIBox SID. I believe the key was to collect all to store and then send it to the MIDIBox SID and after that fetch it again as sysex before saving to PC. Not very simple yet, but maybe I can later simplify the saving process.
- 2026 January 24th: Made instructions for naming and saving the patches. Saving isn't simple, but I managed to get it working somehow. Java editor is still the best =D
- 2026 January 25th: Visual appearance tweaks.