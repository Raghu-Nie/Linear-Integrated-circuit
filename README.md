# _experiment 2_:

## _basic differential amlifier design using LTspice._

## _AIM:_

To design differential amplifier and perform DC analysis,Ac analysis,Transient analysis And extract parameters
for the following specification;
VDD=3.2; P<=2.8mW; Vicm=1.6V; Vocm=1.7V; Vp=0.6
## _Components required:_
1)N-MOSFET(nmos4),

2)Resistors(3.42k(2),685ohm(1),

3)DC Power supply (3.2V,1.6V),

4)Current source (1 mA).

## _Theory_
A **Differential amplifier** takes two input signals and amplifies the difference between them, Ignoring anything that's the same in both signals. It's like tuning out the background noise and focusing on the unique parts of a conversation.This makes it super useful for things like measuring tiny differences in voltages in sensitive electronic equipment.
### The Differential amplifier circuit consists of:
*Two inputs V1 and V2,

*Two Resistors to set gain,

*Power supply, 

*An pair operational amplifer.

## _Working principle:_
The working principle of a differential amplifier can be broken down into a few key steps:

Input Signals: The amplifier receives two input signals, typically labeled as 𝑉1 and 𝑉2.

Difference Calculation: The amplifier focuses on the difference between these two input signals. In mathematical terms, it calculates the difference Vdiff=V1-V2.

Amplification: The amplifier then amplifies this difference by a certain gain factor, which determines how much the difference is magnified. The gain is usually denoted by A.

Output Signal: The amplified difference is then produced as the output signal,Vout=Ad(V1-V2).

## _Procedure:_

1.Open the LTspice software, merge the library file for getting accurate values of NMOS.

2.Select the components which are needed to us like for circuit 1 we need 3.2k & 685ohm resistors,2 CMOSN, three voltage sources(1.6v(2), 3.2v(1)),ground from the components list.

3.Place them all components in necessory way which is helpfull, connect all the components as in given circuit .

4.Link the specification of list of properties of mosfet like threshold voltage, temperature etc.

5.Lets do the DC Analysis first by opting a simulation, we get .op so after placing it we will get the values of it, thet will displayed.

6.After that lets take Transient analysis of 5m cycle so in input and output waveforms in 5 complete cycle, so here we get and seperate and combined waveforms of input and output.

7.For AC analysis, we should do some changes like converting DC SOURCE to sinosoidal waveform (1.6,50m,1k),after that select the AC simulation from the given options of simulation after giving values of (Decade,20,01,1T). So we will get a output after placing node to output waveform.

## _Circuit 01_:
![image](https://github.com/user-attachments/assets/d269d41b-939e-4ba6-bf9b-fb5dd19e4e67)

## _Calculation:_
Iss=p/vdd=2.8/3.2=0.875mA

ID1=ID2=Iss/2=0.875/2=0.4375mA

RD=VDD-Vocm/ID1=3.2-1.7/0.4375mA=3.42K

Rss=VP/Iss=0.6/0.875mA=685 ohms

## _DC Analysis:_

![image](https://github.com/user-attachments/assets/b2466887-bd0a-492c-b84d-08c4bbcf5edd)


Id1=0.4375mA

Id2=0.4375mA

Vocm1=1.7v

Vocm2=1.7v

Iss=0.875mA

## _Transient Anlysis :_

### _Input Waveform :_

![image](https://github.com/user-attachments/assets/0a98d3bc-d70d-456b-a37c-d77f75fa412f)

Vin=1.6-1.53

### _Output waveform :_

![image](https://github.com/user-attachments/assets/09a724ca-15f4-4e7f-b2c6-bbfc7dd1ad19)

Vout=1.75-1.67

### _combined output:_

![image](https://github.com/user-attachments/assets/54fd43a9-9da6-4076-9706-e16ed5518ee4)

Gain=1.75-1.67/1.6-1.53

=1.14 V.

**Gain in dB**=20*log(1.14)

=1.38dB

## _AC analysis :_
![image](https://github.com/user-attachments/assets/75fe4cd8-c9ba-469e-a49d-ac81bd2f433c)

## _Circuit 2 :_

## _DC Analysis:_

## _Transient Anlysis :_

### _Input Waveform :_

### _Output waveform :_

### _combined output:_

## _AC analysis :_

## _Circuit 03 :_

## _DC Analysis:_

## _Transient Anlysis :_

### _Input Waveform :_

### _Output waveform :_

### _combined output:_

## _AC analysis :_

## _Inference :_

**Differential Gain**: It's like a magnifying glass for differences. It makes the tiny differences between two signals much easier to see.

**Common-Mode Rejection**: Think of noise-canceling headphones. They block out background noise and let you hear the important sounds clearly.

**Biasing and Stability**: Imagine balancing a seesaw perfectly so it stays level. Proper biasing keeps everything balanced, and stability ensures it stays that way over time.

**Practical Limitations**: In real life, nothing is perfect. Small variations in components can lead to minor differences in performance, just like using slightly different ingredients in a recipe can change the final dish a bit.














