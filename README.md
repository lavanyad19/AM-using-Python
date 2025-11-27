# AM-using-Python
# AIM:
To implement and analyze Amplitude modulation (AM) using Python's NumPy and Matplotlib libraries.

# EQUIPMENTS REQUIRED
• Software: Python with NumPy and Matplotlib libraries Hardware: Personal Computer

# THEORY:
Theory of Amplitude Modulation (AM) AM is an analog modulation technique where the amplitude of a high-frequency carrier wave is varied in proportion to the instantaneous amplitude of a low-frequency message signal (or baseband signal).

# PROCEDURE
1.Install/Import Libraries: Ensure the necessary libraries, NumPy (np) for numerical calculation and Matplotlib (plt) for plotting, are imported. This is done by the first two lines of the code.

2.Define Parameters: Define the amplitudes (Am, Ac) and frequencies (Fm, Fc, Fs) for the message and carrier signals. These constants determine the characteristics of the generated signals.

3.Create Time Base: Generate a time vector (t) using np.arange(). This array represents the discrete time points over which the signals will be sampled and calculated.

4.Generate Signals: Use the defined parameters and the time base (t) to calculate the three required signal arrays: the message signal (m), the carrier signal (c), and the final AM signal (s).

5.Plot and Visualize: Use the plt.subplot() function to create a figure with three separate axes and plot the three generated signals (m, c, and s) in their respective positions for visual comparison. Finally, use plt.show() to display the generated graph.

# Program:

import numpy as np

import matplotlib.pyplot as plt

Am = 3.4

Fm = 297

Ac = 6.8

Fc = 2970

Fs = 29700

t = np.arange(0, 2 / Fm, 1 / Fs)

m = Am * np.cos(2 * np.pi * Fm * t)

c = Ac * np.cos(2 * np.pi * Fc * t)

s = (Ac + m) * np.cos(2 * np.pi * Fc * t)

plt.figure(figsize=(10, 8))

plt.subplot(3, 1, 1)

plt.plot(t, m)

plt.subplot(3, 1, 2)

plt.plot(t, c)

plt.subplot(3, 1, 3)

plt.plot(t, s)

plt.tight_layout()

plt.show()

# Output Waveform

![WhatsApp Image 2025-11-12 at 21 09 40_fa486a6f](https://github.com/user-attachments/assets/72d48aea-455a-4e45-81f4-87b231fd5459)


# Tabulation

![WhatsApp Image 2025-11-27 at 18 55 05_741874f3](https://github.com/user-attachments/assets/2120b79a-cbef-477a-bc83-c5a76883989d)



 # Calculation 

![WhatsApp Image 2025-11-27 at 18 49 36_03824035](https://github.com/user-attachments/assets/14c121a2-6bb5-440b-8830-26806f9d5c19)

# RESULT:
Thus, the AMPLITUDE modulation using python is successfully done and the output is experimentally verified.
