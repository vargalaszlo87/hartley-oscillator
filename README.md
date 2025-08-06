# 🚀 hartley-oscillator

Hi guys! This is a beautiful **Hartley oscillator** with a Cascode amplifier stage. If you are an old gamer in RF world you've seen something like this before, but it's works really well with cascode amplifier. Worth a try!

For example you can use it as a local oscillator in a AM radio. (I use in that).

## The circuit

<img width="916" height="685" alt="image" src="https://github.com/user-attachments/assets/9cb8ce1c-2d57-4b91-9160-873c74399f70" />

### The first stage 

The hartley oscillator consists of an **tapped coil**, a **capacitor** and an active element (here is a FET). 

What are the conditions of oscillation? Simple:

- Positive feedback
- Loop gain is higher as 1.

**Positive feedback**

In this case the LC tank does not shift pahse at resonant frequency and the feedback comes from source, where the phase of signal matches the phase at the gate of FET. 🖤 **So that is a positive feedback!** 🖤

**Loop gain**

The full loop amplification (that consists of an open-loop amplification and the feedback factor) is higher as 1. **(A ⋅ β ≥ 1)** 

