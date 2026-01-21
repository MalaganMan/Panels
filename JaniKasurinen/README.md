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
- 2025 April 20th: Bug fixes and lots of visual tweaking.

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
- 2025 April 18th: Updated the outlook and info texts.
- 2025 July 3rd: Moved blue "Edit Buffer Send" -button to patch group for better usability. Changed color of incremental patch saving to orange.

Korg Prophecy and Z1 panels are done from basis of this panel: https://ctrlr.org/710/ done by person with signature "jms" on CTRLR.ORG
A huge thank for the initial work done back in 2013 =)!

"Waldorf Blofeld Patch Renamer.bpanelz"
- A tiny panel for quick renaming of Waldorf Blofeld pacthes in edit buffer.
- Changed name must be saved by saving the pacth.

PS: Any PayPal donations to www.paypal.com/paypalme/janikasurinen are dearly appreciated =)