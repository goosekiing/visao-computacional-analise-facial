# Computer Vision: Facial Analysis

This repository contains a project focused on facial analysis using the MediaPipe library to detect facial landmarks and the OpenCV library to capture real-time images from the webcam. The goal of the project is to create an algorithm capable of identifying if people are drowsy based on facial features.

## Project Overview

### Drowsiness Detection
The project uses two research papers available in the repository, which conclude that people who blink less than 10 times per minute are likely to be drowsy, and that partially open eyes also indicate drowsiness. Using the facial landmarks of the eyes obtained through MediaPipe, a blink counter per minute is created, and the Eye Aspect Ratio (EAR) is calculated. If the blink rate is below 10 blinks per minute and the eyes have a low EAR, an alert is generated indicating that the user might be drowsy. The code also includes a calculation for the Mouth Aspect Ratio (MAR) to indicate yawning. A high MAR suggests that the user yawned, which also signifies potential drowsiness.

## Course Details
This project was completed as part of the 'Computer Vision with OpenCV' course on Alura. For more information about the course, visit [Alura](https://cursos.alura.com.br/formacao-visao-computacional-opencv).

## Objectives Achieved
- Understand how to integrate the webcam with Python code using the OpenCV library.
- Learn about the Face Mesh solution from the open-source framework MediaPipe.
- Discover how to perform face detection with MediaPipe.
- Understand facial landmarks and how to manipulate them.
- Build a drowsiness classifier algorithm.

## Project Structure
The directory structure of the project is as follows:
```
visao-computacional-analise-facial/
│
├── Drowsiness Detection According to the Number of Blinking Eyes Specified From Eye Aspect Ratio Value Modification.pdf
├── project-01.ipynb
├── README.md
├── Real-Time Eye Blink Detection using Facial Landmarks.pdf
```

## Setup Instructions
1. Clone the repository:
   ```sh
   git clone https://github.com/goosekiing/visao-computacional-analise-facial.git
   ```
2. Navigate to the project directory:
   ```sh
   cd visao-computacional-analise-facial
   ```
3. Create a virtual environment and activate it:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
4. Install the required libraries:
   ```sh
   pip install -r requirements.txt
   ```

## Running the Notebook
1. Ensure your webcam is connected and working.
2. Run the Jupyter Notebook:
   ```sh
   jupyter notebook
   ```
3. Open `project-01.ipynb` in Jupyter Notebook and execute the cells to run the project.

## Technologies Used
- Python (v3.8.10)
- Jupyter Notebook
- OpenCV (cv2 v3.4.8)
- MediaPipe (v0.8.11)
- Numpy

## Language
The language used in this project is Brazilian Portuguese (pt-br).

## Author
GitHub Username: [goosekiing](https://github.com/goosekiing)
