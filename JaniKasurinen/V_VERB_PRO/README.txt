"V-Verb Pro FULL.bpanelz"
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
- 2026 13th February: Now should fetch Combi number from Edit Buffer dump. Fully reformatted the arrangement of panel.