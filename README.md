# Emotion and Gender Detection with DeepFace and OpenCV

## Project Overview
This application leverages the DeepFace library with OpenCV and Tkinter to perform real-time emotion and gender detection via webcam. By analyzing each frame from the video feed, it identifies faces and returns a probability distribution of different emotions and gender, displaying this data overlaid on the video.

## Setup and Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/DeAngelisDavide/hashGraph.git
    cd hashGraph
    ```
2. Install required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the program:
    ```bash
    python main.py
    ```

## Detailed Model Information

### 1. **Emotion Detection**
   - **Model:** DeepFace uses multiple pre-trained models (such as VGG-Face, Google FaceNet, and others) and, by default, combines outputs for accurate emotion classification. 
   - **Emotions Detected:** Happiness, sadness, surprise, anger, fear, disgust, neutral.
   - **Output:** The model provides a probability distribution for each emotion based on face analysis, allowing the code to determine which emotion is most likely.

### 2. **Gender Detection**
   - **Model:** Gender classification in DeepFace uses robust models, such as FaceNet, that categorize gender into binary classes: male or female.
   - **Output:** This model outputs the probability distribution for both classes (male and female), which is displayed beneath each detected face.

### Backend Detection Model
- **Backend Used:** RetinaFace is used as the face detection backend, which is known for its accuracy.


## Requirements
The following Python libraries are required to run the application. They are included in the `requirements.txt` file:
- `opencv-python`
- `deepface`
- `pillow`
- `tkinter` (pre-installed with Python)

## Acknowledgments
Special thanks to the creators of the DeepFace library for making facial recognition models accessible to the community.
