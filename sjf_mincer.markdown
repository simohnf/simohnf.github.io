---
layout: page
title: sjf_mincer
permalink: /plug-ins/sjf_mincer/
---
<img width="876" alt="Screenshot 2023-11-08 at 16 11 26" src="https://github.com/simohnf/simohnf.github.io/assets/12850558/2dd2b0ca-5938-4048-8ad3-d0e2724da8a6">


sjf_mincer is a granular delay plugin that can apply random playback variations and effects to individual grains, enabling the creation of a wide variety (of mostly chaotic ;) ) textures. 

Delay time and grain rate can either be set in milliseconds or synced to the session tempo, as can random variations applied to the delay time.
Grains can be triggered at different playback speeds (to achieve pitch shifting), in reverse, and repeated. 
Up to four additional grains can be triggered to create polyphonic textures.
Crosstalk feeds the output of the left channel into the right channel and vice versa.
The probability of triggering grains can be changed to create a more sparse texture.
Individual grains can be played in reverse, and grains can be repeated to create various sonic results.

There are three effect processors that are applied to individual grains:

1) Bitcrushing and samplerate reduction

2) Ring modulation

3) Lowpass/highpass/bandpass filter


The frequency of both the ring modulator and filter can also be randomly varied on a grain-by-grain basis.

There are three output modes available:

1) Mix: mixes the output of the delay with the dry signal

2) Insert: is dependent on the density parameter and will insert the wet signal whenever a grain is triggered and otherwise the dry signal will be output

3) Gate: is also dependent on the density parameter but will only output the results of the grain engine. This is essentially the same as the mix output mode with the mix parameter set to 100



---

### Audio Samples
Simple major scale
<audio controls>
<source src="/MP3s/majorScale [2023-11-08 162917].mp3" type="audio/mp3">
</audio>


Simple major scale minced (with two harmonies of a perfect fifth and one octave above)
<audio controls>
<source src="/MP3s/majorScaleMinced1.mp3" type="audio/mp3">
</audio>

Simple major scale minced (with all three effects processors)
<audio controls>
<source src="/MP3s/majorScaleMinced2.mp3" type="audio/mp3">
</audio>


Simple major scale minced (with asynchronous delay variations)
<audio controls>
<source src="/MP3s/majorScaleMined3.mp3" type="audio/mp3">
</audio>



Basic drum beat
<audio controls>
<source src="/MP3s/DrumBeat.mp3" type="audio/mp3">
</audio>


Basic drum beat minced to create random variations
<audio controls>
<source src="/MP3s/drumBeatMinced1.mp3" type="audio/mp3">
</audio>

Basic drum beat minced (with all effects and asynchronous delay variations)
<audio controls>
<source src="/MP3s/drumBeatMinced2.mp3" type="audio/mp3">
</audio>

---


### [[Mac OS Installer (VST3 and Audio Unit)]](https://drive.google.com/file/d/1efOEqh4wgEyUMW7A5eY9BZ_-RFV2pIR6/view)
