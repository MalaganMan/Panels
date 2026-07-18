"Fantom-S - SonicCell - Patch Converter.bpanelz"
- 2025 January 19th: Newly added panel for converting Roland Fantom-S/XR patches to SonicCell and vice versa.
- 2025 January 20th: Patch listings added. No SRX-Expansion patchnames.
- 2025 January 20th: Patch selection functions updated. SRX-Patch selections corrected.
- 2025 April 1st: Waves are now also loaded and selected from sysex files to the converter.
- 2026 January 22nd: Fantom-XR PR-I Patchlist finalised.
- 2026 June 12th: Major bug fixes and featuters added. Complete face rework. SRX waves now working. Performance temps now requested and transmitted from patch temp loads.
- 2026 June 14th: Now also loading a patch to a text box will show Wave Number, Group and Bank from the loaded Sysex dump.

"Roland SonicCell - Fantom - XV - MC-909 - Patch ID Converter.bpanelz"
- 2026 June 25th: Advanced version of previous panel with XV-5050 and MC-909 ID injection into patch sysex dump. Sends Fantom, SonicCell and XV Patch dumps into MC-909 Part 1 Temp buffer.
- 2026 June 26th: Bug crashing the panel fixed on "Save.." and "Send.." buttons when sysex boxes are empty.
- 2026 June 29th: Added Performance requests and saving. Loading done with same buttons as patches. Bug fixes.
- 2026 June 30th: Added features, modified quide texes and formatting for easier usage.
- 2026 July 7th: Tick marks visible again after saving the panel with CtrlrX.org version.
- 2026 July 9th: Complete reface and some External Input parameters added. Setup & System Reques, Save and Load added.
- 2026 July 10th: Bugs in Mididatareceive function of non-existing variables fixed. MIDI OUT button remade.
- 2026 July 11th: Temporary Request, Save and Load added. Reface of positioning of groups and buttons.
- 2026 July 12th: Temporary Load -function had wrong ID 10 = Hx0A instead of 16 = Hx10 and made it inoperable.
- 2026 July 15th: Temporary Request has been streamlined to go without any delays. Will cause problems if simultaneous dump from in example Editors are asked. Based on flags of requested parts in sequence. Every device can now also Save and Load Rhythms.
- 2026 July 16th: Temporary Rhythm memory blocks are now intialized also when asking whole Temporary. MC-909 had never before MC909_Rhythm intialized, so it didn't work before. Rhythm memoryblock size is checked more accurately before saving to avoid problems.
- 2026 July 18th: All Temporary buffers can now be requested, saved and load. Can also select to request only Performance and Patches.