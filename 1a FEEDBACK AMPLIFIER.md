# Exp. No. 1(a)
**Date:**  

## FREQUENCY RESPONSE OF VOLTAGE SERIES FEEDBACK AMPLIFIER

---

### **Aim**
To design and analyze the voltage-series feedback amplifier and to calculate the following parameters with and without feedback:

1. Mid-band gain  
2. Bandwidth and cut-off frequencies  
3. Gain Bandwidth Product  

---

### **Components & Equipment Required**

| Sl. No. | Components / Equipment | Range / Specifications | Quantity |
|:--------:|------------------------|------------------------|:---------:|
| 1 | Power supply | (0–30)V | 1 |
| 2 | Function generator | (0–20M)Hz | 1 |
| 3 | CRO/DSO | 50MHz | 1 |
| 4 | Transistor | BC107 | 1 |
| 5 | Resistors (Ω) | 47k, 10k, 1k, 2.2k | Each 1 |
| 6 | Capacitors (F) | 47µ, 100µ | Each 1 |
| 7 | Connecting wires | – | As required |

---

### **Theory**
In a **voltage-series feedback amplifier**, the sampling is voltage and the mixing is series.  
Since both the input and output are voltage signals, it is called a **voltage amplifier** with gain \( A_{vf} \).

The **bandwidth** is defined as the range of frequencies over which the gain remains greater than or equal to **0.707 times the maximum gain**, or is within **3 dB down** from the maximum gain.

\[
\text{Bandwidth (BW)} = f_h - f_l
\]

Where:  
- \( f_h \): Upper cut-off frequency  
- \( f_l \): Lower cut-off frequency  

At the cut-off frequency:  
\[
A_v = 0.707 \times A_{v(max)}
\]

In all feedback amplifiers, **negative feedback** is employed — it **reduces the gain** but **increases the bandwidth**, enhancing the amplifier's stability.

---

### **Procedure**

1. Connect the circuit as per the given circuit diagram.  
2. Keep the input voltage constant.  
3. Vary the frequency from **50 Hz to 3 MHz** in regular steps and record the corresponding output voltage.  
4. Plot the graph: **Gain (dB)** vs **Frequency**.  
5. Determine the bandwidth from the graph.

---

### **Precautions**
- Avoid loose connections.  
- Ensure proper input voltage is applied.  

---

### **Design**

**Given Data:**  
\[
V_{CC} = 12V, \quad V_{BE} = 0.7V, \quad f = 50Hz, \quad I_C = 2mA, \quad h_{fe} = 100
\]

---

#### **Step 1:**  
Assume proper operating conditions for amplification.

---

#### **Step 2: Finding \( R_E \) and \( R_C \)**  
Apply **KVL** to the output loop:

\[
V_{CC} = I_C R_C + V_{CE} + I_E R_E
\]

---

#### **Step 3: Finding \( R_1 \) and \( R_2 \)**  
From the **voltage divider rule**:

\[
V_B = \frac{R_2}{R_1 + R_2} \times V_{CC}
\]

For a silicon transistor, \( V_{BE} = 0.7V \).  
To avoid overloading:  
\[
I_{R1} = 10 I_B, \quad I_{R2} = 9 I_B
\]

---

#### **Step 4: Finding Capacitances \( C_E \) and \( C_C \)**  

- **Bypass Capacitor (\( C_E \))**  
  Used to short the emitter resistor at signal frequencies to maintain high gain.

- **Coupling Capacitor (\( C_C \))**  
  Used to couple AC signals between stages while blocking DC.

---

### **Circuit Diagram**

#### i) Without Feedback
![Without Feedback Circuit](images/without_feedback.png)

#### ii) With Feedback
![With Feedback Circuit](images/with_feedback.png)

*(Note: Add circuit images in the `images/` folder for proper GitHub rendering.)*

---

### **Tabulation**

| Frequency (Hz) | \( V_0 \) (V) | Gain (dB) = 20 log(V₀/Vᵢ) | Frequency (Hz) | \( V_0 \) (V) | Gain (dB) = 20 log(V₀/Vᵢ) |
|:---------------:|:-------------:|:--------------------------:|:---------------:|:-------------:|:--------------------------:|
| **Without Feedback** |  |  | **With Feedback** |  |  |

**Input Voltage (Vi):** _____  

---

### **Model Graph**
![Gain vs Frequency Graph](images/gain_vs_frequency.png)

*(Gain (dB) vs Frequency plot to determine bandwidth.)*

---

### **Result**

Thus, the **voltage series feedback amplifier** is designed and constructed.  
The following parameters are calculated:

| S.No | Parameters | Without Feedback | With Feedback |
|:----:|-------------|:----------------:|:--------------:|
| 1 | Lower cut-off frequency | = | = |
| 2 | Upper cut-off frequency | = | = |
| 3 | Bandwidth | \( BW = f_h - f_l = \) | \( BW = f'_h - f'_l = \) |
| 4 | Mid-band Gain | \( A_{v(mid)} = \) | \( A'_{v(mid)} = \) |
| 5 | Gain at half power point |  |  |

---

**Conclusion:**  
The frequency response of the voltage-series feedback amplifier was studied. It was observed that the **gain decreases** while the **bandwidth increases** when negative feedback is applied, confirming the theoretical expectations.

---

**End of Experiment**
