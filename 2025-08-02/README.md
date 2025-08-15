# 2025-08-02 Data Analysis: System Stabilization and Vertical Scan Anomaly

This `README` summarizes the analysis of a new dataset acquired on August 2, 2025, to investigate the causes of consistently high ADC counts and a notable discrepancy between vertical and horizontal scans.

---

## Introduction and Hypotheses

Previous scanning operations showed that ADC counts were consistently higher during vertical scans compared to horizontal scans. To investigate this, two hypotheses were proposed:

* **System Stabilization:** The system may require a certain period to stabilize, causing initial high counts.
* **Vertical Scan Anomaly:** There may be a specific issue or inherent difference in the vertical scanning mechanism.

To test these hypotheses, a new dataset was acquired.

In this dataset, the format of taking data was different. There is only one folder and there are 25 data in that folder. Here is an example for horizontal file mapping:

<img width="541" height="193" alt="resim" src="https://github.com/user-attachments/assets/3c5ea533-0814-408e-ada7-543e3e113373" />


## Methodology

The new data acquisition was designed with several key changes to test the hypotheses:

* **Modified Scan Order:** The scan order was changed to Horizontal, Horizontal-Backwards, Vertical, and Vertical-Backwards. This was done to see if starting with horizontal scans would affect the subsequent vertical counts.
* **System Stabilization Check:** After the initial scan sequence, the system was allowed to stabilize. A new vertical scan (`vertical.wait`) was then performed to specifically evaluate the effect of stabilization.
* **Background Radiation Measurement:** "No beam" data was collected by suppressing the electron beam to measure background radiation. This was done in a Vertical, Vertical-Backwards, Horizontal, Horizontal-Backwards sequence.
* **Data Structure:** The new dataset consists of 25 measurements within a single folder, unlike the previous method of averaging two measurements from 10 data points across five folders.

## Analysis and Findings

The analysis confirmed that both hypotheses hold merit.

* The average counts for vertical scans have decreased and are now closer to the horizontal counts. Their standard deviations have also been reduced, providing strong evidence that the order of scanning and the stabilization period significantly impact the ADC counts.
* However, a residual difference remains between vertical and horizontal scans, suggesting a specific anomaly in the vertical scan setup is a contributing factor.
* An analysis of the "no beam" data revealed that even without the electron beam, vertical counts are still higher than horizontal counts. This indicates a potential asymmetry in the background radiation or detector response. The average background radiation has also increased to approximately 11 counts, up from a previous value of 7.

## Further Improvements

Based on these findings, the following actions have been decided upon:

* **Wait for Stabilization:** All future data acquisition will include a mandatory waiting period to allow the system to stabilize before scanning.
* **Vertical Scan Correction:** A correction mechanism will be developed and implemented for the vertical scanning procedure to account for the identified anomaly.
