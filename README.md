## Syntheseyeser

Syntheseyeser is a 3D soundwave visualizer accompanied with a basic web based synthesizer and music player. It is written in Javascript using [Three.js](https://github.com/mrdoob/three.js) for 3D rendering and [Tone.js](https://github.com/Tonejs/Tone.js/) to create the built in synthesizer and music player.

![syntheseyeser](https://github.com/chrishakos/Syntheseyes/blob/master/syntheseyeser.jpg)


### Waveform

The waveform illustrates an audio sample analyzed with a bitrate 128 KB/s animated at a rate of 60 FPS. The sound wave is visualized using a 128 x 32 grid of spherical objects, taking in the waveform analysis (an array of decibel values) and manipulating the height (y-value) of each spherical object based on the given value at said index position of the array. Each line of spherical objects represents the array of analyzed values and is visualized 32 times across the z-axis to create the 3 dimensional visualization.

#### Waveform Colors

The waveform colors are manipulated based on the decibel values given in the array to create a more engaging user experience. Using a math equation and comparator operator, each decibel value in the waveform analysis array is compared and then the color of that spherical object is changed accordingly.

### Synth

A basic polyphonic synthesizer is built in with a triangular waveform oscillator. The synth can be played by clicking on the keys displayed on the keyboard, or by pressing keyboard keys. The keyboard keys are mapped exactly the same as a standard Digital Audio Workstation (pictured below).
!!![keymap](https://github.com/chrishakos/Syntheseyes/blob/master/keymap.png)
