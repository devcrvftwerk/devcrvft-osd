# devcrvft OSD

Custom analog OSD fonts for Betaflight whoops, by **devcrvft** (KVOID). Each theme is a full
256-character MAX7456 font (`.mcm`) with its own boot logo, plus the OSD element positions
it was designed around.

Preview images are simulated analog goggle frames, not captures. The real thing looks softer.

## WHALECRVFT (HELLO, GROUND.)

The whale boot logo over the devcrvft letters, a bong battery, Dead Air signal icons and Sky Mutant clocks.

<img src="themes/whalecrvft/boot.png" width="320" alt="WHALECRVFT (HELLO, GROUND.) boot"> <img src="themes/whalecrvft/cruise.png" width="320" alt="WHALECRVFT (HELLO, GROUND.) cruise"> <img src="themes/whalecrvft/mid-pack.png" width="320" alt="WHALECRVFT (HELLO, GROUND.) mid-pack">

Font: [`themes/whalecrvft/whalecrvft.mcm`](themes/whalecrvft/whalecrvft.mcm) | layout: [`themes/whalecrvft/layout.txt`](themes/whalecrvft/layout.txt)

## VOID MOTH

Same HUD as WHALECRVFT, with the eye-spot moth and moon boot logo.

<img src="themes/void-moth/boot.png" width="320" alt="VOID MOTH boot"> <img src="themes/void-moth/cruise.png" width="320" alt="VOID MOTH cruise"> <img src="themes/void-moth/mid-pack.png" width="320" alt="VOID MOTH mid-pack">

Font: [`themes/void-moth/void-moth.mcm`](themes/void-moth/void-moth.mcm) | layout: [`themes/void-moth/layout.txt`](themes/void-moth/layout.txt)

## SKY MUTANT

The Smiley Patch lives in your goggles: it grins on a full pack and melts when you push it too far.

<img src="themes/sky-mutant/boot.png" width="320" alt="SKY MUTANT boot"> <img src="themes/sky-mutant/cruise.png" width="320" alt="SKY MUTANT cruise"> <img src="themes/sky-mutant/mid-pack.png" width="320" alt="SKY MUTANT mid-pack">

Font: [`themes/sky-mutant/sky-mutant.mcm`](themes/sky-mutant/sky-mutant.mcm) | layout: [`themes/sky-mutant/layout.txt`](themes/sky-mutant/layout.txt)

## ROUND 1

Every pack is a fight and gravity is the opponent: life bar, round timer, K.O.

<img src="themes/round-one/boot.png" width="320" alt="ROUND 1 boot"> <img src="themes/round-one/cruise.png" width="320" alt="ROUND 1 cruise"> <img src="themes/round-one/mid-pack.png" width="320" alt="ROUND 1 mid-pack">

Font: [`themes/round-one/round-one.mcm`](themes/round-one/round-one.mcm) | layout: [`themes/round-one/layout.txt`](themes/round-one/layout.txt)

## RECOVERY MODE

The whoop boots into KVOID//OS and every readout is a terminal window over the video.

<img src="themes/recovery-mode/boot.png" width="320" alt="RECOVERY MODE boot"> <img src="themes/recovery-mode/cruise.png" width="320" alt="RECOVERY MODE cruise"> <img src="themes/recovery-mode/mid-pack.png" width="320" alt="RECOVERY MODE mid-pack">

Font: [`themes/recovery-mode/recovery-mode.mcm`](themes/recovery-mode/recovery-mode.mcm) | layout: [`themes/recovery-mode/layout.txt`](themes/recovery-mode/layout.txt)

## Install

**Analog only** (a MAX7456-style OSD chip). DJI, Walksnail and HDZero use different font formats.

1. **Font:** Betaflight Configurator (or the Betaflight App) -> OSD tab -> **Font Manager** ->
   load the `.mcm` file -> **Upload font**. Then power-cycle the quad from a battery.
2. **Layout (optional):** the themes were laid out for NTSC (30 x 13). Paste the `set` lines
   from `layout.txt` into the CLI tab, then type `save`. They only move the elements the theme
   uses; anything else you have on screen stays where it is. Some layouts also set a pilot or
   craft name: edit those lines to your own before pasting.

Back up first: in the CLI, `diff all` and save the output somewhere.
