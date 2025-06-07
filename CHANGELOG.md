======================================================
koboldplayermodelport-v1.2.15-rur

Kobold Player Model Port - Rur Edition
version 1.2.15-rur

Original Mod Developed by: Soi
1.19-1.20 Port by: Caliber
1.20 "Rur Edition" by: Xeirla (Rur)

CHANGES FROM MAIN BRANCH
======================================================

Recent changes first:
----------------------------------
# :: 2025 June 7
## Overall
- Adjusted `Pour`, `Pour-fp`, and `holdbothhands-fp` animations manually. 
    - `Pour` copied from Kobold Player Model Port v1.2.14
    - `Pour-fp` values adjusted manually from vanilla
    - `holdbothhands-fp` values adjusted manually from vanilla
    - Resulting animations are much less pronounced to avoid clipping through the player's viewport, and to make the shoulders less visible.
    
----------------------------------
# :: 2025 June 3
## Overall
- Cleaned up various clothing patch JSON files to resolve all error log output.
    - This should result in slightly faster loads, and also not write 500,000 lines of pointless json info to disk!!
- Moved `kobold-comment`s to a dedicated file to avoid logging them as errors.
- Moved the above and other documentation files to `/docs` 

----------------------------------
# :: 2025 June 2
## Overall
- Rewrite of `/home/xeirla/Programming/VS Kobold Model Docs/koboldplayermodelport-v1.2.15-rur/assets/koboldplayermodelport/patches/game-shapes-entity-humanoid-seraph-faceless.json`
    - All animations have been reimplemented, including new 1.20 animations
    - Filsesize reduced from 1.4MB -> 1.0MB
    - Details have been documented in the accompanying file and in the `"kobold-comment"`s of the file itself!
- Going forward this should futureproof all Kobold animations against base game updates
    (they should never break again, with the exception of major API updates that change how animations are read entirely, which is highly unlikely)
- `modinfo.json` updated

----------------------------------

# :: 2025 May 27
## Overall
- 'source files' directory and contents copied from 1.2.14
- Added CHANGELOG.txt
- Majority of mod is based on 1.2.14 version, except where specified in this changelog.
    - This is due to 1.2.15 breaking various clothing .json files, but implementing boat animations (partially)

## /assets/koboldplayermodelport/patches/game-shapes-entity-humanoid-seraph-faceless.json
- Copied from 1.2.15 version (taken down from mod-db?)
- Removed 1000+ lines removing the same "/animation/0" repeatedly only to literally just replace it immediately after.
- Changed all instances of "add" to "replace" (fixes smithing animations and behaviour)

----------------------------------
# :: 2025 May 25
# /assets/koboldplayermodelport/patches/game-shapes-entity-humanoid-seraph-faceless.json
- Removed 1000+ lines removing the same "/animation/0" repeatedly only to literally just replace it immediately after.


----------------------------------
End of Changes
