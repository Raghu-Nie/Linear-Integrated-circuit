# Experiment - 1
Question: Given the power as P=100µw, Perform AC, DC and Transient analysis for the given circuit design by using Ltspice simulator.

## Circuit diagram -1
![image](https://github.com/user-attachments/assets/c19f3b9f-993b-4e53-acd4-0dfa1c99bfe7)

## Procedure
Create a Folder

Create a new folder and name it "project file". This will be your repository for all project files.
Set Up Your MOSFETs

For NMOS:

Name: CMOSN
Length (L): 180nm
Width (W): 3μm

For PMOS:
Name: CMOSP
Length (L): 180nm
Width (W): 3μm

DC Analysis
Apply Vdd = 1.8V
Set Vgs = 0.9V
Set up a DC operating point analysis with the .op command
Run the analysis to determine Vout and Id

Transient Analysis
Set Vgs = 0.9V
Apply an amplitude of 50mV
Use a frequency of 1kHz

AC Analysis
Add the library path
Use the command .ac dec 20 .1 1T to set up your AC analysis
Run the simulation to analyze the frequency response

# DC Analysis 

Go to simulate in LTspice, Select the dc output print and the run the simulation

![image](https://github.com/user-attachments/assets/321049e2-101d-4b7d-ba7d-e92693f362cc)

# AC analysis

![image](https://github.com/user-attachments/assets/efe710d6-d698-4442-ae70-808239ef85eb)

Output Graph

![image](https://github.com/user-attachments/assets/2f2bb91d-78da-469e-9176-fdd5ff200ea6)

# Transient Analysis
Open Your LTspice Project:
Load the project file you have been working on.

Set the Stop Time for Transient Analysis:
Go to Simulation > Edit Simulation Cmd.
Select the Transient tab.
Set the stop time to 1ms.
Click OK.
Run the Simulation:

Click on the Run button (the running man icon) to start the simulation.
Observe the Waveform:
The waveform viewer will open, displaying the results of the transient analysis.
You should see the voltage or current waveforms over the 1ms timeframe

![image](https://github.com/user-attachments/assets/0332ad84-d1f7-4646-ab3b-5974cec5c4dc)

# Result 

During the DC analysis, we observed that the NMOS, with a length of 175nm and a width of 178nm, had a drain current of 55.5 µA.

# Inference

The drain current helps determine if the MOSFET is operating in the saturation region, influenced by the gate-to-source voltage (VGS). Coupling and bypass capacitors play a role in the frequency response, while the circuit's gain is shaped by the MOSFET's characteristics. Adding the right library files is crucial for accurate simulation, and tweaking the MOSFET's dimensions can fine-tune the drain current. By understanding these factors, you can optimize the circuit's performance.

# Circuit Diagram-2

![image](https://github.com/user-attachments/assets/28503f80-2c38-4f25-840c-b3a705a19d9e)

# Procedure
## DC Sweep analysis

![image](https://github.com/user-attachments/assets/8165a140-593e-4fa2-b617-b49b1b5cbd05)

VTC curve

![image](https://github.com/user-attachments/assets/b4523150-7fe3-43a9-9891-70ca9ecc3335)

Edit input

![image](https://github.com/user-attachments/assets/bbdf3c2f-080f-4a21-9956-c713e0148648)

Change the length and width of the NMOS and PMOS

![image](https://github.com/user-attachments/assets/167cefd1-e9e9-4b39-96f7-1c0a4152347c)

![image](https://github.com/user-attachments/assets/72b77148-bb75-477f-ab03-cc339b5b1f65)


# DC Analysis

![image](https://github.com/user-attachments/assets/8afc3555-7aba-4994-9a4a-a0309a8c07ac)

# AC Analysis

![image](https://github.com/user-attachments/assets/4dffe530-1931-4e1c-bfb3-5588d70e9b5c)

Output waveform

![image](https://github.com/user-attachments/assets/6820863d-c0c6-439a-a7c6-a1d3dc35d337)

# Transient analysis
Go to the simulation settings in LTspice, set the stop time to 1ms, and run the simulation The waveform of Transient Analysis

![image](https://github.com/user-attachments/assets/fc42037b-7d07-4eb2-a30c-965bd639993f)

# Result
By adjusting the sizes of the MOSFETs, M1 and M2, we achieved our target current. M1 was set to a length of 500nm and a width of 950nm, while M2 had a length of 300nm and a width of 1020nm. The circuit delivered a gain of 3.8 dB and had a phase shift close to 180 degrees, perfectly meeting our expectations. It also showed stable and reliable performance in response to changes in input

# Inference

The DC sweep analysis helped us determine the input DC voltage. By tweaking the sizes of the MOSFETs, we were able to calculate the drain current during the simulation. We adjusted both M1 and M2 to achieve the desired drain current. For the AC analysis, we set the AC amplitude to 1 for an accurate evaluation. The DC sweep also displayed the Voltage Transfer Characteristic (VTC) curve at the output

