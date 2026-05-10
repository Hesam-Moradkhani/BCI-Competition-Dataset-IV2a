# BCI Competition IV Dataset 2a for Jupyter Notebook
This repository provides a beginner-friendly guide to work with the **BCI Competition 2008 - Dataset IV 2a** using original GDF files. Perfect for students starting with EEG and motor imagery BCI!

## About the Dataset
You first need to read the original paper: http://bbci.de/competition/iv/desc_2a.pdf

This dataset contains EEG recordings of **motor imagery tasks** from 9 subjects. Each subject imagined moving different body parts:

| Class | Task | Event Code |
|-------|------|------------|
| 1 | ✋ Left Hand | 769 |
| 2 | ✋ Right Hand | 770 |
| 3 | 🦶 Both Feet | 771 |
| 4 | 👅 Tongue | 772 |

### Dataset Characteristics
- **9 subjects** (A01T to A09T)
- **48 trials per subject** (12 for each class)
- **Sampling rate**: 250 Hz
- **22 EEG channels** + 3 EOG channels
- **Each trial duration**: ~6 seconds

### Event Codes
| Code | Description |
|------|-------------|
| 768  | Start of trial |
| 769  | Cue onset - Left hand |
| 770  | Cue onset - Right hand |
| 771  | Cue onset - Foot |
| 772  | Cue onset - Tongue |
| 783  | Unknown |
| 1023 | Reject trial |

# Install requirements
pip install -r requirements.txt
