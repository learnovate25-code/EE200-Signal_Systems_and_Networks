# EE200: Signals, Systems and Networks

## Digital Signal Processing using Fourier Analysis and Frequency-Domain Filtering

This repository contains the practical course project completed as part of **EE200: Signals, Systems and Networks** at **IIT Kanpur**.

The project demonstrates the application of Digital Signal Processing (DSP) techniques in both **image processing** and **audio signal restoration** using Python.

Two independent problems are solved:

- Frequency Mixer – Hybrid Image Generation
- Frequency De-mixer – Audio Noise Removal

---

## Project Overview

The project explores how signals can be analyzed and manipulated in the frequency domain using Fourier Transform techniques.

For images, frequency components are separated and combined to generate hybrid images whose appearance changes with viewing distance.

For audio, unwanted instrumental components are identified through spectral analysis and removed using carefully designed digital filters.

The project provides practical exposure to:

- 2D Fourier Transform
- Frequency spectrum visualization
- Hybrid image synthesis
- Digital filter design
- Power Spectral Density analysis
- Pole-Zero analysis
- Bode plots
- Audio restoration

---

## Project Structure

```
EE200/
│
├── Q1_Frequency_Mixer.ipynb
├── Q2_Frequency_DeMixer.ipynb
│
├── reports/
│   ├── Frequency_Mixer_Report.pdf
│   └── Frequency_DeMixer_Report.pdf
│
├── images/
│
├── audio/
│
└── README.md
```

---

# Question 1 — Frequency Mixer: *Beauty and the Blur*

### Objective

Study the frequency characteristics of images using the 2D Fourier Transform and construct hybrid images by combining low-frequency information from one image with high-frequency information from another.

### Key Features

- 2D FFT computation
- Magnitude spectrum visualization
- dB spectrum visualization
- FFT spectrum centering
- Rotation analysis
- Hybrid image generation
- Gaussian Low-pass filtering
- High-pass filtering
- Transfer function visualization

### Techniques Used

- NumPy FFT
- OpenCV
- Gaussian Filtering
- Frequency-domain image processing
- Matplotlib visualization

### Results

- Successfully computed and visualized the 2D Fourier magnitude spectra in both centered and non-centered forms.
- Verified that rotating an image by 90° results in an equivalent rotation of its frequency spectrum while preserving the spectral energy distribution.
- Generated a hybrid image by combining the low-frequency structure of one image with the high-frequency details of another.
- Visualized Gaussian low-pass, high-pass, and combined transfer functions to demonstrate the frequency mixing process.

### Conclusion

This experiment demonstrated how the 2D Fourier Transform can be used to analyze and manipulate image frequencies. By separating and combining different frequency components, a hybrid image was created whose appearance changes with viewing distance, illustrating the role of spatial frequencies in human visual perception.

---

# Question 2 — Frequency De-mixer: *Unwanted Solo*

### Objective

Restore a corrupted music track by removing unwanted instrumental components using frequency-domain analysis and digital filtering.

### Key Features

- Audio normalization
- PSD analysis
- Spectrogram generation
- Butterworth Band-stop filter design
- Bode plots
- Pole-Zero plots
- Sequential filtering
- Clean audio reconstruction

### Techniques Used

- SciPy Signal Processing
- Butterworth Filters
- Welch Power Spectral Density
- Spectrogram Analysis
- Zero-phase filtering (filtfilt)

---

# Technologies Used

- Python
- NumPy
- SciPy
- OpenCV
- Matplotlib
- Jupyter Notebook

### Results

- Successfully identified unwanted frequency bands using Power Spectral Density and spectrogram analysis.
- Designed and implemented multiple Butterworth band-stop filters to suppress interfering frequency components.
- Verified filter performance through Bode plots and pole-zero diagrams.
- Produced a cleaned audio signal with significantly reduced interference while preserving the original musical content.

### Conclusion

The frequency de-mixer effectively removed unwanted instrumental noise using frequency-domain filtering techniques. The project demonstrated the practical application of Digital Signal Processing in audio restoration and highlighted the importance of spectral analysis, filter design, and zero-phase filtering for producing high-quality reconstructed audio.

---

# Learning Outcomes

Through this project, I gained practical experience in:

- Frequency-domain signal analysis
- Image processing using Fourier Transform
- Audio signal restoration
- Digital filter design
- Signal visualization techniques
- Python-based DSP implementation

---

# Repository Contents

- Source code (Jupyter Notebooks)
- Project reports
- Generated figures
- Hybrid image outputs
- Audio filtering results

---

# Acknowledgements

This project was completed as part of the **EE200: Signals, Systems and Networks** course at **IIT Kanpur** under the guidance of **Prof. Tushar Sandhan**.
