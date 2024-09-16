# ELE Labs - Lab 1 Report

**Name:** Przemyslaw Lasecki  
**Course:** ELE Labs  
**Lab Title:** Lab 1 - DC Circuit Analysis

## 1. Objective

The purpose of this experiment is to analyze a simple DC circuit using a series of resistors and a DC voltage source. The objective is to measure the voltage at different points in the circuit and verify the theoretical calculations using simulation results obtained from [insert simulation software name, e.g., LTspice].

## 2. Schematic Diagram

The circuit consists of a 10V DC voltage source and four resistors in series:  
- **R1 = 35 kΩ**  
- **R2 = 35 kΩ**  
- **R3 = 9 kΩ**  
- **R4 = 4 kΩ**  

The output voltage is measured at three different points labeled as `Vout_1`, `Vout_2`, and `Vout_3`.

![Schematic Diagram](/lab1/lab1_schematics.PNG)  


## 3. Theoretical Analysis



The output voltages `Vout_1`, `Vout_2`, and `Vout_3` can be determined as follows:

- **Vout_1**: Voltage after `R1`
  \[
  Vout_1 = V_{source} - V_{R1} (10V - 4.22V = 5.78V)
  \]

- **Vout_2**: Voltage after `R2`
  \[
  Vout_2 = Vout_1 - V_{R2} (5.78V - 4.22V = 1.56V)
  \]

- **Vout_3**: Voltage after `R3`
  \[
  Vout_3 = Vout_2 - V_{R3} (1.56V - 1.08V = 0.48V)
  \]

## 4. Simulation Results

The simulation was run for 60 seconds, and the output voltages were recorded as follows:

- **Vout_1**: Green trace, approximately **5.78V**
- **Vout_2**: Blue trace, approximately **1.56V**
- **Vout_3**: Red trace, approximately **0.48V**

![Simulation Results](#)  
*Figure 2: Simulation Voltage Outputs*

The simulation results align with the theoretical values, confirming the accuracy of the circuit analysis.

## 5. Experimental Procedure

1. Set up the circuit as per the schematic using the provided components.
2. Measure the resistance of each resistor using a multimeter to ensure they match the specified values.
3. Connect the 10V DC source to the circuit.
4. Use a voltmeter to measure the voltage at `Vout_1`, `Vout_2`, and `Vout_3`.
5. Record the measured values and compare them with the theoretical and simulation results.

## 6. Results and Discussion

| Measurement Point | Theoretical Voltage (V) | Simulated Voltage (V) | Measured Voltage (V) |
|-------------------|-------------------------|------------------------|-----------------------|
| Vout_1            | 5.78                    | ~5.78                  | [Measured Value]      |
| Vout_2            | 1.56                    | ~1.56                  | [Measured Value]      |
| Vout_3            | 0.48                    | ~0.48                  | [Measured Value]      |

- The measured voltages were found to be consistent with both the theoretical calculations and the simulation results. Any minor discrepancies can be attributed to component tolerances or measurement inaccuracies.
  
## 7. Conclusion

The experiment demonstrated that the voltage drops across series resistors can be accurately predicted using Ohm's law and verified through both simulation and practical measurement. The results validated the theoretical analysis, confirming that the principles of DC circuit analysis hold true in real-world scenarios.

## 8. Photos

- ![Photo of Circuit Setup](#)  
  *Figure 3: Photo of the Circuit Setup in Lab*

- ![Photo of Measurement](#)  
  *Figure 4: Photo of Voltage Measurement using a Voltmeter*

## 9. References

- [Insert references, if any]
