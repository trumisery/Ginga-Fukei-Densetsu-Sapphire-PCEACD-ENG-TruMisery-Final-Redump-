GINGA FUKEI DENSETSU SAPPHIRE
English Translation - Final-Redump

Translation by: TruMisery

Release tag:
Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump]

ABOUT THIS RELEASE
------------------
An English translation based on the verified Japanese Redump release of
Ginga Fukei Densetsu Sapphire for the PC Engine Arcade CD-ROM2.

All text has been translated into English, including the system card
warning. Original Japanese audio remains; this is not an English dub.

DIFFERENCES FROM THE JAPANESE REDUMP
-----------------------------------
- Tracks 02 and 17 contain the English translation and associated code
  changes.
- All 15 audio tracks (01, 03-16) remain byte-for-byte identical to Redump.
- The 17-track layout, track lengths, pregaps, and catalog value are kept.
- Files use the Final-Redump release tag and a matching multi-file CUE.

"Final-Redump" means the translation is based on the verified Redump dump.
The altered data tracks cannot match the original Japanese checksums.
All audio tracks still match. Use the expected output hashes below to
verify the translated data tracks.

WHAT YOU NEED
-------------
1. The untranslated Japanese Redump BIN/CUE set, with all 17 track BINs.
   Reference: http://redump.org/disc/60904/
   Title: Ginga Fukei Densetsu Sapphire (Japan)
   Serial: HCD5080
   Total BIN size: 407,968,512 bytes (173,456 raw 2,352-byte sectors).
2. Both xdelta patches: _track02.xdelta and _track17.xdelta.
3. An xdelta-compatible patching tool.
4. Approximately 390 MiB of additional free space for the patched BINs.
5. An emulator or hardware setup with the Arcade Card support required
   by the game.

Use the original split-track dump, not a previously translated image,
CHD, compressed audio conversion, or single-file ISO as direct input.
The original track filenames follow this pattern:
Ginga Fukei Densetsu Sapphire (Japan) (Track 01).bin
...
Ginga Fukei Densetsu Sapphire (Japan) (Track 17).bin

REQUIRED ORIGINAL JAPANESE TRACK HASHES
---------------------------------------
These SHA-1 hashes match Redump entry 60904. Sizes are in bytes.
Verify your source files against these hashes before patching.

Track  Size        SHA-1
01       7914480   66940b3369f008f3a21c7029e785d12ac0392907
02      18402048   43c85bf6a9a71cd2ffd8cb71ec3296fbc73172d1
03      43003968   2e195dbf52137cce5c5225ca7c13b454d1d4c247
04      42799344   ac588d4961de3e0e6875d710d2f660e231370722
05      42651168   011b7a5a5ffa521976e405f6c8a5c1e640231f01
06      42733488   740d364f06999ecc0bd4ac6b2726e4038dc583ea
07      42813456   351e967dacd99ff4a72d80c52c2af17b2ccd45f4
08      21459648   09e36ec83f59a284ea2e5db5d40fec61a2823346
09      21694848   88951b76951a9b7be3a8621de8ecb6ea3e720c05
10      21433776   8e031c048355f1504c522a7c2d3e3154f93e2af7
11       5884704   e243b935363f2e806e300981fc55c994608eda68
12       5785920   f85c762df48c88b412808ca735e88c8584bb90ce
13      10882704   f02ef760e43622f0dd62284a10202f8ddd8ffa02
14      12717264   0430c2142c230ecc14e0cb62031c9ee3857f68ad
15      15814848   0ddb8899ed3e83d701a9e5e87b933f7a36a0b927
16      33925248   f99dbfc5d2375eedbc799d5e52033ac7ab009494
17      18051600   a52aa2292cca6e23668ce2d2af6f62dff120440c

HOW TO APPLY THE PATCHES
------------------------
1. Verify your original Japanese tracks against the source hashes below.
   Keep the original set as a backup and create a separate output folder.

2. Open your xdelta patching tool and select its Apply/Decode function.
   For Track 02, select:

   Patch:
   Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump]_track02.xdelta

   Source/original file:
   Ginga Fukei Densetsu Sapphire (Japan) (Track 02).bin

   Output file:
   Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump]_track02.bin

3. Apply the second patch using:

   Patch:
   Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump]_track17.xdelta

   Source/original file:
   Ginga Fukei Densetsu Sapphire (Japan) (Track 17).bin

   Output file:
   Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump]_track17.bin

4. Copy all original audio tracks (01 and 03-16) into the output folder.
   Do not patch or convert them. Rename each copy using this pattern,
   replacing NN with its two-digit track number:

   Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump]_trackNN.bin

5. Use a CUE whose FILE entries match these renamed BINs exactly. If you
   already have the matching Final-Redump CUE, place it in the output folder.
   Otherwise, copy the original Japanese CUE, change only its quoted FILE
   names to the new names, and save it as:

   Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump].cue

   Keep CATALOG, TRACK, AUDIO/MODE1/2352, and INDEX lines unchanged.
   For example, the original Track 02 FILE line becomes:

   FILE "Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump]_track02.bin" BINARY

6. Verify the patched data tracks against the expected output hashes below.
   The audio tracks must still match the original source hashes.

7. Load the translated CUE in your emulator or use it when preparing the
   disc for compatible hardware. Keep the CUE and all 17 BINs together.

Each patch applies only to its matching data track. If a patching tool
reports a source/checksum error, check that you selected the correct
original track and that its hash matches. Do not force a mismatched patch.

EXPECTED TRANSLATED DATA TRACK HASHES
-------------------------------------
SHA-1:
Track 02: f49328d9264577d2b225718783ca794c81ad4682
Track 17: 47bdf2bca3a4ba47216174d7b84462636e1a9eaa

All audio tracks retain the original hashes listed above.

TESTED SETUPS
-------------
Release testing reported by TruMisery:
- GearGrafx
- PC Engine + SuperHD System3 Pro
- Original Turbo Duo with an Arcade Card Duo

CHEAT CODE - INFINITE HEALTH
----------------------------
At the title screen, enter:

UP, UP, UP, DOWN, DOWN, DOWN, RUN

Release the direction between presses. RUN is the seventh input and is
required to complete the sequence. The cheat remains present in both
translated data tracks. The six directional presses alone do not finish
activation.

PATCH FILES
-----------
Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump]_track02.xdelta
Ginga Fukei Densetsu Sapphire [PCEACD][ENG][TruMisery][Final-Redump]_track17.xdelta

The patches do not contain the full game. The original untranslated
Redump files are required to reconstruct the translated release.

CREDITS
-------
Translation by: TruMisery
