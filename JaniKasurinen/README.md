"EX5R Switches.bpanelz" is propably at stage of final version, but I might in future add some editing functions there.
The EX5/7 parameter sysex bug made some difficulties in making the panel, but it is actually in case of this hardware pretty useless sysex-implementation after all and new implementation has even removed parameter request totally from it's documentation.
- UPDATE: Added one more save button which also after saving, automatically advances to the next patch.

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
- ;-) "Kippis vuoan mulkut! Mie lähren tästä huilaamaan!"

- WARNING! SAMPLE DUMPS TO AX000 CAN EMPTY WHOLE RAM MEMORY FROM DEVICE EASILY. SO DOODLE EASY.
	- UPDATE: Limited "wavedata" to 1 packet to avoid corruption.
- 2024 MAY 7th: Major bug fixes on midi data handling and function loops dismandled. Might have affected multiple A4000 or A5000 owners. A5000 panel I have not updated yet with same fixes. OBS!

"V-Verb Pro FULL.bpanelz" is also a work in process as it only receives few first engine A model modulators fully from the sysex-dump.
- On 2024 20th April FIXED file handling bugs and removed PC hanging os.time function.
 
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
- UPDATE 2024 JUNE 24th: Sysex for Multipart and MIDI settings.
This is probably pretty final stage for this editor for now.

"Korg Prophecy Editor.bpanelz" has surely still many bugs and only few modulators are now fetched from the program bulk dump, but likewise to Z1 panel file handling and sysex-dumping works fully already.
- BACKUP ALL YOUR PROPHECY VOICES AND SETTINGS BEFORE USING THIS PANEL!
- 2024 May 6th: Bug fixed in "Load Patch to Edit Buffer"'s function which caused it to send patch from midi buffer even if no file was loaded = canceled the loading.
- 2024 May 7th: Minor formatting and more modulators fetched from patch midi dump.
- 2024 May 7th: Modulation OSC fixed. Formatting. Few more modulators called from patch dump.
- 2024 May 8th: Bug fixes. More modulators from patch dump. More saving and loading functionality, arp patterns, global and program writes to current and slot separated.
- A MAJOR BUG IN VST VERSION IN CAKEWALK: THE PANEL WILL REQUEST DUMP AND WRITE ON THE SLOT(21 OR LAST EDITED, DO NOT KNOW FOR SURE).
- MAKE BACKUPS, IF USING THIS PANEL!
- 2024 May 10th: Remedied the unintented write problem with a write protect switch, which might also help user prone accidental writings.

Korg Prophecy and Z1 panels are done from basis of this panel: https://ctrlr.org/710/ done by person with signature "jms" on CTRLR.ORG
A huge thank for the initial work done back in 2013 =)!

"Waldorf Blofeld Patch Renamer.bpanelz"
- A tiny panel for quick renaming of Waldorf Blofeld pacthes in edit buffer.
- Changed name must be saved by saving the pacth.

PS: Any PayPal donations to www.paypal.com/paypalme/janikasurinen are dearly appreciated =)