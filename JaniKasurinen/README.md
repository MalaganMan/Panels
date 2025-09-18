"Fantom-S - SonicCell - Patch Converter.bpanelz"
- 2025 January 19th: Newly added panel for converting Roland Fantom-S/XR patches to SonicCell and vice versa.
- 2025 January 20th: Patch listings added. No SRX-Expansion patchnames.
- 2025 January 20th: Patch selection functions updated. SRX-Patch selections corrected.
- 2025 April 1st: Waves are now also loaded and selected from sysex files to the converter.

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
- PLEASE, save your full EX5R always before using this panel. Had already done some messing with voices while sysex dumping with this panels development.
- Device ID is still mostly fixed on 1 with most dumps, but will correct that later. Check sum editing causes some trouble there.
- UPDATE 2024 October 2st: Device_ID now changed for sysex dumps and checked on receive to match. Confusion still possible with MIDI out and in channels. Uploaded text files of preset and internal banks for EX5R named Preset Bank 1/2 and Internal Bank 1/2.txt
- UPDATE 2024 October 3st: Bug fixes and styling.
- UPDATE 2024 October 4st: Managed to get also the User VL Element name list saving and loading working. When changing voice type there is still a bug that makes asking current voice dump several times necessary to get the right bank and sample to show up in the first element. No more need for extra text boxes after correcting save funtions length call for the text.
- UPDATE 2024 October 6th: Minor updates/finishing current modulator returns.
- UPDATE 2024 October 8th: Oh yes, I could not at this moment figure out how to else prevent lua code from using non existent variable than making them exist with that little "Request 1st Preset" button. So please, keep that on while closing the panel or use it at the beginning always, but disable it later.
- UPDATE 2025 January 23rd: Both PATCH and PERFORMANCE change main selections work now with enabling midi out ON.
 
 "YAMAHA A4000 SAMPLER MANIPULATOR.bpanelz & YAMAHA A5000 SAMPLER MANIPULATOR.bpanelz"
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
- UPDATE 2024 October 24th: Added new features and tried to kill bugs. Now wave and loop addresses are updated on the panel and to control sliders for up to 65536 samples long samples.
- UPDATE 2024 October 25th: Added new features and tried to kill bugs. Now wave and loop addresses are updated on the panel and to control sliders for all sample lengths.
- UPDATE 2025 January 4th: Bug fix in loop point controls.
- UPDATE 2025 January 4th on A5000 panel: Bug fix in loop point controls and added the same features as in A4000 panel.
- UPDATE 2025 January 23rd on A5000 panel: (Trying to) Fix bootup button pushes and lua executions.
- UPDATE 2025 February 27th on A4000 panel: FX section updated with parameter names and so far until TECH MODULATION/FX3 fully adjusted values and labels (Except I believe you can not actually change some delay values so precise =D. Input/output settings also now added.
- UPDATE 2025 March 3rd on A4000 panel: At least I had a bug which disabled LUA in my VST version. Now got it working again.
- UPDATE 2025 April 22nd on A4000 panel: Visual tuning and minor bug fixes.
- UPDATE 2025 April 24th on A4000 panel: Added "smarter" loop point control functions.
- UPDATE 2025 April 27th on A4000 panel: Added funtionality for sample handling.
- UPDATE 2025 April 29th on A4000 panel: Added funtionality for program selection. Bug fixes and new parameters.
- UPDATE 2025 April 29th on A4000 panel: Added funtionality. Bug fixes and new parameters. SDS dumping for samples skips now the box with new(uppes SDS buffer) buttons. Might for well. We'll see that =)
- UPDATE 2025 April 30th on A4000 panel: Added funtionality. MAJOR BUG FIXED IN ALLOWING TO DELETE WHILE BANKS EXIST = RESULTS IN WRONG SAMPLE DELETION. Object linking the most important update.
- UPDATE 2025 May 2nd on A4000 panel: Added funtionality. Updatable program list with full names.
- UPDATE 2025 May 2nd on A4000 panel: Added Multi Part Selections.
- UPDATE 2025 May 3th on A4000 panel: Finally got working FULL sample dumping for short MONO samples (Stereo SDS might not be a thing at all). Try higher global MIDI delay for longer samples.
- UPDATE 2025 May 4th on A4000 panel: Some styling and adding boxes everywhere. FULL PROGRAM REQUEST, SAVE AND LOAD! Both A4000 and A5000. No cross breeding! Yet!
- Note!: The AX000 panel should now be able to control both A5000 and A4000
- UPDATE 2025 May 5th on AX000 panel: FX sections for A5000 and selection for the model A4000 or A5000. Ah yes, and ONLY 4 first Effects have proper limits and values set. So, still work to be done =D
- UPDATE 2025 May 13th on AX000 panel: Unlucky day, maybe. For A3000 users. Added model to requests. Button makros should be disabled when A3k selected != Unknown results. A3000 FX undone. 4 first FX might be the same for all.
- UPDATE 2025 May 14th on AX000 panel: Minor bug fixes on knobs etc.
- UPDATE 2025 May 15th on AX000 panel: Non-funtional FX selection working now. Trying to fix Program selection issues. No links.
- UPDATE 2025 May 15th#2 on AX000 panel: Wave Data flag added for Stereo samples to work in midi dump. VST indexes still messed up.
- UPDATE 2025 May 16th on AX000 panel: When saving full program, program number in form "Pgm 001" is added to the name in dialog.
- UPDATE 2025 May 18th on AX000 panel: Selection for only fetching program names while changing the program.
- UPDATE 2025 May 19th on AX000 panel: VST indexes corrected. Styling and some small bugs fixes. (And new created =)
- UPDATE 2025 May 23th on AX000 panel: Sequence LUA code is now only for small under 8192 dumps. Haven't got a proper way in this panel to get and send dumps, so external application is adviced for dumping and receiving sequences to and from the sampler. Sample level and outputs added. (Were bare minimum for any use of this panel =D
- UPDATE 2025 May 25th on AX000 panel: Some parameters for Program added. Program LFO settings and control settings. Removed annoying extra program selector.
- UPDATE 2025 May 26th on AX000 panel: Added proper logic when adding samples to program OR to a bank.
- UPDATE 2025 May 28th on AX000 panel: Visual styling and bug fixes.
- UPDATE 2025 May 28th#2 on AX000 panel: Current "Alles ok version."
- UPDATE 2025 May 29thon AX000 panel: Lost buttons for Full Program dumps restored and added buttons also for Full Sample Banks.
- UPDATE 2025 May 29thon#2 AX000 panel: Disabling wave/loop controls before selecting a sample!!!!
- UPDATE 2025 May 29thon#3 AX000 panel: Disabled any logic in wave/loop control settings. Can now go illegal, but at least works without hickups.
- UPDATE 2025 May 30th AX000 panel: Hopefully the last major bug fixes this spring before summer to this panel. Now MIDI OUT remains OFF while getting all the modulators. Safer this way. No more edited sample parameters while getting the values to the panel.
- UPDATE 2025 May 31th AX000 panel: Corrected sample makros (Tree has different sorting than main screen, you know =). Added adjustment for know and button delays. Please keep them high enough = 300 ms and 1000 ms?? Added code for getting all the program names with a single button.
- UPDATE 2025 June 2nd AX000 panel: MAJOR BUG FIXED. 1 "End" in wrong place in the "mididatareceived" function. Loop length got messed up.
- UPDATE 2025 June 2nd Afternoon AX000 panel: MAJOR BUG FIXED. Button and knob delays had to initialized.
- UPDATE 2025 June 5th AX000 panel: More perfect sample linking logic. (Hide, unhide)
- UPDATE 2025 June 18th AX000 panel: Enabled MIDI OUT ON on effect change to make it more user friendly. Might cause issues thou, but will see.
- UPDATE 2025 September 3rd AX000 panel: 15 first Effects (to LOFI) with proper value display. Major formatting. Full Program, Bank and Sample dump receiving, saving and loading should work for tiny = floppy?? samples.
- UPDATE 2025 September 3rd#2 AX000 panel: Sample and Sample Bank Renaming now possible with a button makro. Use with care to avoid any harm!
- UPDATE 2025 September 8th AX000 panel: Sample and Sample Bank Renaming with a button makro now faster. Use with care to avoid any harm! 18 first Effects has proper values.
- UPDATE 2025 September 10th AX000 panel: 25 first Effects has proper values.
- UPDATE 2025 September 11th AX000 panel: 30 first Effects has proper values.
- UPDATE 2025 September 14th AX000 panel: Added missing VST indexes back to buttons and knobs for use within DAWs for easy control and wishing them not to be pressed upon loading again. Corrected FX visible/VST names for the effect parameters in Effects 4 to 6 (A5000). 30 first Effects has proper values.
- UPDATE 2025 September 18th AX000 panel: 54 first Effects have now proper values. Added Target Program & Target Sample buttons for faster switching between objects. Sends only the name of the object to the sampler. Organized a bit the buttons.

"V-Verb Pro FULL.bpanelz" is also a work in process as it only receives few first engine A model modulators fully from the sysex-dump.
- 2024 20th April FIXED file handling bugs and removed PC hanging os.time function.
- 2024 11th August: Second/lower OK/TAP button fixed. Unneccery code disabled in set combich function. Setting panel midi channel should be enough for panel buttons to work.
- 2024 12th August: NEW FEATURE: Screen dump request and display manually.
- 2024 12th August#2: Necessary font 'ZXSpectrumJJK.ttf' for the Screendump suplied here also.
- 2024 14th August: The panel should now be missing most of the return values from the sysex dumps, but should otherwise work usably.
- 2024 15th August: Renaming of Engines and Combis now possible via rewriting with a new hex string at the end of the sysex dump.
- 2024 15th August: All rotaries changed to Vertical Drag style.
- 2024 26th August: Looping bug remedied. Received NRPN displays added. Sysex handling aids added.
- 2024 31st October: Removed unneccery VST-indexes causing a long list of "undefined" paramaters in VST.
- 2024 17th November: Fixed the Edit Buffer sysex to modify only device id and nothing else when loading.
- 2024 19th November: "REQUEST EDIT BUFFER" now only triggers that and nothing else. No more asking combis or engines to get the parameters, which caused often a infinite loop. Could not make it work properly, to say.
- 2024 8th December: Return values from Edit Buffer until B Engines Theater algorithm. Device ID bugs fixed in LUA codes. Other fixes and changes made.
- 2024 8th December#2: Return values from Edit Buffer until B Engines REVERSE REVERB algorithm. Some fixes made.
- 2024 9th December: All parameters are now returned from Edit Buffer dump to modulators. Some fixes made.
- 2024 9th December#2: Bug fix off wrong variable name in COMBI selection function.
- 2024 10th December: Tweaks to requests of engines and combi returns.
- 2024 10th December#2: More tweaks to requests of engines and combi returns. Now only combi return will change some parameters. Still figuring out the best solution for returns.
- 2024 11th December: Ok, requests are only sysex requests. No messing around with paramaters there now. Some manual labour required to get the names of engines, but at least you can trust them to be right after doing so.
- MERRY XMAS 2024 TO EVERYONE!!!!

"V-Verb Pro Panel Only.bpanelz"
- Necessary font 'ZXSpectrumJJK.ttf' for the Screendump suplied here also.
- 2024 16th November: Simplified version utilizing mainly the V-Verb's screendump function.
- 2024 17th November: Fixed the Edit Buffer sysex to modify only device id and nothing else when loading.

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

"MIDI Box SID panel for anyone else who might still use this old PIC and version 1
- 2024 July 28th: Tryed to rationalize the panel, so that others can use it too =)
- 2024 July 29th: Completing as much as possible and added a functionality to get all patch names from the bank sysex dump.
- 2024 August 03th: Bug in patch name fetcing fixed and function simplified by using only string.format function.
- 2024 August 09th: Bug fixes in sysex dump handling.

PS: Any PayPal donations to www.paypal.com/paypalme/janikasurinen are dearly appreciated =)