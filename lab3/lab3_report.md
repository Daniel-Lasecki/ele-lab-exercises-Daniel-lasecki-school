# Transient Analysis of Step Response in RC and RL Circuits

## Group Information
- **Student Names**: Przemyslaw Lasecki
- **Student number**: 2203535

---

## Introduction

This report covers the transient analysis of RC and RL circuits. The circuits are analyzed for their step response using LTSpice simulations. Lab procedue is below in part 3.

## Part 1: RC Circuit Simulation and Lab Measurements

### Circuit Description

This is a simulation of an RC circuit with the following component values:
- **R** = 45.3 kΩ 
- **C** = 36 nF
- **Step Voltage** = 2.2 V

The voltage source generates a step input at 1 ms, transitioning from 0V to 2.2V. The goal is to observe the voltage across the capacitor as it charges over time.

### Task 1: RC Circuit Current Calculation

The current in an RC circuit decays exponentially as the capacitor charges. The current at any time \( t \) can be calculated using the formula:

\[
I(t) = \frac{V}{R} \cdot e^{-\frac{t}{\tau}}
\]

### Schematic and simulation

![Schematic of RC Circuit](elelab3_task1.PNG)

*Figure 1: Schematic of the RC Circuit simulated in LTSpice. Current is plotted on negative axis but its alinged with correct values*



### Analysis

- The voltage across the capacitor follows an exponential charging curve, as expected, approaching 2.2V after a few time constants.
- The current through the capacitor decays exponentially as the capacitor charges up.


---

## Part 2: RL Circuit Simulation

### Circuit Description

The RL circuit is simulated with the following component values:
- **Resistor (R)** = (53 + 20)=73Ω
- **Inductor (L)** = (35 + 2)= 37µH
- **Step Voltage** = (22 / 10)= 2.2 V


The goal is to observe the current through the inductor and the voltage across the inductor over time in response to the step voltage input.

### Schematic and simulation

![Schematic of RL Circuit](elelab3_task2.PNG)

*Figure 2: Schematic of the RL Circuit simulated in LTSpice. Current is plotted correctly on positive axis*


### Analysis

- The current through the inductor starts at 0 and increases over time as the inductor opposes the change in current initially, then slowly allows current to flow.
- The voltage across the inductor decays as the current increases.

---

## Part 3: Lab Measurements (RC Circuit)

### Component Values Used in Lab:

- **Resistor (R)**: 47 Ω (lab value, simulated value: 45.3 kΩ)
- **Capacitor (C)**: 47 nF (lab value, simulated value: 36 nF)
- **Step Voltage**: 2.2 V

### Signal Generator Configuration

To generate the step input, the signal generator was set up with the following parameters:

- **Initial Voltage**: 0 V
- **Final Voltage**: 2.2 V
- **Frequency**: 10 Hz (low enough to allow the capacitor to fully charge before the next pulse)
- **Waveform**: Square wave (mimicking a step input)

### Oscilloscope Setup

The oscilloscope was used to measure the **voltage across the capacitor** over time to capture the charging behavior. The following steps were followed:

1. **Circuit Connection**: The signal generator was connected in series with the resistor and capacitor, and the oscilloscope probes were placed across the capacitor.
2. **Measurement of Voltage**: The voltage across the capacitor was recorded, showing the exponential rise as the capacitor charged.
3. **Time Constant Estimation**: The oscilloscope was used to estimate the time constant (\( \tau \)) by measuring the time it took for the voltage to reach approximately **63% of the final voltage**.

### Captured Data

- **Breadboard Setup**: A photo of the physical RC circuit setup on the breadboard.
- **Oscilloscope Screenshot**: A screenshot showing the **voltage across the capacitor** over time.
- **Signal Generator Settings**: A photo of the signal generator settings used during the experiment.
- **Oscilloscope Measurement**: A screenshot showing the **estimated time constant** (the time at which the capacitor voltage reaches 63% of 2.2V).

### Observations

- The **real-world time constant** was calculated from the oscilloscope measurement and compared with the theoretical time constant:
  \[
  \tau = R \times C = 47 \, \Omega \times 47 \, \text{nF} = 2.21 \, \text{μs}
  \]
- This value was slightly different from the time constant observed in the simulation due to the change in component values.

### Conclusion

The real-world RC circuit behaved similarly to the simulated circuit, with the capacitor charging curve closely following the expected exponential behavior. The time constant observed in the lab was comparable to the calculated value based on the lab component values.


