# Fourier Ptychographic Microscopy (FPM) System

An open-hardware computational imaging setup that overcomes the conventional trade-off between field-of-view (FOV) and spatial resolution using LED-matrix angular illumination and phase retrieval algorithms.

## Authors
* **Shlok Khaire**
* **Apurva Kulkarni**

## Overview
This repository contains the acquisition scripts, calibration workflows, reconstruction algorithms (DR/EPRY), presentations, and technical documentation for a low-cost, miniature Fourier Ptychographic Microscope.

## Hardware Components
* **Controller:** Raspberry Pi 3
* **Illumination:** Pimoroni Unicorn HAT HD (16×16 RGB LED array, 3.3 mm pitch)
* **Detector:** Raspberry Pi Camera Module v2 (1.12 µm sensor pixel size)
* **Optomechanics:** 3D-printed chassis mounted to an optical breadboard

## System Parameters & Calibration
* **Image Scale:** 1.055 µm/pixel
* **Optical Magnification:** 1.06×
* **LED-to-Sample Distance:** 61.8 mm
* **Reconstruction Pipeline:** Directed Relaxation & Embedded Pupil Recovery (DR/EPRY)
* **Resolution Validation:** Resolves down to the 81 LP/mm target on Thorlabs R1L3S5 ruling.

## Repository Structure
* `/Code`: Jupyter notebook for multi-color full FOV reconstruction (`FPM_RGB_FULL_FOV_FAST_GOOD_QUALITY.ipynb`).
* `/Report`: Standard Operating Procedure and technical documentation (`FPM_Report.pdf`).
* `/PPT`: Initial, mid-term, and final project presentations.
* `/Results`: Raw captures, spiral acquisition sequences, phase retrieval plots, and full FOV reconstructions.

## References
* Reconstruction code framework based on [johnmeshreki/FPM](https://github.com/johnmeshreki/FPM).
* Hardware concept based on open-source FPM works by Aidukas et al. and Guzmán et al.
```[cite: 1]
