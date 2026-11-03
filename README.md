# BN4601-AI-Cardiology-

# CardioLens App Integration

This branch contains:
- Gradio clinician-facing interface
- ECG waveform-model integration
- Clinical Detective conversation flow
- Structured report generation

## ECG input

The app expects:
- NumPy .npy file
- Shape: (12, 1000)
- Sampling frequency: 100 Hz
- Units: mV
- Lead order: I, II, III, AVR, AVL, AVF, V1, V2, V3, V4, V5, V6

## Current limitation

The waveform model provides rhythm annotations only.
The explanation and conversation layer is currently a placeholder
until the pretrained VLM is integrated.

## How to run

Install dependencies:

pip install -r requirements.txt

Run:

python app.py
