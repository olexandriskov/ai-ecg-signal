# ai-ecg-signal

During this project, I focused on creating a software module to generate synthetic electrocardiograms (ECGs) with T-wave alternation using JavaFX. The goal was to simulate the ECG cycles accurately and visually demonstrate T-wave alternation effects.

Here's how I did it:

First, I familiarized myself with the theoretical principles of ECG signal modeling. An ECG consists of various waves: P, Q, R, S, and T, each representing different phases of the heart's electrical activity. My task was to replicate these waves using mathematical functions.

Development Process:

Initial Application Setup: I built a JavaFX application that allows users to input parameters through sliders and buttons to control the amplitude, peak time, and symmetry of the ECG waves. The interface updates the ECG graph in real-time as users adjust these settings.

Wave Calculation: The core of the application is the mathematical function that calculates the values of each ECG wave over time. This function considers parameters like amplitude and timing to generate realistic waveforms. I integrated these calculations into the app, ensuring the graph accurately reflects the input values.

Graph Generation: I used JavaFX's LineChart to visualize the ECG cycles. Each wave (P, Q, R, S, and T) is represented by a series of data points calculated for every time increment from 0 to 1.3 seconds. These series are then combined to form a complete ECG cycle.

Parameter Management: For the T-wave, users can set parameters through the GUI. I hardcoded the parameters for other waves as constants, following the assignment requirements. Event handlers for sliders and buttons dynamically update the graph based on user input, providing immediate feedback.

Enhancing with T-wave Alternation:

I extended the application to simulate T-wave alternation, which is a variation in the T-wave amplitude that can occur in successive heartbeats.

Generation Interface: I added a feature where users can specify the number of ECG cycles to generate and set the alternation level of the T-wave. This was done through a new window that opens on clicking the “generation” button.

Cycle Calculation: The program generates multiple ECG cycles, each shifted in time. The T-wave alternation is applied to even-numbered cycles, creating a realistic alternation effect in the waveform. This was achieved by modifying the amplitude in a recursive manner for each cycle.

Visualization: The generated cycles are displayed in a new graph. Users can update the graph by adjusting the alternation level and highlighting cycles with visible alternation through the “MULTICOLORED” button.

Outcome:

The result is a functional GUI application that not only displays synthetic ECGs but also simulates the T-wave alternation phenomenon. Users can interactively modify parameters and visualize the impact on the ECG cycles, making it a useful tool for understanding ECG signal variations.
