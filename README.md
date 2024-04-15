# YaVCF: MS20-inspired resonant VCF

My take on the MS20 voltage-controlled filter - if you want squally, resonant acid sounds then this may well be right up your alley.

This is a redesigned version of the old 4HP module which is a bit friendlier for those who insist on running ludicrously shallow cases. 
As a result, the module is now 6HP wide and only 15mm deep (excluding power cable - approximately 25mm with it attached)

Built around an LM13700 transconductance amplifier, this filter uses a pair of red LEDs in the feedback path, rather than the string of diodes 
in the original Korg design, to make things a little more ... interesting, but other than that it's a straight-up lifting of the classic MS20 design.
Note, however, that this module does not have voltage-controlled resonance (but my diode filter does)

Has both low-pass and high-pass inputs, which should be pretty self-explanatory and there's nothing at all to stop you using them both together if 
you want a freaky bandpass response.

# Build notes

The build is fairly straightforward - if you bought the PCB/panel set then the surface-mount components will be pre-soldered for you.
Some points to note:

- Take care of the polarity of electrolytic capacitors and diodes. For diodes, the ring on the silkscreen corresponds to the cathode end (usually marked by a black band on the diode body)
- The cathodes (short leg) of the LEDs, D1 and D2, should go through the square pads.
- C2 and C5 are the actual filter capacitors. 1nF is a representative value and what I use in the pre-built modules. Smaller values will result in a 'sharper' sound. Values greater than around 3.3nF will result in a 'muddy' sound. Use film capacitors - ceramics will work, but may result in an altered sound/response.
- For reasons of stability, C8 should _always_ be a film/PET capacitor.
- The feedback LEDs, D1 and D2, can be whatever you like - I recommend red LEDs with a relatively low (1.8-2.0V) forward voltage.
- Resistors R22 and R25 control the cutoff frequency range. Again, 47k is a representative value - anything between 33k and 56k will also work (I don't recommend going outside this range)
- I don't bother making sure that the transistors, Q1 and Q2, match - if matched transistors are your thing, go nuts.
- All pots are linear taper - I recommend 100k, but 50k is OK as well. Anything with an Alpha-compatible footprint will work 
