# Binary classification

Trains a small neural network to classify rows from vibration frequency and temperature.

## What it does

- The label column is 0 or 1. Frequency is stored in hertz and temperature in degrees Celsius.
- Splits the rows, scales the features, and trains a Keras sequential network with L2 regularization.
- Reports accuracy, precision, recall, F1, a confusion matrix, and an ROC curve.

## Layout

- `notebooks/binary_classification.ipynb` — the network and the metrics
- `data/data.csv` — frequency, temperature, and label

## Run

From the repository root:

```bash
pip install -r requirements.txt
jupyter notebook notebooks/binary_classification.ipynb
```

The notebook also runs if its working directory is `notebooks/`.

## Stack

Python, pandas, NumPy, scikit-learn, TensorFlow, Matplotlib, Jupyter. Written for MEEN 423.
