"EX5R Switches.bpanelz" is propably at stage of final version, but I might in future add some editing functions there.
The EX5/7 parameter sysex bug made some difficulties in making the panel, but it is actually in case of this hardware pretty useless sysex-implementation after all and new implementation has even removed parameter request totally from it's documentation.
- UPDATE: Added one more save button which also after saving, automatically advances to the next patch.
- UPDATE 2024 September 12th: Added some perhaps useful commands and removed unwanted VST indexes.
- UPDATE 2024 September 13th: Added VL Element sysex handling and saving.
- UPDATE 2024 September 13th#2: Added VL Element sysex handling and saving functionality and made other improvements.
- UPDATE 2024 September 16th: Non-existing variable bug remedied.
- UPDATE 2024 September 27th: Features added and MIDI OFF after each dump receive.
- UPDATE 2024 September 28th: Features added.
- UPDATE 2024 September 29th: Propably final features added. Full preset and internal voice lists created and enabled for creation with switch.
- UPDATE 2024 September 30th: Saving and loading voice lists for Internal Banks.
- UPDATE 2024 October 1st: Bug fixes and styling.
PLEASE, save your full EX5R always before using this panel. Had already done some messing with voices while sysex dumping with this panels development.
-Device ID is still mostly fixed on 1 with most dumps, but will correct that later. Check sum editing causes some trouble there.

"YAMAHA A4000 SAMPLER MANIPULATOR.bpanelz" is now at current final state and wont likely to be edited soon again.
- Update 2024 22th April 04:25 GMT: FIXED file handling bugs and removed PC hanging os.time function.
- NOTE!: After experimenting with midi dumps you must send all data in this order back to A4000: 
"wavedata" - "sample bulk" - "sample bank dump" - "Program dump".
- I gave up trying to calculate the right checksum so only unmodified midi dumps will succeed hence the checksum is incorrect otherwise and will fail the dumps.
- UPDATE 23th April 2024: Added more features of which most usefull is the objectlist request.
- UPDATE 23th April 2024 #2: Uploaded YAMAHA A5000 panel version with correct "family device code" ASCII "5" = 35h = 53 incomparison A4000 ASCII "4" = 34h = 52.
- UPDATE 26th April 2024: Bug fixes on MIDI ON/OFF. Object list bug fixing. Object list is now at least quite functional.
- UPDATE 27th April 2024: Major bug fixes and separated object types into own list from dump.
- UPDATE 29th April 2024: Removed Program list. Major bug fixes.
	- File Load Cancelin actually triggered earlier buffers to be send and written to the text boxes.
	
- Hopefully last update for a looog time: Object lists now injects names from list strings to name boxes for selecting samples and samplebanks easier.
- Last piece of advice: Edit the "Program Select" -modulator to send program change CC (number 32 seems to work) and allow program change in YAMAHA AX000 and you will always have the matching "Program Number" and "Program Name". - Update: That is done.

- WARNING! SAMPLE DUMPS TO AX000 CAN EMPTY WHOLE RAM MEMORY FROM DEVICE EASILY. SO DOODLE EASY.
	- UPDATE: Limited "wavedata" to 1 packet to avoid corruption.
- 2024 MAY 7th: Major bug fixes on midi data handling and function loops dismandled. Might have affected multiple A4000 or A5000 owners. A5000 panel I have not updated yet with same fixes. OBS!

"V-Verb Pro FULL.bpanelz" is also a work in process as it only receives few first engine A model modulators fully from the sysex-dump.
- 2024 20th April FIXED file handling bugs and removed PC hanging os.time function.
- 2024 11th August: Second/lower OK/TAP button fixed. Unneccery code disabled in set combich function. Setting panel midi channel should be enough for panel buttons to work.
- 2024 12th August: NEW FEATURE: Screen dump request and display manually.
- 2024 12th August#2: Necessary font 'ZXSpectrumJJK.ttf' for the Screendump suplied here also.
- 2024 14th August: The panel should now be missing most of the return values from the sysex dumps, but should otherwise work usably.
- 2024 15th August: Renaming of Engines and Combis now possible via rewriting with a new hex string at the end of the sysex dump.
- 2024 15th August: All rotaries changed to Vertical Drag style.
- 2024 26th August: Looping bug remedied. Received NRPN displays added. Sysex handling aids added.

"Korg Z1 Editor.bpanelz" is still greatly work in process stage and does NOT have all the modulators, but file loading saving and storing functions fully.
- BACKUP ALL YOUR Z1 VOICES AND SETTINGS BEFORE USING THIS PANEL!
- 2024 May 6th: Bug fixed in "Load Patch to Edit Buffer"'s function which caused it to send patch from midi buffer even if no file was loaded = canceled the loading.
- VPM added to OSC1 and OSC2
- UPDATE 2024 MAY 28th: Buggy last version remade and fixed minor older bugs.
- UPDATE 2024 JUNE 3th: Oscillator modulators until "Sync" done.
- UPDATE 2024 JUNE 4th: Organ Model added.
- UPDATE 2024 JUNE 5th: Electric Piano and Brass Model added.
- UPDATE 2024 JUNE 6th: FIXED ALL BYTE VALUES IN MODULATORS WHICH WERE TOTALLY MISSING.
- UPDATE 2024 JUNE 9th: All Oscillator modulators done one directional.
- UPDATE 2024 JUNE 11th: Fixed back 6th of June mistake with modulator values and functionalized patch changes to work bidirectionally and removed linking that to save slot.
- UPDATE 2024 JUNE 23th: Finished FX and sysex without Multipart handling.
- UPDATE 2024 JUNE 24th: Sysex for Multipart and MIDI settings(Uncomplete!).
This is probably pretty final stage for this editor for now.
- Was not =) UPDATE 2024 JUNE 27th: Grouped the functions and removed the unneccery ones. Fixed some bugs. Multi and Midi sysex are still missing correct sizes and thus not function fully.
- UPDATE 2024 JUNE 28th: Bug fixing and new 'Dump byte calculator' added to aid in understanding the bulk dump.
- 2024 10th July: Sysex bug fix and removed unfuntional Mono SW.
- 2024 17th July: Performance Editor added.
- 2024 July 26th: Arpeggio Editor added, minor updates and bug fixes. Last page of arp this not linked to notes.
- 2024 July 27th: Arpeggio Editor added, minor updates and bug fixes. All Notes linked to last arp tabs matrix.
- 2024 August 1st: Arpeggio Editor fixed (not fully propbably) and some other advance done.
- 2024 August 5th: Arpeggio Editor fixed (fully propbably).
- 2024 August 6th: Tested and Pitch offset % removed from Arp values.
- 2024 August 8th: Arpeggio editors VST exports removed and all modulators in there also muted on start.
- 2024 August 26th: Sysex hexes have been manually lined up to text boxes to avoid misalignment with numbers for columns.
- 2024 August 27th: Added midi off switch to prevent sysex sending in start of the panel.

"Korg Prophecy Editor.bpanelz" has surely still many bugs and only few modulators are now fetched from the program bulk dump, but likewise to Z1 panel file handling and sysex-dumping works fully already.
- BACKUP ALL YOUR PROPHECY VOICES AND SETTINGS BEFORE USING THIS PANEL!
- 2024 May 6th: Bug fixed in "Load Patch to Edit Buffer"'s function which caused it to send patch from midi buffer even if no file was loaded = canceled the loading.
- 2024 May 7th: Minor formatting and more modulators fetched from patch midi dump.
- 2024 May 7th: Modulation OSC fixed. Formatting. Few more modulators called from patch dump.
- 2024 May 8th: Bug fixes. More modulators from patch dump. More saving and loading functionality, arp patterns, global and program writes to current and slot separated.
- A MAJOR BUG IN VST VERSION IN CAKEWALK: THE PANEL WILL REQUEST DUMP AND WRITE ON THE SLOT(21 OR LAST EDITED, DO NOT KNOW FOR SURE).
- MAKE BACKUPS, IF USING THIS PANEL!
- 2024 May 10th: Remedied the unintented write problem with a write protect switch, which might also help user prone accidental writings.
- 2024 July 14th: All existing parameters on panel should now get updated with patch dumps.
- 2024 July 15th: Bug fixes and some Arpeggio and CC controls added.
- 2024 July 18th: Arpeggio steps editor added.
- 2024 July 26th: Minor updates.
- 2024 August 1st: Major updates and propably the final version for a long time =D Patch lists can now be read from bank dumps and all the patches can be seen at once.
- 2024 September 6th: Patchlist tweaking and made note that it should be only used for selecting patches because the names in those lists might be partially incorrect.
- 2024 September 6th #2: General Arpeggio parameters fetch when changing patterns. Step values still unfetched, but will do later.
- 2024 September 7th: Final version for now. Arpeggio return values finished.
- 2024 September 8th: Some final tweaks and function to adjust arpeggio length more easily.
- 2024 September 8th #2: Some final tweaks and putting some VST indexes in order for modulators and especially for the arpeggio length so that I can play with it =).
Most VST indexes are still just random numbers and not in any order.

Korg Prophecy and Z1 panels are done from basis of this panel: https://ctrlr.org/710/ done by person with signature "jms" on CTRLR.ORG
A huge thank for the initial work done back in 2013 =)!

"Waldorf Blofeld Patch Renamer.bpanelz"
- A tiny panel for quick renaming of Waldorf Blofeld pacthes in edit buffer.
- Changed name must be saved by saving the pacth.

"MIDI Box SID panel for anyone else who might still use this old PIC and version 1
- 2024 July 28th: Tryed to rationalize the panel, so that others can use it too =)
- 2024 July 29th: Completing as much as possible and added a functionality to get all patch names from the bank sysex dump.
- 2024 August 03th: Bug in patch name fetcing fixed and function simplified by using only string.format function.
- 2024 August 09th: Bug fixes in sysex dump handling.

PS: Any PayPal donations to www.paypal.com/paypalme/janikasurinen are dearly appreciated =)