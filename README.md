# EEG-Spindle

Original_Data_V561892_2024.xlsx file contents original row data from 32-bit channel
EEG. Every column defines the EEG electrode code/name/index.
Problem Statement:
1. Alpha Spindle Count Comparison:
o Count the total number of alpha spindles in the sheets labelled ECBL
and EOBL, then compare the counts to determine the difference.

2. Electrode-wise Alpha Spindle Count Comparison:
o For each electrode, count the number of alpha spindles in both ECBL
and EOBL sheets. Compare the counts side by side for each electrode
to highlight the differences.

3. Wavelet Transform (Scaleogram) and Spindle Visualization:
o Calculate the Scaleogram (wavelet transform coefficients) for a single
electrode and for the complete dataset. Visualize the Scaleogram
alongside the spindle activity on the same time scale.
4. Epoch-based Visualization and Spindle Counting:
o Divide the complete dataset into 10-second epochs. For each epoch,
visualize the spindles and the corresponding Scaleogram, while also
counting the total number of spindles within each epoch.

Example: This is not the actual result of the above data, shared for reference only.

Hints:
1. Use MNE Python
2. Appy ICA on the data with sampling frequency 512
3. Save data in fif and csv format
4. Dive the number of samples by Sampling Frequency the you will get the time, because time
stamp is in the data as a separate column.
5. Alpha Spindle (8-13 Hz)
6. Use additional package PyWavelets for Scaleogram.
