# moody-ds

A touchscreen analog style synth and groovebox for the Nintendo DS.

by HobbyChop (hobbychop.com)

Turn your Nintendo DS into a pocket synthesizer. Sculpt sounds with your finger on the filter pad, build basslines and beats on the step sequencer, chain them into a full song, and sync it all to your gear. moody-ds is made to be picked up and played.

## The sound

moody-ds is a virtual analog synth. It has the warm, hands on character of a classic subtractive synthesizer, an oscillator running into a filter into an envelope, shaped with an LFO and a touch of effects, recreated in software on your DS. There is no analog circuitry inside a DS, so think of "analog" here as the sound and the feel rather than the wiring. If you love that fat, filtered, knob twiddling vibe, you will feel right at home.

## What you can do

**Play**

* A touch keyboard right on the screen, so you can perform by hand.
* Press B to move through the voice modes, from single notes to full chords.

**Shape**

* A filter pad you sweep with your finger for instant movement and squelch.
* Oscillator, envelope, and LFO pages to dial in your tone.
* Onboard delay and chorus for space and width.

**Sequence**

* A 16 step sequencer with adjustable length and swing for groove.
* An arpeggiator that turns your held notes into rolling patterns.
* A pattern bank that stores 16 of your patterns.
* A song mode that chains patterns into a full arrangement.

**Save**

* 16 preset slots, each one a snapshot of your whole sound and its sequence.
* Name your presets so you can find them again.
* Your setup also saves itself, so moody-ds powers up right where you left off.

**Sync**

* Play moody-ds from any MIDI keyboard, controller, or computer.
* Lock the sequencer and song to your DAW or hardware clock so everything stays in time.
* Or let moody-ds lead and send clock to the rest of your setup.
* Works great with a DAW, and with an arduinoboy or LSDJ rig.

## Free demo and full version

The free demo is the real instrument, not a teaser. You get the complete sound engine, the effects, the sequencer, song mode, and the touch keyboard, so you can sit down and make music with it right away.

The full version adds the things you keep and connect:

* Saving and loading your presets.
* The automatic save of your working setup.
* MIDI, so you can play from outside gear and sync clock in or out.

Get the full version at hobbychop.com.

## What you need

* A Nintendo DS or DS Lite with a flashcart, to run the game from an SD card.
* An SD card, if you want to save your presets and setup (full version).
* For MIDI, the mDS cartridge that plugs into the second cart slot. Because it uses that slot, MIDI works on the original DS and DS Lite. The DSi and 3DS do not have the slot, but the synth, sequencer, and song mode still play on any DS that can run the game.

## Getting started

1. Copy the game file onto your flashcart and launch it.
2. To use MIDI (full version), put the mDS cartridge in the second slot and tap A to connect it. The settings page shows CART OK when it is ready. Then plug in your MIDI.
3. Tap the tabs along the top to move between pages. Drag the pad and sliders to shape your sound, and tap the keyboard to play.

## The pages

Tap the tabs across the top of the touch screen:

* FILT: the filter pad you sweep with your finger.
* ENV: how each note swells and fades.
* MOD: the LFO and movement.
* OSC: the raw oscillator tone.
* SEQ: the 16 step sequencer.
* SONG: chain your patterns into a song.
* PAT: your bank of saved patterns.
* PRE: your saved presets.
* FX: delay and chorus.
* SET: MIDI settings.

Press B at any time to switch between the voice modes.

## A note on MIDI sync

Turn on Clock In to follow an external clock. moody-ds starts right on the beat and stops cleanly when the clock stops. Turn on Clock Out to lead instead, sending clock and transport to the rest of your rig.

If you sync from an arduinoboy or LSDJ setup, moody-ds quietly ignores the extra start note those rigs send alongside their clock, so you get clean timing with no surprise drone. Notes you actually play still come through as normal.

## Building from source

For developers. You will need devkitPro with devkitARM and libnds installed. From the ds-rom folder:

* `make` builds the full version (moody-ds.nds).
* `make DEMO=1` builds the free demo (moody-ds-demo.nds).

Run `make clean` when switching between the two, so it rebuilds completely.

## Credits and license

moody-ds is a HobbyChop release, grown from the sDS synth project. The free demo is fine to share. Please do not redistribute the full version. The names moody-ds, sDS, and mDS belong to the author.

Make all the music you want with moody-ds and release it freely. For commercial or licensing questions, get in touch at hobbychop.com.
