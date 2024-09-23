## Project Overview
This Flask web application allows users to upload an image of the moon, and it predicts the lunar day within the synodic month based on the uploaded image. It utilizes a pre-trained Convolutional Neural Network (CNN) model to perform the classification.

## Features
- Upload an image (JPG or JPEG format) of the moon to receive a lunar day prediction.
- Display the predicted lunar day and the associated probability.
- Dynamic carousel for user interaction and a clean UI for uploading files.

## Technologies Used
- Python (Flask)
- FastAI for deep learning
- HTML/CSS and JavaScript for the frontend
- Model trained on a ResNet18 architecture
- Image input processing using the `PILImage` from FastAI

## Setup and Installation

### Prerequisites
- Python 3.7+
- Install dependencies:
    ```bash
    pip install Flask fastai
    ```

### Clone the Repository
```bash
git clone https://github.com/your-username/moon-phase-prediction-app.git
cd moon-phase-prediction-app
```

### Model
Make sure the pre-trained model (`19yearsExportGray100epoch.pkl`) is placed in the `./static/` directory.

### Running the Application
1. Start the Flask server:
    ```bash
    python app.py
    ```
2. Open a web browser and navigate to `http://127.0.0.1:5000`.

## Usage
1. On the homepage, click "Choose a file" and upload an image of the moon in either `.jpg` or `.jpeg` format.
2. Submit the image to receive the predicted lunar day and its probability.
3. The result will be displayed as: 
    ```
    Prediction: Day X, Probability: 0.YYYY
    ```

## File Upload Guide
- Ensure the uploaded file is in `.jpg` or `.jpeg` format.
- If an invalid file format is uploaded, the server will respond with an error.

## Contributing
Feel free to contribute to this project by opening issues or submitting pull requests. For major changes, please open a discussion beforehand to ensure the changes fit the project’s scope.

## License
This project is licensed under the MIT License.
