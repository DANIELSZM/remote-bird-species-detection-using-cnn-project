# Bird Species Detection

## Overview
This project aims to detect bird species using a Convolutional Neural Network (CNN). The project includes resources for training the model and using it for detection with two different implementations:
1. Using a webcam as a source
2. Using an ESP32 camera as a source

## Project Structure
bird-species-detection/
│
├── model_training/
│   ├── train/
│   ├── test/
│   ├── val/
│   ├── train_model.ipynb
│
├── src/
│   ├── models/
│   │   ├── birdclassifier95.keras (to be downloaded, see instructions below)
│   ├── bird_detections_webcam.csv
│   ├── bird_detections_esp.csv
│   ├── detect_with_webcam.py
│   ├── detect_with_esp32.py
│
├── README.md
├── LICENSE

## Instructions

### Dataset
1. Download the dataset from Kaggle: [Kaggle Dataset Link](https://www.kaggle.com/link-to-dataset)
2. Place the downloaded images into the respective folders (`train`, `test`, `val`) inside the `model_training` directory. This allows you to run the Jupyter notebook with the dataset.

### Model Training
* Open the `train_model.ipynb` notebook in the `model_training` directory.
* Ensure the dataset is properly placed as described above.
* Run the notebook to train the CNN model.

### Pre-trained Model
To use the pre-trained model:
1. Download the pre-trained model from Google Drive: [Download birdclassifier95.keras](https://drive.google.com/link-to-your-file)
2. Place the downloaded model file in the `models` folder inside the `src` directory.

### Usage

#### Webcam Implementation
* Ensure you have the required dependencies installed.
* Navigate to the `src` directory.
* Run the following command:
    ```bash
    python detect_with_webcam.py
    ```

#### ESP32 Implementation
* Ensure you have the required dependencies installed.
* Navigate to the `src` directory.
* Run the following command:
    ```bash
    python detect_with_esp32.py
    ```

## Acknowledgements
* Dataset: [Kaggle Dataset](https://www.kaggle.com/link-to-dataset)
