# Experiment 6

## Aim:

Design and analyze current mirror circuit as active load in amplifier circuit.

# current-mirrior-circuit

## Theory

A current mirror circuit is a commonly used configuration in analog electronics, typically employed to replicate a reference current in a load or another part of the circuit. It works by mirroring (or copying) the current flowing through one active device, such as a transistor, and using it to generate the same current in a different device, often in a different location. Basic Operation: A current mirror usually consists of two or more transistors (typically bipolar junction transistors, BJTs, or MOSFETs) that are connected in such a way that the current through one transistor is mirrored by the current through the other transistor(s).

**Matched Transistors**: Two or more BJTs are matched (have the same characteristics) and are typically placed in a configuration where their base-emitter voltages are equal. 

**Reference Current**: A reference current is applied to the base of one transistor (the reference transistor), causing it to conduct a current.

**Mirror Current**: The second transistor (output transistor) will conduct the same current because the base-emitter voltage of the output transistor is the same as that of the reference transistor (assuming both are in thermal equilibrium and have matched characteristics). 

For **MOSFETs**: In MOSFET-based current mirrors, the transistors are usually configured in such a way that the gate-to-source voltages are matched, and the drain current in one MOSFET is mirrored by another MOSFET. 

**Basic BJT Current Mirror**: In a basic BJT current mirror, two NPN transistors (Q1 and Q2) are used: Q1 is the reference transistor, with its collector connected to a voltage source (often a Vcc) through a resistor, and its emitter grounded. Q2 is the output transistor, which mirrors the current flowing through Q1. The base of Q2 is connected to the base of Q1, and the emitter of Q2 is connected to the same voltage level as the emitter of Q1. When a current 𝐼𝑅𝐸𝐹I REF flows through Q1, the same current (or a scaled version depending on the mirror ratio) flows through Q2. The ratio of the currents in the two transistors is determined by the ratio of their collector-emitter areas or other factors depending on the mirror design. 

 
# Quetion A

For the cicuit given below,Design and analyze current mirror circuit as active load in amplifier circuit , 
having a gain of AV = -10V/V, VDD = 1.8V, and P <= 1mW.
Perform DC analysis ,Transient analysis and AC analysis for mirror ratio 1:1, 1:2. by varying length from  180nm , 500nm , 1µm.

![image](https://github.com/user-attachments/assets/4aa1f2d9-76c1-4090-a39e-652b30230d1f)


## Design

Given ;

AV = -10V/V,

VDD = 1.8V, 

P <= 1mW

Itotal=power/Vdd

=1mW/1.8v

=0.555mA

Iref=Id=Itotal/2

       =0.277mA
       
Vg=Vin;

Rout=(ro1||ro2)

ro1=1/λ1(Id),ro2=1/λ2(Id)

gm = 2Id/Vov

Av=-2/Vov.(λ1+λ2)

Vov=0.073

Vgs = Vov+Vt=0.569

Vs = 0;

vin=Vg=Vgs=0.569 

nearly=0.57V

Ratio 1:1

Iref=0.277mA

Ratio 1:2

Iref=0.183mA

