# kahvelab-journal

This repository contains the data analysis scripts, Jupyter Notebooks, and presentation materials for the beam characterization experiments conducted at KAHVELab. The project aims to analyze and interpret data from our experimental setup.

---

## Key Learnings & Goals

This project serves as a crucial learning platform, providing hands-on experience in both physics and engineering. My key learning objectives and outcomes from this work include:

- **Data Analysis**: Gaining practical skills in data cleaning, processing, and interpreting raw data to draw meaningful conclusions from various datasets and formats.

- **Programming Languages and Libraries**: Learning and applying the Python programming language, along with fundamental scientific computing libraries such as **NumPy**, **Pandas**, **Matplotlib**, and **SciPy**.

- **Physical Systems and Experimental Design**: Developing a deeper understanding of the physical principles behind our experimental setup (e.g., PMTs, Scintillators, ADCs, Electron Gun, etc.) and the scientific methodology for approaching complex problems.

- **Beam Dynamics and Simulations**: Researching and applying concepts related to charged particle beams, including **beam emittance**, **transverse beam dynamics**, and **Twiss parameters**. This also includes hands-on experience in processing data from simulation software like **Ibsimu** to create visualizations such as **heat maps**.

- **Statistical Methods**: Learning how to apply statistical distributions, specifically **Poisson** and **Gaussian fits**, to analyze experimental data. The concept of **Chi-Square ($\chi^2$)** was also explored to determine the goodness of a fit.

---

## Project Milestones

### Data Acquisition and Analysis

- **ADC Values and PMT Response**: Initial analysis focused on understanding how nanosecond (ns) values affect ADC counts and the number of non-zero counts. We confirmed that increasing the ns value results in higher non-zero ADC values, as predicted by the increase in the signal's integral.

- **Counter Test**: A dedicated test was initiated to verify the counter's functionality. Initially, the data was found to more closely resemble a Normal distribution, but new data collected under "no beam" and "visible light" conditions showed a pattern consistent with a Poisson distribution, as expected for random events.

- **Cage Code Development**: The data processing scripts were modified to handle different scan types. This involved adapting the code for a **vertical scan** using the `.T` (transpose) attribute in NumPy, which allowed the system to acquire data column by column instead of row by row.

- **Advanced Data Analysis**: The data acquisition format was updated to include four scan types: horizontal, horizontal backwards, vertical, and vertical backwards. We processed this new data by generating scatter plots of both the average and difference between data points, as well as combined histograms for all scan types on a single graph.

### System Anomalies and Improvements

- **Vertical Scan Anomaly**: Investigations were conducted into consistently high ADC counts, particularly during vertical scans. Analysis revealed that a **system stabilization** period is crucial, as the counts significantly decrease after waiting. However, a residual difference between vertical and horizontal counts still exists, suggesting a persistent anomaly in the vertical scanning mechanism.

- **Background Radiation**: Our analysis of "no beam" data showed that even without the electron beam, vertical counts are still higher than horizontal counts, indicating a potential asymmetry in the background radiation or detector response. The average background radiation was also found to have increased.

---

## Future Goals

Based on these findings, we plan to implement a mandatory stabilization period for all future data acquisition and develop a correction mechanism for the vertical scanning procedure. The ultimate goal is to use all the knowledge and data gained to simulate our existing beamline.