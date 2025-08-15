# 2025-06-02 Counter Test: An Analysis of Counter Data and Statistical Distributions

This README summarizes the analysis conducted on June 2, 2025, focusing on the functionality and data patterns of the counter. The study involved a deep dive into statistical distributions and the analysis of new datasets to validate the counter's performance.

## Research and Methodology

The primary goal of this work was to understand the underlying statistical nature of the counter's output. The following concepts were researched and integrated into the analysis:

- **Poisson Distribution**: Research was conducted to understand the Poisson distribution, a model that describes the number of events occurring in a fixed interval of time or space. This distribution is expected for random, independent events, such as background radiation or particle counts in our detector.

- **Bin Width**: The concept of bin width was explored, and a custom code was written to manually adjust it for more precise histogram analysis.

## Findings and Conclusions

Initial analysis of the previous counter dataset revealed an unexpected pattern. Although the data was expected to follow a Poisson distribution, it was found to more closely resemble a Normal (Gaussian) distribution. This finding prompted further investigation into the system's behavior.

The concept of **Chi-Square (χ2)** was also introduced to quantitatively assess how well a specific fit matches the histogram data. This tool will be crucial for future analyses to determine the goodness of fit.

Finally, new data was collected under two conditions: **"no beam"** and **"visible light."** Histograms and fits were generated for these new datasets. The results showed a significant shift, with the data now aligning more closely with a Poisson distribution.

These findings suggest that the counter is functioning as expected under different conditions and that the Poisson model is indeed the correct statistical framework for our data under specific circumstances. The histograms and fits from this analysis are shared in the accompanying PDF, 2025-06-02_counter_test.pdf.
