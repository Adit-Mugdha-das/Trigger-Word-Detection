# Trigger Word Detection

This repository contains the programming assignment from **Week 3** of **Course 5: Sequence Models** in the [Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning) by Andrew Ng on Coursera.

## Overview

In this assignment, a trigger word detection model is built using spectrograms and a sequence model based on LSTM networks.  
The system is trained to detect the word "activate" in continuous audio streams.

Key concepts covered:
- Preprocessing audio signals into spectrograms
- Building a training dataset with trigger and non-trigger segments
- Designing a deep LSTM network for sequence prediction
- Post-processing predictions to detect the activation word

## Contents

- `Trigger_word_detection_v2a.ipynb` – Jupyter notebook implementing the full pipeline
- `td_utils.py`, `test_utils.py` – Helper utilities for spectrograms and model evaluation
- `models/` – Contains the trained trigger word detection model
- `XY_train/`, `XY_dev/` – Small versions of training and development datasets
- `audio_examples/` – Example audio files
- `chime_output.wav`, `insert_test.wav` – Processed test audio examples

## Dataset and Model Notice

To comply with GitHub's 100MB file size limitations:
- Only a **reduced version** of the training and development datasets is included (first few samples).
- Only the **final trained model** (`tr_model.h5`) is kept in the `models/` directory.
- Unnecessary `.wav` files (`tmp.wav`, `train.wav`) and intermediate models (`model.h5`, `model_new8.h5`, `.json`) have been removed.
- `.DS_Store` and temporary system files were deleted.
- Audio examples have been minimized to essential demonstration files.

Full results can still be reproduced by regenerating datasets and retraining the model following the steps in the notebook.

## Technologies Used

- Python 3
- TensorFlow / Keras
- NumPy
- Librosa (for audio processing)

## Course Information

- Course: Sequence Models (Course 5 of 5)
- Specialization: Deep Learning Specialization
- Instructor: Andrew Ng
- Platform: Coursera
- Institution: DeepLearning.AI

## License

This repository is based on educational material provided by DeepLearning.AI through Coursera. It is intended for educational and personal use only and should not be used for commercial purposes.

---
