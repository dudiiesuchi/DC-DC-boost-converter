# DC-DC-boost-converter
Here is a **README** file for your **DC-DC Boost Converter** simulation created in MATLAB/Simulink.

---

## **Overview**
This MATLAB/Simulink model represents a **DC-DC Boost Converter**, which steps up a lower DC input voltage to a higher DC output voltage. The model is built using Simulink blocks, including power electronics components such as MOSFETs, diodes, inductors, capacitors, and control circuits. 

## **Working Principle**
A **Boost Converter** operates by storing energy in an inductor during the ON period of a switching device (MOSFET) and releasing it through a diode to the output capacitor and load during the OFF period. The step-up voltage gain is determined by the **duty cycle** of the pulse-width modulation (PWM) signal controlling the MOSFET.

The relationship between input voltage \( V_{in} \) and output voltage \( V_{out} \) is given by:

\[
V_{out} = \frac{V_{in}}{1 - D}
\]

where **D** is the duty cycle.

---

## **Components in the Simulink Model**
1. **DC Voltage Source**:
   - Provides the input voltage.
   - Typically, a low-voltage DC source (e.g., 12V).

2. **Inductor**:
   - Stores energy when the switch is ON.
   - Releases energy when the switch is OFF.

3. **MOSFET (Switching Device)**:
   - Controlled by a PWM signal to regulate the energy transfer.

4. **Diode**:
   - Ensures unidirectional current flow to the output.

5. **Capacitor**:
   - Smoothens the output voltage and reduces ripples.

6. **Resistive Load**:
   - Represents the output load where the boosted voltage is applied.

7. **PWM Generator**:
   - Generates a switching signal for the MOSFET.
   - Determines the boost converter's output voltage.

8. **Measurement Blocks**:
   - Voltage and current sensors to analyze system performance.
   - Display and Scope blocks for real-time visualization.

---

## **Simulation Details**
- **Software:** MATLAB/Simulink  
- **Simulation Type:** Continuous  
- **Control Method:** PWM Switching  
- **Expected Output:** Boosted DC voltage with regulated ripple  
- **Example Parameters**:  
  - Input Voltage: **12V**  
  - Duty Cycle: **60%**  
  - Expected Output Voltage: **30V** (approx.)  

---

## **How to Run the Simulation**
1. Open **MATLAB** and navigate to the Simulink model file.
2. Load the **Simulink model** (.slx file).
3. Run the simulation by clicking **Start (▶)** in Simulink.
4. Observe the output voltage using **Scope** and **Display Blocks**.
5. Adjust the **PWM Duty Cycle** to see its effect on the output voltage.

---

## **Applications**
- Used in **battery-powered applications** to step up voltage.
- Essential in **solar power systems** for voltage regulation.
- Used in **electric vehicles (EVs)** and **portable electronics**.
- Forms the basis of **power management circuits** in embedded systems.

## **References**
- MATLAB Documentation: [Boost Converter in Simulink](https://www.mathworks.com/help/physmod/sps/ug/boost-converter.html)
- Power Electronics Textbooks and Research Papers.
