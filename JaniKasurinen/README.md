"EX5R Switches.bpanelz" is propably at stage of final version, but I might in future add some editing functions there.
The EX5/7 parameter sysex bug made some difficulties in making the panel, but it is actually in case of this hardware pretty useless sysex-implementation after all and new implementation has even removed parameter request totally from it's documentation.

"YAMAHA A4000 SAMPLER MANIPULATOR.bpanelz" is now at current final state and wont likely to be edited soon again.
- Update 2024 22th April 04:25 GMT: FIXED file handling bugs and removed PC hanging os.time function.
- NOTE!: After experimenting with midi dumps you must send all data in this order back to A4000: 
"wavedata" - "sample bulk" - "sample bank dump" - "Program dump".
- I gave up trying to calculate the right checksum so only unmodified midi dumps will succeed hence the checksum is incorrect otherwise and will fail the dumps.
- UPDATE 23th April 2024: Added more features of which most usefull is the objectlist request.
- UPDATE 23th April 2024 #2: Uploaded YAMAHA A5000 panel version with correct "family device code" ASCII "5" = 35h = 53 incomparison A4000 ASCII "4" = 34h = 52.

"V-Verb Pro FULL.bpanelz" is also a work in process as it only receives few first engine A model modulators fully from the sysex-dump.
 - On 2024 20th April FIXED file handling bugs and removed PC hanging os.time function.
 
"Korg Z1 Editor.bpanelz" is still greatly work in process stage and does NOT have all the modulators, but file loading saving and storing functions fully.
 
"Korg Prophecy Editor.bpanelz" has surely still many bugs and only few modulators are now fetched from the program bulk dump, but likewise to Z1 panel file handling and sysex-dumping works fully already.

- Korg Prophecy and Z1 panels are done from basis of this panel: https://ctrlr.org/710/ done by person with signature "jms" on CTRLR.ORG
- Huge thank for the initial work done back in 2013 =)!

PS: Any PayPal donations to www.paypal.com/paypalme/janikasurinen are dearly appreciated =)