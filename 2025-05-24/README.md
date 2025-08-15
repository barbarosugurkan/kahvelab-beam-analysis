# 2025-05-24 Data Analysis: A Study on ADC Values and PMT Response

This README provides a summary of the data analysis and key findings from the experiment conducted on May 24, 2025. This study builds upon the previous analysis, with code updates to explore new hypotheses.

## Project Overview

This work focuses on analyzing data from the photomultiplier tube (PMT) and ADC (Analog-to-Digital Converter) system. The main goal of this analysis was to understand how changes in the experimental parameters, specifically the nanosecond (ns) values, affect the system's output. The findings of this analysis are documented in the accompanying presentation.

## Hypotheses and Findings

Based on the initial data exploration, two main hypotheses were tested:

1. Hypothesis 1: Increasing the ns value would lead to a decrease in the number of non-zero ADC counts.

- Reasoning: The initial expectation was that an increase in ns values might lead to more data being read, but our hypothesis posited a counterintuitive decrease in non-zero counts.

- Finding: As shown in the initial histograms presented, this hypothesis was confirmed.

2. Hypothesis 2: Increasing the ns value would result in higher non-zero ADC values.

- Reasoning: The increase in ns values corresponds to a longer data acquisition window. This is expected to increase the integral of the signal read by the ADC, resulting in higher measured values.

- Finding: This expected outcome was also confirmed in subsequent histograms, which showed a clear increase in non-zero ADC values as the ns values were raised from 10 to 20 to 30 ns.

## Ongoing Work: Counter Test and Fit Analysis

In addition to the main analysis, a new study has been initiated to test the functionality of the counter. The purpose of this test is to verify the counter's correct operation.

Data for this test has been collected and plotted in a new histogram. For the first time in this project, two different fits—Poisson and Gaussian fits—were applied to this new histogram. How apply this fits to the histograms is learnt with the help of LLMs. The meaning and implications of these fits will be the focus of the next week's analysis.
