# experiment 2:basic differential amlifier design using LTspice.
## AIM:
To design differential amplifier and perform DC analysis,Ac analysis,Transient analysis And extract parameters
for the following specification;
VDD=3.2; P<=2.8mW; Vicm=1.6V; Vocm=1.7V; Vp=0.6
## Components required:
1)N-MOSFET(nmos4),

2)Resistors(3.42k(2),685ohm(1),

3)DC Power supply (3.2V,1.6V),

4)Current source (1 mA).

## Theory
A differential amplifier takes two input signals and amplifies the difference between them, Ignoring anything that's the same in both signals. It's like tuning out the background noise and focusing on the unique parts of a conversation.This makes it super useful for things like measuring tiny differences in voltages in sensitive electronic equipment.
### The Differential amplifier circuit consists of:
*Two inputs V1 and V2,

*Two Resistors to set gain,

*Power supply, 

*An operational amplifer.

## Working principle
The working principle of a differential amplifier can be broken down into a few key steps:

Input Signals: The amplifier receives two input signals, typically labeled as 𝑉1 and 𝑉2.

Difference Calculation: The amplifier focuses on the difference between these two input signals. In mathematical terms, it calculates the difference Vdiff=V1-V2.

Amplification: The amplifier then amplifies this difference by a certain gain factor, which determines how much the difference is magnified. The gain is usually denoted by A.

Output Signal: The amplified difference is then produced as the output signal,Vout=Ad(V1-V2).
