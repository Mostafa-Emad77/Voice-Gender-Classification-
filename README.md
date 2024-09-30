# Voice Activity Detection and Gender Classification Pipeline

This project implements an end-to-end pipeline for detecting voice activity, reducing noise, normalizing audio, and classifying the speaker's gender using pre-trained models.

## Overview

The pipeline integrates the following tasks:
1. **Voice Activity Detection (VAD)**: Detects segments in the audio where speech is present using the Silero VAD model.
2. **Noise Reduction**: Applies noise reduction techniques to enhance the audio quality.
3. **Audio Normalization**: Normalizes the audio for consistent volume levels.
4. **Gender Classification**: Classifies the detected voice as either male or female using a pre-trained Wav2Vec2 model.

## Key Features
- **Voice Detection**: Automatically identifies whether an audio file contains speech or not.
- **Noise Reduction**: Improves audio clarity by reducing background noise.
- **Audio Normalization**: Ensures the audio is at a consistent volume for accurate processing.
- **Gender Classification**: Predicts the gender of the speaker with high accuracy using a fine-tuned speech model.

## Workflow
1. Load an audio file (WAV format).
2. Detect speech segments using Silero VAD.
3. If speech is detected:
    - Apply noise reduction.
    - Normalize the audio.
    - Classify the gender of the speaker.
4. Output the predicted gender along with any detected voice segments.

## Models Used
- **Silero VAD**: A pre-trained model for voice activity detection.
- **Wav2Vec2**: A fine-tuned pre-trained model for gender classification based on speech.

## Applications
- **Speech Processing**: Use this pipeline for tasks involving speech detection and speaker identification.
- **Audio Preprocessing**: Clean and normalize audio before further analysis or modeling.
- **Gender Analytics**: Gain insights into the gender of speakers in audio datasets.

## Requirements
- Python 3.x
- Torch
- Transformers
- Torchaudio
- Noisereduce


