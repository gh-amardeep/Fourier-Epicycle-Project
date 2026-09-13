# Fourier Epicycle Project

## Overview

This project demonstrates how the Fourier Transform can be used to
reconstruct 2D curves using rotating vectors, commonly visualized as
epicycles.

The project converts a curve into a sequence of complex-valued points,
computes its Fourier coefficients, sorts the frequency components by
magnitude, and uses the resulting components to reconstruct the
original curve.

The project is implemented in Python and designed to run in Google
Colab.

---

## Features

- Generate and process different predefined curves
- Uniformly sample points along a curve
- Convert 2D coordinates into complex numbers
- Compute the Fourier Transform using NumPy
- Calculate and sort Fourier coefficients by magnitude
- Reconstruct curves using selected Fourier components
- Visualize the Fourier reconstruction
- Visualize the epicycle chain
- Animate the epicycles as they reconstruct the curve
- Draw a custom curve using the mouse
- Apply Fourier analysis to the custom drawing
- Animate the Fourier reconstruction of the custom drawing

---

## Predefined Curves

The notebook includes the following predefined curves:

- Circle
- Ellipse
- Heart
- Star
- Oval
- Egg

A dropdown menu using `ipywidgets` allows the user to select a curve
for processing.

---

## How It Works

The main processing pipeline is:

```text
Input Curve
     ↓
Curve Sampling
     ↓
Uniform Sampling
     ↓
Complex Number Representation
     ↓
Fourier Transform
     ↓
Fourier Coefficients
     ↓
Sort Components by Magnitude
     ↓
Epicycle Reconstruction
     ↓
Animation
