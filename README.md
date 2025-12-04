# DSBSC-using-Python

## AIM:

To implement and analyze DSBSC using Python's NumPy and Matplotlib libraries. 

## EQUIPMENTS REQUIRED

1.	Software: Python with NumPy and Matplotlib libraries
2.	Hardware: Personal Computer


## Algorithm:


1.	Initialize Parameters: Set the values for carrier frequency, message frequency, sampling frequency, and frequency deviation.
2.	Generate Time Axis: Create a time vector for the signal duration.
3.	Generate Message Signal: Define the message signal as a cosine wave.
4.	Compute the Integral of the Message Signal: Calculate the integral of the message signal over time.
5.	Generate DSBSC Signal: Apply the DSBSC formula to obtain the modulated signal.
6.	Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.


## Program

``
import numpy as np
import matplotlib.pyplot as plt
Am=5.7
fm=461
Ac=11.4
fc=4610
fs=46100
m=Am*np.cos(2*np.pi*fm*t)
c=Ac*np.cos(2*np.pi*fc*t)
s1=(Ac+m)*np.cos(2*np.pi*fc*t)
s2=(Ac-m)*np.cos(2*np.pi*fc*t)
s=s1-s2
plt.subplot(3,1,1)
plt.plot(t,m)
plt.subplot(3,1,2)
plt.plot(t,c)
plt.subplot(3,1,3)
plt.plot(t,s)
``


## Output Graph

<img width="554" height="413" alt="image" src="https://github.com/user-attachments/assets/e8918913-ab69-444d-9f36-514ebcce1b04" />




## Tablular Column

<img width="960" height="1280" alt="image" src="https://github.com/user-attachments/assets/e378ecc9-f2b4-4a36-bbd0-23f35cb4d602" />




## Result

Thus the DSB-SC-AM Modulation is generated using python.

