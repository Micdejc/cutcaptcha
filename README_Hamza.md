# Purpose of this guide

This README.md is separated from the student work since it's still part of a Masters Project submission.
This guide lists and details the missing parts necessary to use the project on Debian-based machines.
Also, a commit with other missing bits has been made (mostly about the missing "cutcaptchas" folder necessary to run the app).

# Installation
Non-exhaustive list of dependencies to install on Debian-based machines (Mint 21):
```
	jupyter-notebook
	python-numpy
	python3-opencv
	python3-tk
```

# How to run the program?

* Clone the repository, enter the project's folder and launch the notebook:
```
cd cutcaptcha
jupyter-notebook GUI.ipynb
```

* Then on your browser go to:
```
http://localhost:8888/notebooks/GUI.ipynb
```

* Once on the notebook, click on the "Cell" menu, then "Run all". The interface of the app is quite simple: click on "New" to download a new picture from filecrypt servers, and then on "solve" to attempt to solve the image.

