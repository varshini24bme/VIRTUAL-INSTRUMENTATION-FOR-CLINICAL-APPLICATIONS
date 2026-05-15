#  Experiment 7 – INSTRUMENTATION OF AN AMPLIFIER TO ACQUIRE AN ECG SIGNAL

##  Aim
To acquire and analyze an ECG signal using NI ELVIS Lab VIEW.

---

##  Tools Required
- National Instruments LabVIEW (any version supporting basic VI creation)

---

##  Algorithm

Procedure Without Express:
1. Construct the basic block diagram for acquiring a signal without using express.
---
<img width="1518" height="930" alt="image" src="https://github.com/user-attachments/assets/14b2fdaa-62b1-4d6c-b588-f285a61c2279" />

2. For acquiring ECG Signal:
*From the front panel, set the number of samples to read as 3000 and the sampling rate as 1000.From the physical channel drop down menu select device and the channel no. (DEVICE 1 / AI0 CHANNEL).

---
* Set the Voltage Maximum and Minimum to -5/5 V
* Save the program (CTRL + S). From the Front panel tool bar menu select
* Operate →Run (or press CTRL + R) to execute the
program. Raw ECG Signal Output:
<img width="1206" height="632" alt="image" src="https://github.com/user-attachments/assets/2845d96e-20f6-4cc8-b84c-3f5dcab2b900" />
3. Taking FFT for raw ECG:
Right click on the block diagram. From the menu appearing select Signal
Processing Wfm Measure FFT Spectrum magnitude and phase. Place the FFT
block in the block diagram.
4. Connect the data in the DAQmx read terminal to Time signal terminal of the
FFT block.

<img width="1144" height="792" alt="image" src="https://github.com/user-attachments/assets/1d445154-88a5-4357-8dee-16044ebab248" />
5. Configuring FFT block:
Keep the cursor over Window. Right click on it. A menu will pop up.
Select Create → control.

<img width="1248" height="662" alt="image" src="https://github.com/user-attachments/assets/5d6e2436-85b4-4fa8-b341-9d3b88c147fc" />
6. Similarly create a control for view.
<img width="1202" height="668" alt="image" src="https://github.com/user-attachments/assets/8647ea4b-a079-4f5f-a92a-98bff7ef9f65" />
7. Displaying the FFT magnitude:
In the front panel do right click. Select Graph Waveform Graph. Place the
Waveform Graph in the front panel.


<img width="1164" height="780" alt="image" src="https://github.com/user-attachments/assets/b3184bd3-f69b-495d-8fd8-5b6c22f97710" />

8. Connect the FFT magnitude terminal of the FFT block to the waveform Graph in
the block diagram.
9. While running the application select ‗db On (F)‟ in the view palette in the front
panel. Select Hanning window using the control in the front panel.

Final Block Diagram:
<img width="1732" height="862" alt="image" src="https://github.com/user-attachments/assets/85b74d76-c442-458f-aa69-de3ec3f9e9c2" />
10. Save the program (CTRL + S). From the Front panel tool bar menu select Operate →Run (or press CTRL + R) to execute the program. The output is as shown in the figure.

Final Front Panel:
<img width="1702" height="1270" alt="image" src="https://github.com/user-attachments/assets/df8610d6-5a0e-4ddd-83a4-9d6db345b824" />



Final Block Diagram:
<img width="1698" height="938" alt="image" src="https://github.com/user-attachments/assets/a699db72-3440-4514-b7de-223a5b96199a" />

<img width="1850" height="756" alt="image" src="https://github.com/user-attachments/assets/36cb221f-01c1-431a-900c-d7bf3b4e8418" />

Result: Thus the raw ECG signal (0-40Hz) was acquired and its FFT was obtained. Power line interference occurred at 50Hz.
