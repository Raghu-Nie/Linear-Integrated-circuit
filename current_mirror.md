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

       =0.277 mA
       
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

# Circuit :

CASE 1:

1:1 USING 180nM

![image](https://github.com/user-attachments/assets/e5c370b2-ce05-4aaa-854f-07d511fecb84)


# DC Analysis:

![image](https://github.com/user-attachments/assets/61bc0681-c187-4e17-9bdb-5f1842ae988f)

# Transient Analysis:

![image](https://github.com/user-attachments/assets/120b0c6c-3711-4f50-8a4d-24fbd1a11719)

# AC Analysis(Frequency responce):

![image](https://github.com/user-attachments/assets/adcd1784-1cb8-4daa-8de0-c8d5433599d8)

CASE 2:

1:2 USING 180nM

# Circuit :

![image](https://github.com/user-attachments/assets/4d0bb71c-a8fe-4ff3-92d3-bb10cc67a0b3)

# DC Analysis:

![image](https://github.com/user-attachments/assets/b15825c2-9485-4743-a35d-57f5aec144fd)

# Transient Analysis:

![image](https://github.com/user-attachments/assets/16d1155c-9661-4571-95e3-f877e20274e8)

# AC Analysis(Frequency responce):

![image](https://github.com/user-attachments/assets/70a93278-13b8-4726-aabc-7b4786c00b44)

CASE 3:

1:1 USING 500nM

# Circuit :

![image](https://github.com/user-attachments/assets/e5c370b2-ce05-4aaa-854f-07d511fecb84)

# DC Analysis:

![image](https://github.com/user-attachments/assets/aab85715-d23b-4770-8aa4-46f690378e45)

# Transient Analysis:

![image](https://github.com/user-attachments/assets/1748a95f-a0b6-40f6-9506-5fab55505195)

# AC Analysis(Frequency responce):

![image](https://github.com/user-attachments/assets/06c83365-9fb4-40cf-a1a7-299d67b94436)

CASE 4:

1:2 USING 500nM

# Circuit :

![image](https://github.com/user-attachments/assets/4d0bb71c-a8fe-4ff3-92d3-bb10cc67a0b3)

# DC Analysis:

![image](https://github.com/user-attachments/assets/116b35a6-3f77-4260-938a-413598311799)

# Transient Analysis:

![image](https://github.com/user-attachments/assets/1f16386a-65a8-43be-a59d-4e01f5abd782)

# AC Analysis(Frequency responce):

![image](https://github.com/user-attachments/assets/c2c60390-4111-4617-b56e-7fee93c0da2c)

CASE 5:

1:1 USING 1uM

# Circuit :

![image](https://github.com/user-attachments/assets/e5c370b2-ce05-4aaa-854f-07d511fecb84)

# DC Analysis:

![image](https://github.com/user-attachments/assets/e18c5d03-59d1-470f-b25d-4e494891a96d)

# Transient Analysis:

![image](https://github.com/user-attachments/assets/447b11b0-0207-4d8c-ab9e-d8aacddfd96c)

# AC Analysis(Frequency responce):

![image](https://github.com/user-attachments/assets/bd0c6c44-ec3b-4ed8-a463-e38988be6db1)

CASE 6:

1:2 USING 1uM

# Circuit :

![image](https://github.com/user-attachments/assets/4d0bb71c-a8fe-4ff3-92d3-bb10cc67a0b3)

# DC Analysis:

![image](https://github.com/user-attachments/assets/6499f457-59ac-42a8-9a01-12e842591ce3)

# Transient Analysis:

![image](https://github.com/user-attachments/assets/53fcc68e-9a5e-4cab-ac88-b0e1a5aaaf5e)

# AC Analysis(Frequency responce):

![image](https://github.com/user-attachments/assets/6d820ab9-0416-49f6-9f19-8c024d9597cd)

