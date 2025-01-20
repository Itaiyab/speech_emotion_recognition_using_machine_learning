Speech recognition using machine learning 

This project is a Speech Emotion Recognition System that uses audio recordings to classify human emotions based on features extracted from speech. It leverages machine learning, specifically a Multi-Layer Perceptron (MLP) classifier, to predict emotions such as calm, happy, fearful, and disgust. Here's a brief overview:

Key Components
Feature Extraction:

Uses the librosa library to extract important audio features:
MFCC (Mel Frequency Cepstral Coefficients): Captures the timbre of the sound.
Chroma: Represents pitch classes.
Mel Spectrogram: Represents the energy in different frequency bands.
These features are crucial for differentiating between emotions in speech.
Dataset:

The project assumes the use of the RAVDESS dataset or a similarly labeled dataset.
Audio file names encode emotion labels (e.g., 03 for happy), which are mapped to specific emotions.
Machine Learning Model:

A Multi-Layer Perceptron (MLP) is trained on the extracted features.
The model uses a single hidden layer and adaptive learning to classify emotions.
Real-Time Emotion Prediction:

The script includes functionality to record audio from a microphone.
It extracts features from the recorded audio and predicts the emotion using the trained model.
Workflow
Data Loading:
The dataset is loaded, and features are extracted from audio files.
Training and Testing:
The data is split into training and testing sets.
The MLP model is trained on the training data and evaluated on the testing data.
Real-Time Emotion Detection:
Users can record their speech using a microphone.
The system predicts the emotion from the recorded audio.
Applications
Customer Service: Analyze customer sentiment during calls.
Mental Health: Detect emotional changes to support therapy or well-being monitoring.
Interactive Systems: Enhance human-computer interaction by recognizing emotions in speech.
Requirements
Python libraries: librosa, soundfile, numpy, scikit-learn, sounddevice, wavio.
An audio dataset with labeled emotions.

A microphone for real-time recording.


Codespaces
https://upgraded-fishstick-jvvg9qrrgxv2pw9j.github.dev/

To deploy this project run

```bash
  python emotion_recognition.py

```

```bash
   pip install numpy librosa soundfile sounddevice wavio scikit-learn
```

