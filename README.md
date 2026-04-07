# MV-Project
Software DSP project 
# Hilbert Transform Based High-Frequency Trading Strategy

This project focuses on applying the Hilbert Transform to financial time-series data for high-frequency trading (HFT). With the increasing availability of tick-by-tick market data, traditional methods often struggle to extract meaningful insights due to noise and non-stationary behavior. This work uses signal processing techniques to transform raw price data into a more informative representation, allowing the detection of hidden market cycles and patterns. The approach is based on concepts discussed in the research paper .

The main objective of this project is to identify dominant market cycles, reduce noise in financial data, and improve trading decisions. By converting the price signal into a complex analytic signal, the method enables the extraction of phase and instantaneous frequency, which are useful for understanding market behavior. This helps in determining potential buy and sell points based on cycle peaks and troughs.

The core concept used in this project is the Hilbert Transform, which converts a real-valued signal into a complex signal consisting of an in-phase component (original signal) and a quadrature component (phase-shifted signal). This representation allows the computation of phase and frequency, making it possible to analyze cyclical movements in financial data more effectively than traditional techniques like Fourier Transform in certain cases.

The methodology involves collecting high-frequency price data, preprocessing it to remove noise and trends, and then applying the Hilbert Transform to obtain the analytic signal. From this, phase and frequency are calculated to detect cycles in the data. Based on these cycles, a simple trading logic can be implemented where buying decisions are made near cycle lows and selling decisions near cycle highs.

The implementation is done using Python, with libraries such as NumPy, Matplotlib, and SciPy for numerical computation, visualization, and signal processing. The project demonstrates how financial data can be treated as a signal and processed using digital signal processing techniques.

The results show that this approach is capable of identifying cyclic patterns in price movements and can improve the timing of trading decisions. However, there are some limitations. The method is sensitive to noise, assumes relatively narrow-band signals, and may not perform well when multiple frequencies are present in the data.

To run the project, clone the repository, install the required dependencies, and execute the main Python script. The code is organized into separate folders for data, source files, and results for better readability and structure.

This project highlights the intersection of financial engineering and signal processing, demonstrating how mathematical tools like the Hilbert Transform can be applied to real-world trading problems.

## Citation

If you use this work, please cite:

Author: Manju S Totad and Vinayak K H 

Title: Hilbert Transform Based High-Frequency Trading Strategy  
Year: 2026  

Based on research on Hilbert Transform in financial market cycle analysis.
