## Experiment No: 4
INTEGRATOR USING OP-AMP (μA741)
## Aim
To design and simulate an Integrator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the integral of the input voltage.
## Apparatus Required
•	μA741 Op-Amp
•	Resistor R = 10 kΩ
•	Capacitor Cf = 0.01 µF
•	Signal Generator
•	Dual Power Supply (±15V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
<img width="816" height="373" alt="IA" src="https://github.com/user-attachments/assets/dd17ff60-8ed3-458c-a803-4ae67a029a9d" />

## Connection Details:
•	Input signal → Resistor (R) → Inverting terminal (Pin 2)
•	Feedback capacitor (Cf) → Between Output (Pin 6) and Pin 2
•	Non-inverting terminal (Pin 3) → Ground
•	Pin 7 → +15V
•	Pin 4 → −15V
## Theory
An Integrator circuit produces an output voltage proportional to the integral of the input voltage.
## Working Principle:
•	When input is constant → output is ramp signal
•	Output is inverted
•	Output depends on time
For Sine Wave Input:
•	Output lags input by 90°
•	Output amplitude decreases with frequency
## Procedure
1.	Open Proteus software.
2.	Select μA741, resistor, capacitor, signal generator, and CRO.
3.	Connect circuit in integrator configuration.
4.	Apply ±15V power supply.
5.	Set input waveform (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.
## Tabulation
S.No	           Input Signal	 Frequency	      Expected Output	               Practical Observation

<img width="953" height="253" alt="image" src="https://github.com/user-attachments/assets/e602ffa1-91d7-448d-bc5d-07449197dae6" />

## Waveforms
<img width="1355" height="844" alt="IA-COS" src="https://github.com/user-attachments/assets/00f8b630-b5f0-4656-805f-dadb8c032897" />

<img width="1381" height="849" alt="IA-SSW" src="https://github.com/user-attachments/assets/29d7abc9-37fe-43fb-92af-f29fca252416" />

<img width="1357" height="842" alt="IA-TR" src="https://github.com/user-attachments/assets/0b53c2e5-7b5f-42b4-abf7-33b27577749e" />
## Result
The Integrator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the integral of the input signal.
The circuit behaves as an integrator.

## Conclusion
•	Output lags input by 90° (for sine input).
•	Output amplitude decreases with increase in frequency.
•	Used in waveform generation and analog computation.
## Viva Questions
1.	What is an integrator circuit?
An integrator is an op-amp circuit that produces an output voltage proportional to the integral (accumulation) of the input voltage over time.
It performs mathematical integration of the input signal.
2.	Write the output equation of integrator.
Vout=-1/Rc​∫Vindt
3.	Why does output lag input?
ntegration of a sine wave results in a negative cosine wave.
Since cosine lags sine by 90°, the output of an integrator lags the input by 90°.
Therefore, phase shift = –90
4.	What happens at very low frequency?
At very low frequency:
Capacitive reactance 
𝑋c=1/2πfC​ becomes very high.
Gain becomes very large.
Output may saturate.
Circuit may behave like an open-loop amplifier.
Drift and offset errors increase.
So, ideal integrator is unstable at low frequency.
5.	What is practical integrator?
A practical integrator is a modified integrator circuit that includes:
A resistor connected in parallel with the feedback capacitor.
This resistor:
Limits low-frequency gain.
Prevents output saturation.
Improves stability.
Reduces drift due to offset voltages.
