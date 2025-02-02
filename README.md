# Speech Understanding Assignment

This repository contains two main components for audio classification and song spectrogram analysis.

## Urban Sound Classification

A comprehensive audio classification system based on the spectrogram obtained from the Short-Time Fourier Transform (STFT) using three different windowing techniques. The project includes multiple classification approaches and modules for effective audio classification.

### Components:

- **Feature Extraction Pipeline**: Extracts relevant features from audio data to prepare it for classification.
- **Pre-processing Module**: Pre-processes the raw audio data to ensure it is in a suitable format for feature extraction and model training.
- **Data**: Contains the dataset used for training and evaluation of the classification models.
  
### Classification Models:

- **Rectangular Window-based Classification**: Classifies audio based on the spectrogram generated using a rectangular window for STFT.
- **Hamming Window-based Classification**: Classifies audio using the Hamming window for STFT.
- **Hann Window-based Classification**: Classifies audio using the Hann window for STFT.

## Audio Feature Analysis Tool

A Python-based tool for analyzing and visualizing audio features of different music genres. The tool utilizes PyTorch and torchaudio libraries to process audio files and generate waveforms and spectrograms.

### Key Features:

- **Audio Feature Extraction and Visualization**: Extracts various features from audio files and visualizes them for analysis.
- **Waveform Generation**: Generates and visualizes the waveform of audio files.
- **Spectrogram Analysis**: Analyzes and visualizes spectrograms to understand the frequency content of the audio.
- **Genre-based Music Analysis**: Provides tools to classify and analyze music based on its genre using extracted features.

## Directory Structure

The repository contains the following structure:
 ```
├── audio_classification/
│   ├── feature_extraction.ipynb
│   ├── pre_process.ipynb
│   ├── Rectangular_window_based_classification.ipynb
│   ├── hamming_window_based_classification.ipynb
│   ├── hann_window_based_classification.ipynb
│   └── requirements.txt
├── song_analysis/
│   ├── Q2_TaskB.ipynb
│   └── requirements.txt
 ```


