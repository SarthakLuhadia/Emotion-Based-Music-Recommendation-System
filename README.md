# Emotion-Based-Music-Recommendation-System

This project uses computer vision techniques to recognize facial and hand landmarks to determine a user's emotion and recommend music accordingly. The system includes a data collection script, a neural network model for emotion classification, and a Streamlit application for live emotion recognition and music recommendation.

## Table of Contents

- [Installation](#installation)
- [Data Collection](#data-collection)
- [Model Training](#model-training)
- [Emotion Recognition and Music Recommendation](#emotion-recognition-and-music-recommendation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/emotion-based-music-recommendation.git
    cd emotion-based-music-recommendation
    ```

2. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Data Collection

To collect data for training the emotion classification model, run the data collection script:

```bash
python collect_data.py
```

This script captures video from your webcam, processes it using MediaPipe to extract facial and hand landmarks, and saves the data to a `.npy` file. You will be prompted to enter the name of the data.

## Model Training

After collecting the data, you can train the model using the following script:

```bash
python train_model.py
```

This script loads the collected data, preprocesses it, trains a neural network model, and saves the trained model to `model.h5`. It also saves the label encoding to `labels.npy`.

## Emotion Recognition and Music Recommendation

The main application for emotion recognition and music recommendation is built using Streamlit and can be run with:

```bash
streamlit run app.py
```

This application captures live video from your webcam, recognizes your emotion using the trained model, and recommends music based on the recognized emotion. 

## Usage

1. Run the Streamlit application:

    ```bash
    streamlit run app.py
    ```

2. Enter the desired language and singer for music recommendation.

3. Allow the application to capture your emotion through the webcam.

4. Click the "Recommend me songs" button to get music recommendations based on your emotion.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

Please replace `https://github.com/yourusername/emotion-based-music-recommendation.git` with your actual GitHub repository URL.
