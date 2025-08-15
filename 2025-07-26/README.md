# 2025-07-26 Remote Work: Data Analysis

This `README` documents the remote work conducted on July 26, 2025. The focus of this session was to analyze new data from the Cage code, which has a different format than previous acquisitions.

---

## Data Format and Scan Types

The data acquisition method has been updated, and the new dataset consists of four distinct scans: **horizontal**, **horizontal backwards**, **vertical**, and **vertical backwards**. The logic for these scan types is detailed in the previous `README` document.

A key change in the data structure is that each folder now contains **10 data values**, corresponding to **five points**. Specifically, the first and second values represent the first point, the third and fourth values represent the second point, and so on, for a total of five data points per folder.

Horizontal file mapping:

<img width="573" height="280" alt="resim" src="https://github.com/user-attachments/assets/cd691dfe-2ab1-444d-afc0-0d150286df39" />

Horizontal backwards file mapping:

<img width="575" height="295" alt="resim" src="https://github.com/user-attachments/assets/d2e28c7f-b0f4-4944-ad80-d5d9af9395d4" />

Vertical file mapping:

<img width="579" height="294" alt="resim" src="https://github.com/user-attachments/assets/4a2512c7-b9e1-49a8-abbe-8b072fc9260f" />

Vertical backwards file mapping:

<img width="585" height="288" alt="resim" src="https://github.com/user-attachments/assets/7229ce5d-2cd2-4a24-aab5-efb7e2ca8509" />

## Methodology and Visualization

The primary objective was to process this new data format to generate insightful visualizations. For each data pair, two different scatter plots were created:

- A scatter plot of the **average** of the two values for each point.
- A scatter plot of the **difference** between the two values for each point.

Additionally, a combined plot was generated to display histograms for all four scan types (horizontal, horizontal backwards, vertical, and vertical backwards) on a single graph, allowing for a direct comparison of the distributions.

## Initial Findings and Next Steps

The analysis of this new data revealed significantly higher readings compared to previous experiments. The reason behind this increase is not yet clear and will be the subject of the next analysis.
