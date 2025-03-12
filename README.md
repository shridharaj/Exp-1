# EXPERIMENT-1
Question: Given the power as P=100µw, Perform AC, DC and Transient analysis for the given circuit design by using Ltspice simulator.

### CIRCUIT DIAGRAM-1 :
![image](https://github.com/user-attachments/assets/c780ef91-3ebe-4195-921f-04f17883b623)

### PROCEDURE:
Using the power formula P=V*I, we can calculate drain current as:
Id=5.55e-005A
#### 1. DC Analysis
Go to simulation.  Select the dc output type and then run the simulation.

![image](https://github.com/user-attachments/assets/ef924102-e523-4182-a514-e4dd73970e36)

This figure represents the results of dc analysis.
 ![Screenshot 2025-03-12 144632](https://github.com/user-attachments/assets/6f0b8f0e-fbb4-4679-bb6d-8bc8d972fe60)

#### 2. AC Analysis
Go to simulation.  Choose the ac analysis.  Use the values provided below and run the experiment.

![image](https://github.com/user-attachments/assets/a0f7da9d-3529-4060-b0c1-7669947a6c04)

The output of the AC analysis is shown in the graph below.

![image](https://github.com/user-attachments/assets/b547e04e-196e-47fd-8797-e1cc9ba7eb9c)

#### 3. Transient Analysis
Go to simulation.  Set the stop time to 1ms and start the experiment.
 The graph below displays the results of transient analysis.

![image](https://github.com/user-attachments/assets/eee3db42-638e-430f-9aaf-1dd7c4141f70)

### RESULT:
* got the calculated drain current=5.55e-005 in DC analysis output by calculating the NMOS length=175nm and width=178nm.
* The circuit maintains its performance across the tested frequency range.
* The circuit reacts well to changes and conforming its stability.

### INFERENCE:
* Drain current indicates whether MOSFET is in sturation region.
* The regions of the MOSFET depends on VGS value.
* Coupling and bypass capacitors affect the frequency response.
* Gain depends on the MOSFET parameters.
* To simulate add a Specific components library files to simulated software.
* Adjust the length and width of the MOSFET to get calculated drain current value in simulation.

### CIRCUIT DIAGRAM-2:

![image](https://github.com/user-attachments/assets/aa571835-21ea-4ca5-942e-f7bcbca4cc25)

### PROCEDURE
#### 1. DC Sweep analysis
This analysis used to find the vin value.
Go to simulate, Select a dc sweep analysis, Give the values as shown below and run the simulation.

![image](https://github.com/user-attachments/assets/33d5b92c-a501-43eb-a134-30cc05e216e1)

Below graph shows the VTC curve and the value of vin as 0.8v

![image](https://github.com/user-attachments/assets/c9c9e3d4-0a57-4356-b84d-8a821b9c8448)

Now give the input as 

![image](https://github.com/user-attachments/assets/bb1c591b-4d3a-4344-b2f2-80372af8567a)

The length and width of the NMOS and PMOS tranistor as shown in the below figure

![image](https://github.com/user-attachments/assets/283c39f0-5eea-4292-a833-91b5da308a6b)

![image](https://github.com/user-attachments/assets/3641668c-d141-48e5-b0e2-aac11a9b014c)

#### 2. DC Analysis
Go to simulate, Select the dc output print and the run the simulation.

![image](https://github.com/user-attachments/assets/daef7b7e-e64c-4510-8f23-e55121daa510)

#### 3. AC Analysis
Go to simulate, Select the ac analysis, Give the values as shown below and run the simulation.

![image](https://github.com/user-attachments/assets/6d629781-a005-40d2-87f3-e2b178e2ad4c)

Below graph shows the output of the AC analysis.

![image](https://github.com/user-attachments/assets/cbcdaa25-38e7-4266-8034-4108e9402a90)

#### 4. Transient analysis
Go to simulate, Set the stop time as 1ms and run the simulation.
The below graph shows the output of transient analysis.

![image](https://github.com/user-attachments/assets/c0f8f7c7-ed03-4867-8433-047d7c474862)

### RESULT:
* By adjusting the channel dimensions (L, W) of MOSFETs M1 and M2, the desired current was achieved at:
   M1: L = 500nm, W = 950nm
   M2: L = 300nm, W = 1020nm
*The gain is 3.8dB, and the phase shift is nearly 180 degrees, aligning with theoretical expectations.
*The circuit exhibits a stable response to input variations, confirming reliable operation.


### INFERENCE:
* By DC sweep analysis,The transistor operates correctly in the saturation region, which is required for amplification and we get the input DC voltsge.
* In simulation, modify the MOSFET size to obtain the estimated drain current value by Varying both MOSFET(M1 & M2) to get the calculated drain curren.
* AC Analysis: The circuit maintains constant gain over a range of frequencies, demonstrating its suitability for amplification and Set the AC amplitude to one in the AC analysis.
* In DC sweep analysis, we obtain the VTC curve at the output.
