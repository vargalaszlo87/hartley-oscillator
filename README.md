# 🚀 hartley-oscillator

Hi guys! This is a beautiful **Hartley oscillator** with a Cascode amplifier stage. If you are an old gamer in RF world you've seen something like this before, but it's works really well with cascode amplifier. Worth a try!

For example you can use it as a local oscillator in a AM radio. (I use in that).

## The circuit

<img width="985" height="708" alt="image" src="https://github.com/user-attachments/assets/40f51c18-bdd2-4258-b09a-6d27808db605" />

### The first stage 

The hartley oscillator consists of an **tapped coil**, a **capacitor** and an active element (here is a FET). 

What are the conditions of oscillation? Simple:

- Positive feedback
- Loop gain is higher as 1.

**Positive feedback**

In this case the LC tank does not shift pahse at resonant frequency and the feedback comes from source, where the phase of signal matches the phase at the gate of FET. 🖤 **So that is a positive feedback!** 🖤

**Loop gain**

The full loop amplification (that consists of an open-loop amplification and the feedback factor) is higher as 1. **(A ⋅ β ≥ 1)** 

### The second stage

Why is this stage needed? The problem is the load impedance. The hartley oscillator (like most other types) is really sensitive to load impedance. If the impedance of the next stage is not suitable oscillator, for example the oscillation may stop or not start.

The cascode amplifier provides relative fix impedance for the output of hartley oscillator stage. If the load impedance is 50ohm, than the output signal level is Vp = 20mV (If a higher signal level is required due to low load, you can also insert a power amplifier stage at the end of the circuit.), but if the load is higher than 10k, the signal level is Vp = 450mV (that's good for me in this case)

## The charts of simulation

### The case of 2.28MHz

<img width="1918" height="917" alt="image" src="https://github.com/user-attachments/assets/9b65e1be-a69c-419c-be47-d8aea2fe6268" />


### The case of 900kHz

<img width="1919" height="916" alt="image" src="https://github.com/user-attachments/assets/84bf0bff-d2a3-4b39-8704-ce4b87e3a25a" />








