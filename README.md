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
A **Differential amplifier** takes two input signals and amplifies the difference between them, Ignoring anything that's the same in both signals. It's like tuning out the background noise and focusing on the unique parts of a conversation.This makes it super useful for things like measuring tiny differences in voltages in sensitive electronic equipment.
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

##Procedure:

1.Open the LTspice software, merge the library file for getting accurate values of NMOS.

2.Select the components which are needed to us like for circuit 1 we need 3.2k & 685ohm resistors,2 CMOSN, three voltage sources(1.6v(2), 3.2v(1)),ground from the components list.

3.Place them all components in necessory way which is helpfull, connect all the components as in given circuit .

4.Link the specification of list of properties of mosfet like threshold voltage, temperature etc.

5.Lets do the DC Analysis first by opting a simulation, we get .op so after placing it we will get the values of it, thet will displayed.

6.After that lets take Transient analysis of 5m cycle so in input and output waveforms in 5 complete cycle, so here we get and seperate and combined waveforms of input and output.

7.For AC analysis, we should do some changes like converting DC SOURCE to sinosoidal waveform (1.6,50m,1k),after that select the AC simulation from the given options of simulation after giving values of (Decade,20,01,1T). So we will get a output after placing node to output waveform.

## Circuit 01:
![image](https://github.com/user-attachments/assets/d269d41b-939e-4ba6-bf9b-fb5dd19e4e67)

## Calculation:
Iss=p/vdd=2.8/3.2=0.875mA

ID1=ID2=Iss/2=0.875/2=0.4375mA

RD=VDD-Vocm/ID1=3.2-1.7/0.4375mA=3.42K

Rss=VP/Iss=0.6/0.875mA=685 ohms

## DC Analysis:

![image](https://github.com/user-attachments/assets/5813c145-c168-4ae1-affc-d8613b681eac)

Id1=0.4375mA

Id2=0.4375mA

Vocm1=1.7V

Vocm2=1.7V

Iss=0.875mA

## Transient Anlysis :
### Input Waveform :

![image](https://github.com/user-attachments/assets/0a98d3bc-d70d-456b-a37c-d77f75fa412f)





