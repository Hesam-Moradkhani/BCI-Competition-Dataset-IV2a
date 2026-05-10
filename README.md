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

## Event Structure
A typical trial looks like this in the timeline:

Time (seconds):
0s     → Trial starts (event 768)
2s     → Cue onset (769-772: imagery task starts)
2-6s   → Motor imagery period
6s     → Trial ends

## Install requirements
pip install -r requirements.txt

## Tutorial Notebooks
This repository includes 4 Jupyter notebooks designed for beginners:

- **01_loading_gdf_files.ipynb** - Load GDF files and understand their structure
- **02_exploring_eeg_data.ipynb** - Basic EEG data exploration and visualization
- **03_visualizing_trials.ipynb** - Extract and visualize individual trials
- **04_extracting_motor_imagery_trials.ipynb** - Complete pipeline for trial extraction


⭐ Most important channels for motor imagery (sensorimotor cortex)
