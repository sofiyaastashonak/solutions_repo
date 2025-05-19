# Problem 1

# Measurements – Problem 1  
## Measuring Earth's Gravitational Acceleration with a Pendulum  

---

## 🎯 Motivation  

The gravitational acceleration $g$ is one of the most fundamental constants in physics. It affects the motion of all bodies on Earth and plays a key role in mechanics, structural engineering, and even timekeeping. One of the most classical ways to measure $g$ is using the oscillation of a simple pendulum. The relationship between the period of a pendulum and gravitational acceleration is:

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

This experiment helps practice real measurement, data recording, and uncertainty estimation — all critical components of experimental physics.

---

## 🧪 Materials  

- String of length ~1.00 m  
- Small weight (keychain)  
- Stopwatch (smartphone)  
- Ruler or measuring tape (resolution: 1 mm)

---

## 🔧 Experimental Setup  

1. Suspend a small weight from a fixed support using a string.
2. Measure the length $L$ of the pendulum from the **pivot point to the center of mass** of the weight.  
   - **Measured length**: $L = 1.000$ m  
   - **Measurement tool resolution**: $\Delta L = \pm 0.005$ m (half of smallest division)

---

## ⏱️ Data Collection  

Measure the time for **10 full oscillations**. Repeat the process **10 times**.

| Trial | Time for 10 Oscillations $t_{10}$ (s) |
|-------|--------------------------------------|
| 1     | 20.12                               |
| 2     | 20.08                               |
| 3     | 20.09                               |
| 4     | 20.11                               |
| 5     | 20.14                               |
| 6     | 20.10                               |
| 7     | 20.13                               |
| 8     | 20.12                               |
| 9     | 20.11                               |
| 10    | 20.09                               |

---

### 📊 Statistical Analysis  

- Mean time for 10 oscillations:

$$
\bar{t}_{10} = \frac{1}{10} \sum t_{10} = 20.109\ \text{s}
$$

- Mean period for 1 oscillation:

$$
T = \frac{\bar{t}_{10}}{10} = 2.0109\ \text{s}
$$

- Standard deviation of $t_{10}$:  
$$
\sigma = 0.018\ \text{s}
$$

- Uncertainty in mean time:  
$$
u_{\bar{t}_{10}} = \frac{\sigma}{\sqrt{N}} = \frac{0.018}{\sqrt{10}} \approx 0.0057\ \text{s}
$$

- Uncertainty in $T$:  
$$
u_T = \frac{u_{\bar{t}_{10}}}{10} = 0.00057\ \text{s}
$$

---

## 🧮 Calculations  

### ✅ Calculating $g$

Rearrange the pendulum formula:

$$
g = \frac{4\pi^2 L}{T^2}
$$

Substitute:

$$
g = \frac{4\pi^2 \cdot 1.000}{(2.0109)^2} \approx 9.774\ \text{m/s}^2
$$

---

### ✅ Propagating Uncertainty in $g$

Using:

$$
\frac{u_g}{g} = \sqrt{\left(\frac{u_L}{L}\right)^2 + \left(2\frac{u_T}{T}\right)^2}
$$

Substitute:

$$
\frac{u_g}{g} = \sqrt{\left(\frac{0.005}{1.000}\right)^2 + \left(2 \cdot \frac{0.00057}{2.0109}\right)^2} \approx 0.0050
$$

Then:

$$
u_g = 0.0050 \cdot 9.774 \approx 0.049\ \text{m/s}^2
$$

---

### ✅ Final Result:

$$
g = (9.774 \pm 0.049)\ \text{m/s}^2
$$

---

## 📈 Comparison with Accepted Value

- Accepted value: $g = 9.80665$ m/s²  
- Our value: $9.774$ m/s²  
- Deviation: $\approx 0.33\%$  
- **Reasonable match** within experimental uncertainty.

---

## 🧐 Uncertainty & Limitations

- **Measurement Uncertainty**: Small changes in length or timing can significantly affect $g$.
- **Human Reaction Time**: Manual timing is limited by human reflex (typical uncertainty ~0.2s if timing 1 oscillation, but minimized here by timing 10 oscillations).
- **Assumptions**:
  - The angle is small (<15°), ensuring approximation $\sin \theta \approx \theta$.
  - The string is massless and taut.
  - No air resistance or friction at the pivot.

---

## ✅ Conclusion

We used a simple pendulum to estimate Earth's gravitational acceleration and obtained:

$$
g = (9.774 \pm 0.049)\ \text{m/s}^2
$$

This value is **consistent with the accepted standard**, demonstrating that with careful measurement and uncertainty analysis, accurate physical constants can be determined even with basic equipment. This experiment reinforces the importance of statistical treatment and precision in experimental physics.

---
