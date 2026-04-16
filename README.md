<p align="center">
  <img src="assets/GUI1.png" width="45%" />
  <img src="assets/GUI2.png" width="45%" />
</p>

# CUTCAPTCHASOLVER

## Overview
**CUTCAPTCHASOLVER** is a research prototype that implements an automated solver for cutCAPTCHA challenges.

For background information and a public demonstration of cutCAPTCHA, refer to:  
https://filecrypt.cc/Contact.html

---

## Description
cutCAPTCHA is a puzzle-based CAPTCHA that presents a partially reconstructed image and requires users to correctly reposition three missing fragments using drag-and-drop interactions.

This project implements an automated attack pipeline that estimates the correct placement of the three puzzle fragments and outputs their corresponding \((x, y)\) coordinates within the challenge image.

---

## Installation

The project is implemented in **Python using Jupyter Notebook**. To run the system:

### 1. Clone the repository
```bash
cd cutcaptcha
jupyter-notebook GUI.ipynb
```

### 2. Open in browser
```
http://localhost:8888/notebooks/GUI.ipynb
```
### 3. Dependencies
Install the required packages:
```
	jupyter-notebook
	python-numpy
	python3-opencv
	python3-tk
```
Once on the notebook, click on the "Cell" menu, then "Run"

## Usage

The application provides a simple graphical interface with two main actions:

- **New:** Downloads a new cutCAPTCHA challenge and displays the challenge image along with the puzzle fragments.
- **Solve:** Executes the solver pipeline and outputs the estimated solution as \((x, y)\) coordinates corresponding to the correct placement of each puzzle fragment.


## Roadmap / Future Improvements
Future work aims to improve the robustness and generalization of the solver by exploring the following directions:

- Incorporation of **color continuity features** to improve matching accuracy in visually similar fragments.
- **Adaptive parameter selection** for Canny edge detection to replace fixed threshold values and improve accuracy across diverse images.

## Disclaimer
This project is intended for **research and security analysis purposes only**, focusing on evaluating the resilience of puzzle-based CAPTCHA systems under controlled experimental conditions.

## License
All right reserved.
