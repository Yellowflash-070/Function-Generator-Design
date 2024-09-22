# Function Generator Design
 A Sine, Square wave Function Generator utilising Schmitt Trigger and Wein Bridge Oscillator designed on PCB using EasyEDA.


## What is a Function Generator?

A function generator is an electronic test device or software that creates various electrical waveforms across a broad frequency spectrum. Commonly generated waveforms include sine, square, triangular, and sawtooth waves. These signals can be either continuous or one-time events, with the latter requiring an internal or external trigger.


## What is a Sine and Square Wave?

A **sine wave** is a smooth, continuous waveform that oscillates between positive and negative values in a repetitive manner. It is characterized by its smooth, symmetrical shape and is commonly found in many natural and engineered systems, such as sound waves and alternating current (AC) electricity. The mathematical representation of a sine wave is based on the sine function, and it has a uniform frequency and amplitude.

 
A **square wave**, on the other hand, is a waveform that alternates between two fixed levels, typically high and low, with sudden transitions. It has a non-smooth, rectangular shape with vertical edges. The signal remains at one constant value for a period of time, then instantly switches to the other value, making it ideal for representing binary signals in digital electronics.


## What is a Wien Bridge Oscillator?
A **Wien bridge oscillator** is a simple circuit for generating a sine wave. This simple circuit does not perform a conversion between one signal and another to provide a stable reference output waveform. Instead, this is a standalone oscillator that incorporates amplification with RC elements on a positive feedback loop to produce an output signal. The principle of operation in this circuit is deceptively simple and does not rely explicitly on resonance to produce an output sinusoidal waveform.

 
![Screenshot 2024-09-22 140426](https://github.com/user-attachments/assets/64d63d09-2e54-4a98-a8b1-750e0152cf65)

Fig 1: Wien Bridge Oscillator circuit diagram. [1]

 
## What is a Schmitt Trigger?

A **Schmitt Trigger** is a type of comparator circuit that exhibits hysteresis. It is used to convert a noisy or slowly changing input signal into a clean, fast-transitioning output signal. It has two distinct threshold voltage levels: an upper threshold (Vᴛ₊) and a lower threshold (Vᴛ₋). The output of the Schmitt Trigger changes state when the input crosses these thresholds.

**Input Signal > Upper Threshold (Vᴛ₊)** : The output switches to a high state (logic 1). <br>
**Input Signal < Lower Threshold (Vᴛ₋)** : The output switches to a low state (logic 0).  <br>
In between these thresholds, the output maintains its current state until the input crosses either of the thresholds.Here, the input signal can be referred to as a sine wave.

 ![schmitt trigger ckt diagram](https://github.com/user-attachments/assets/8e2a4f33-5a75-4362-851d-01346ff10de8)

Fig 2 : Schmitt Trigger circuit diagram and waveform [2].

 
**74HC14N Schmitt Trigger IC** is used to convert the sine wave obtained using the Wien Bridge oscillator into a square wave.

## Project Schematic
![Schematic_Frequency-Generator_2024-09-22](https://github.com/user-attachments/assets/8cbac623-6037-4b5f-83c9-694faaf6be4c)

## PCB Design (2D View)
![PCB_Final-PCB-Frequency-Generator_AM_2024-09-22(2)](https://github.com/user-attachments/assets/342d62d7-2ee5-4d61-a58a-95b608fd033f)

## PCB Design (3D View)
![Screenshot 2024-09-22 132840](https://github.com/user-attachments/assets/aa2c9298-efe7-40fd-aa79-717cdd1f8bb2)


**Note** : PCB designing is done in Easy EDA - an open source PCB Design tool. <br>
**Project Link:** https://oshwlab.com/originalmamba/Frequency-Generator


## References
1. https://www.researchgate.net/figure/Circuit-diagram-of-Schmitt-trigger-with-waveform_fig1_353878777
2. https://resources.pcb.cadence.com/blog/2020-designing-a-wien-bridge-oscillator-for-sine-wave-generation

