# _experiment 2_: 

## Basic Differential amlifier design using LTspice.

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
A *Differential amplifier* takes two input signals and amplifies the difference between them, Ignoring anything that's the same in both signals. It's like tuning out the background noise and focusing on the unique parts of a conversation.This makes it super useful for things like measuring tiny differences in voltages in sensitive electronic equipment.

### The Differential amplifier circuit consists of:

*Two inputs V1 and V2,

*Two Resistors to set gain,

*Power supply, 

*pair operational amplifers.

## Working principle:

The working principle of a differential amplifier can be broken down into a few key steps:

Input Signals: The amplifier receives two input signals, typically labeled as 𝑉1 and 𝑉2.

Difference Calculation: The amplifier focuses on the difference between these two input signals. In mathematical terms, it calculates the difference Vdiff=V1-V2.

Amplification: The amplifier then amplifies this difference by a certain gain factor, which determines how much the difference is magnified. The gain is usually denoted by A.

Output Signal: The amplified difference is then produced as the output signal,Vout=Ad(V1-V2).

## Procedure:

1.Open the LTspice software, merge the library file for getting accurate values of NMOS.

2.Select the components which are needed to us like for circuit 1 we need 3.2k & 685ohm resistors,2 CMOSN, three voltage sources(1.6v(2), 3.2v(1)),ground from the components list.

3.Place them all components in necessory way which is helpfull, connect all the components as in given circuit .

4.Link the specification of list of properties of mosfet like threshold voltage, temperature etc.

5.Lets do the DC Analysis first by opting a simulation, we get .op so after placing it we will get the values of it, thet will displayed.

6.After that lets take Transient analysis of 5m cycle so in input and output waveforms in 5 complete cycle, so here we get and seperate and combined waveforms of input and output.

7.For AC analysis, we should do some changes like converting DC SOURCE to sinosoidal waveform (1.6,50m,1k),after that select the AC simulation from the given options of simulation after giving values of (Decade,20,01,1T). So we will get a output after placing node to output waveform.

## _Circuit 01_:
![image](https://github.com/user-attachments/assets/d269d41b-939e-4ba6-bf9b-fb5dd19e4e67)

## Design:

Iss=p/vdd=2.8/3.2=0.875mA

ID1=ID2=Iss/2=0.875/2=0.4375mA

RD=VDD-Vocm/ID1=3.2-1.7/0.4375mA=3.42K

Rss=VP/Iss=0.6/0.875mA=685 ohms

W=2.52uM

L=180nM

## _DC Analysis:_

![image](https://github.com/user-attachments/assets/b2466887-bd0a-492c-b84d-08c4bbcf5edd)


Id1=0.4375mA

Id2=0.4375mA

Vocm1=1.7v

Vocm2=1.7v

Iss=0.875mA

## _Transient Anlysis :_

### _Input Waveform :_

![image](https://github.com/user-attachments/assets/5d232e44-4c18-45eb-8161-b800261d468b)


**Vin=1.65-1.55**

### _Output waveform :_

![image](https://github.com/user-attachments/assets/91855cd9-7d20-4506-a04b-acfb405a72ad)


**Vout=1.86-1.53**

### _combined output:_

![image](https://github.com/user-attachments/assets/0f77d9af-e1f6-472d-9009-30951e30ef06)

## Gain calculation

**Gain**=1.86-1.53/1.65-1.55

=3.3 V.

**Gain in dB**=20*log(3.3)

=10.52 dB.

## _AC analysis :_

![image](https://github.com/user-attachments/assets/7efa0e16-fce7-4db3-ae4b-61786fb4e06a)

## _Circuit 2 :_

![image](https://github.com/user-attachments/assets/678f149c-2c11-4c6e-ad7d-e1bfc3d018a1)

## Design

P=2.8 mV

Iss=p/vdd=2.8/3.2=0.875mA

ID1=ID2=Iss/2=0.875/2=0.4375mA

RD=VDD-Vocm/ID1=3.2-1.7/0.4375mA=3.42K

Rss=VP/Iss=0.6/0.875mA=685 ohms

W=2.52uM

L=180nM


## _DC Analysis:_

![image](https://github.com/user-attachments/assets/c269a94b-40ac-4f83-8838-5e88fd86d61d)

## _Transient Anlysis :_

### _Input Waveform :_

![image](https://github.com/user-attachments/assets/03ed9117-4220-46c1-b127-ed29d7569cf2)

**Vin=1.65-1.55**

### _Output waveform :_

![image](https://github.com/user-attachments/assets/3808525e-5669-40e7-946c-a83d29311733)

**Vout=1.86-1.53**

### _combined output:_

![image](https://github.com/user-attachments/assets/f5c6b038-13a0-4e66-ac01-be159273969b)

## Gain calculation

**Gain**=1.86-1.53/1.65-1.55

=3.3 V.

**Gain in dB**=20*log(3.3)

=10.52 dB.


## _AC analysis :_

![image](https://github.com/user-attachments/assets/0cc2a50d-8f14-4daf-baa8-f696ee4bd5ee)


## _Circuit 03 :_

![image](https://github.com/user-attachments/assets/1e24bc6a-5a43-4350-86ea-b6bff523a677)

## Design

P=2.8 mV

Iss=p/vdd=2.8/3.2=0.875mA

ID1=ID2=Iss/2=0.875/2=0.4375mA

RD=VDD-Vocm/ID1=3.2-1.7/0.4375mA=3.42K

Rss=VP/Iss=0.6/0.875mA=685 ohms

W=2.52uM

L=180nM

**CMOS M3 :**- W=6.22u , L=180nm with 0.966v gate voltage.


## _DC Analysis:_

![image](https://github.com/user-attachments/assets/1f3e8beb-21be-43ee-8adf-d7cc116b851f)

## _Transient Anlysis :_

### _Input Waveform :_

![image](https://github.com/user-attachments/assets/c7f48e1a-81cb-479a-b4be-92aa816ebe5d)

**Vin=1.65-1.55**

### _Output waveform :_

![image](https://github.com/user-attachments/assets/38b7fc2c-c795-4779-8308-f95c4771b7d3)

**Vout=1.86-1.53**


### _combined output:_

![image](https://github.com/user-attachments/assets/8eab372a-ccbd-4050-806d-3b420046199d)

 ## Gain calculation

**Gain**=1.86-1.53/1.65-1.55

=3.3 V.

**Gain in dB**=20*log(3.3)

=10.52 dB.


## _AC analysis :_

![image](https://github.com/user-attachments/assets/fcaf2588-c1c5-44af-b45d-0e5152e4c1fd)

## Result:

In Differencial Amplifier Specification Vdd=3.2V , P<=2.8mw, Vicm=1.6v , Vocm=1.7v , Vp=0.6v DC analysis For W=2.52um , L=180nm We observed the Required Output By comparing the DC operationg point and given specification Transient Analysis , We Calculated gain and its is compared with AC analysis output waveform. For Circuit 2 replaced resister by current source, For Circuit 3 replaced Current Source by Mosfet. All the design specification is appeared in Simulation

## _Inference :_

**Differential Gain**: It's like a magnifying glass for differences. It makes the tiny differences between two signals much easier to see.

**Common-Mode Rejection**: Think of noise-canceling headphones. They block out background noise and let you hear the important sounds clearly.

**Biasing and Stability**: Imagine balancing a seesaw perfectly so it stays level. Proper biasing keeps everything balanced, and stability ensures it stays that way over time.

**Practical Limitations**: In real life, nothing is perfect. Small variations in components can lead to minor differences in performance, just like using slightly different ingredients in a recipe can change the final dish a bit.














