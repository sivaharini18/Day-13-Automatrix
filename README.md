
# Day-13-Automatrix

## Day 13: TensorFlow Lite Iris Classifier

This project deploys a compact TensorFlow Lite model for classifying Iris flower samples using an ESP32.

The model accepts four normalized input features and produces scores for three flower classes.

## Model Details

- **Inputs:** 4 normalized features
- **Outputs:** 3 classes
- **Model size:** 5,040 bytes
- **Operations:** Fully connected and softmax

## Project Files

- `model.h` — generated model data and sample input arrays.
- `sketch.ino` — ESP32 inference code.
- `diagram.json` — Wokwi ESP32 configuration.
- `python.py` — model training and conversion code, if included.

## How It Works

1. The input sample contains four normalized feature values.
2. The TensorFlow Lite model processes the input.
3. The model produces scores for three Iris classes.
4. The classifier selects the class with the highest score.
5. The ESP32 displays the input values and predicted class in the Serial Monitor.

## Run the Project

1. Open the Wokwi ESP32 simulation.
2. Start the simulation.
3. Open the Serial Monitor.
4. View the input values and predicted flower class.

## Wokwi Simulation
Run the simulation 
https://wokwi.com/projects/469378874786036737

## Note

The model file, input format, and output handling must match the generated model used by the ESP32 code.

