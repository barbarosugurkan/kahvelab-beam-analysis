# 2025-07-20 Remote Work: Cage Code and Vertical Scan

This `README` documents the remote work performed on July 20, 2025, focused on understanding and modifying the "Cage" code for data acquisition. The main task was to develop the code for a vertical scan, building upon the existing horizontal scan logic.

## Horizontal vs. Vertical Scan

To understand the scope of the project, it's essential to define the difference between the horizontal and vertical scan methods used in our data acquisition:

- **Horizontal Scan:** The system acquires ADC data by scanning row by row. This is organized in folders named `1, 2, 3, 4` up to `20`, where each folder represents a row. Inside each folder, there are `21` individual files, for example, `SEMtest0.0.adc` for the first row, first column, and `SEMtest0.1.adc` for the first row, second column. The non-zero values in these files represent the data for each cell.

- **Vertical Scan:** The system is configured to scan column by column. Accordingly, the folders named `1, 2, 3, 4` now represent the columns. The goal was to write a new code that would process the data in this vertical format, interpreting the folders as columns instead of rows.

## Methodology and Key Changes

The primary task was to write the code for the vertical scan. This was achieved by leveraging the `.T` (transpose) attribute of a NumPy array. This allowed me to effectively flip the data from a row-based format to a column-based format with minimal code changes. Additionally, variable names were updated to be more descriptive and align with the new logic, improving the code's readability and maintainability.
