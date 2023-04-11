---
layout: page
title: AAIM
permalink: /AAIM/
---
The AAIM (Algorithmically Assisted Improvised Music) performance system is a portfolio of interconnectable algorithmic software modules, developed using Max/MSP, designed to facilitate improvisation and live performance of electronic music. In contrast to much of the current related research within the field of algorithmic performance systems, the AAIM system makes no attempt to generate new materials in a specific style or act as an autonomous improviser. Instead, the goal of the AAIM system is to facilitate improvisation through the variation and manipulation of precomposed materials entered by the user. By generating these variations algorithmically the system attempts to afford improvisers of computer music the ability to focus on macro elements of their performances, such as form, phrasing, texture, spatialisation, and timbre, while still enabling them to incorporate the melodic and/or rhythmic variations of a virtuosic instrumental improviser.

Example videos:
<iframe width="420" height="315"
src="https://www.youtube.com/embed/watch?v=eoj4ZDR5FSI&list=PLEZ5qOoNxYwVy1ynp8B4bTB01B2EqeKBM">
</iframe>

[MaxForLive Devices](https://drive.google.com/drive/folders/127ekOV4a4opyMvh4PmikDIRuewhGjmqj?usp=sharing)



<iframe width="420" height="315"
src="https://www.youtube.com/embed/watch?v=Fol9t-_k8ng">
</iframe>

AAIMduino.drums is a hardware based drum machine, which uses an Arduino Mega, 8 4*4 Matrix Keypads, and an assortment of switches, potentiometers, and push buttons, and the underlying logic of the AAIM.rhythmGen and AAIM.patternVary modules, to allow users to create, vary, and manipulate drum patterns. The keypads enable the user to enter patterns, which are then output as MIDI messages to any MIDI enabled sound generator.

For simplicities sake, AAIMduino.drums always considers the base i-o-i to be an 1/8 note. While the AAIM.rhythmGen and AAIM.patternVary modules allow users to work in any time signature, physical limitations require that AAIMduino.drums patterns are limited to a maximum of 16 beats per bar. The number of bars per phrase is also limited to 16. Similarly, the spatial and financial requirements of affording control over the chance for each individual i-o-i would have been astronomical, and as such an alternative method was devised, whereby a single potentiometer controls the centre peak, which is relative to the length of the i-o-i, and width of a gaussian curve, which in turn attenuates the chance of each i-o-i occurring. This feature allows swift changes from rhythmic lines using only very short i-o-i’s to rhythmic lines using only very long i-o-i’s, or anything in between, with only one gesture.

The AAIMduino.drums implementation also includes a potentiometer that controls the amount of ‘swing’ applied to the rhythm. This is achieved by considering every two base i-o-i’s to be equivalent to one 1/4 note. The position within each 1/4 note is then raised to some power, between 0.5 and 2 to achieve either a positive or negative displacement, and then converting this value back to a position relative to the base i-o-i. A further feature hardwired into the AAIMduino.drums results in an algorithmic splicing and re-arranging of the user defined pattern for the last bar of each phrase. This is achieved by first using the ‘genGrouping’ algorithm to generate a suitable grouping for the number of beats in the bar. The first group is then left unchanged, and for each subsequent group, a group of equal length is taken from the original pattern, each beginning on a random beat.
