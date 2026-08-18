# QuickNosis

On-device symptom-to-diagnosis Android prototype built as a solo summer project.

## What it does

- Trains a machine learning classification model on a public symptom-to-diagnosis dataset
- Packages the model into an Android app that runs inference locally on-device
- Lets a user input symptoms through a guided quiz and returns a predicted diagnosis
- No server or cloud inference required after the model is trained

## Stack

- **ML model:** TensorFlow
- **Android app:** Kotlin / Java, Android Studio
- **Model formats exported:** `joblib`, `ONNX`
- **Platform:** Android

## Context

This was a self-directed exploration of on-device ML. I taught myself Kotlin and Android
development from scratch to complete the project end-to-end, then presented the prototype
and slide deck at a George Mason research symposium as a solo presenter.

## Repository contents

- `model.ipynb`, `model2.ipynb` — training and experimentation notebooks
- `nb_model.joblib`, `rf_model.joblib`, `svm_model.joblib` — serialized scikit-learn models
- `nb_model.onnx`, `rf.onnx`, `svm_model.onnx` — ONNX exports
- `random_forest_model.ppml` — additional model artifact
- `Training.csv`, `Testing.csv` — dataset splits

## Status

Research prototype, not actively maintained. Kept public as proof of work for end-to-end
ML + Android delivery.
