# Seismic Waveform Frequency Analysis Using ObsPy

This project demonstrates a workflow for analyzing seismic waveform data using the ObsPy Python library. It includes downloading waveform data from IRIS, preprocessing the signal, computing the Fourier amplitude spectrum, estimating the corner frequency, and visualizing both the waveform and its frequency spectrum.

---

## Project Overview

Earthquake source characterization often involves frequency-domain analysis of seismic signals. The corner frequency extracted from displacement spectra is an important parameter related to the earthquake source. This project automates the processing and analysis steps using ObsPy and scientific Python libraries.

---

## Features

- Download seismic waveform data for a specified event and station using IRIS FDSN client
- Remove instrument response to obtain displacement time series
- Preprocess signal: detrending and tapering
- Compute Fourier amplitude spectrum with cosine tapering
- Estimate corner frequency using spectral amplitude criteria
- Plot and save waveform and spectrum for visualization

---

## Requirements

- Python 3.x
- ObsPy
- NumPy
- SciPy
- Matplotlib

Install dependencies using:

## Usage

Edit parameters (network, station, channel, event time, duration) in `main.py` as required. Run:


This will output the estimated corner frequency and save plots to `figures/` directory.

---

## Repository Contents

- `main.py` — Python script implementing the analysis
- `figures/` — Folder containing output waveform and spectrum plots
- `jaje.pdf` — Detailed report documenting methodology and results
- `README.md` — This file

---

## Sample Output

![Waveform](figures/waveform.png)

![Spectrum](figures/spectrum.png)

---

## Author

Aditya Phukon, IIT Bombay

---

## References

- ObsPy Documentation: https://docs.obspy.org  
- IRIS FDSN Web Services: https://service.iris.edu  
- Seismological signal processing literature

