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
