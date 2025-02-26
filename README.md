Tumor Volume Calculator

Overview

The Tumor Volume Calculator is a Python-based graphical user interface (GUI) tool that allows users to estimate tumor volume using front and side view images. The tool utilizes the Tkinter library for the GUI, PIL for image processing, and Pandas for data management.

Features

Load front and side view images of the tumor

Select a scale reference in each image for accurate measurements

Measure tumor dimensions (length, width, height) using interactive point selection

Calculate tumor volume using an ellipsoid volume approximation

Option to estimate volume using only the front view (assuming height is 2/3 of length)

Save measurements and volume calculations to an Excel file

Restart calculations and load new images as needed

Installation

Prerequisites

Ensure you have Python installed (Python 3.6 or later is recommended). The following dependencies are required:

pip install tkinter pillow pandas openpyxl

Usage

Run the script using:

python tumor_volume_calculator.py

Steps to Calculate Tumor Volume:

Load Images: Click "Load Front View" and "Load Side View" to select the corresponding tumor images.

Set Scale: Click on two points of a known real-world distance in each image and enter the actual distance in cm.

Measure Tumor Dimensions:

Click two points to measure length and width in the front view.

Click two points to measure height in the side view.

Calculate Volume:

Click "Calculate Volume (with Side View)" to compute using all three dimensions.

Click "Calculate Volume (Front View Only)" to estimate volume assuming height is 2/3 of length.

Save Data: Measurements and volume calculations can be saved to an Excel file.

Restart: Click "Restart Calculation" to clear images and reset measurements.

Calculation Formula

The volume is estimated using the ellipsoid formula:
V = (4/3) * π * (L/2) * (W/2) * (H/2)
Where:

L: Length

W: Width

H: Height

For front-view-only estimation, the height is assumed to be  of the length:
V = (4/3) * π * (L/2) * (W/2) * ((2/3) * L / 2)

License

This project is open-source and available under the MIT License.

Author

Peng Cui, PhD
Dept of OnkPat, Karolinska Institutet

