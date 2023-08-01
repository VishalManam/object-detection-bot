# Object Finder Bot using Feature Matching and Detection Algorithms

## Introduction

The Object Finder Bot is a Python-based application that utilizes Feature Matching and Detection Algorithms to locate a target object within a reference image. This powerful bot can assist users in identifying specific objects within complex images, making it a valuable tool for various applications such as computer vision, image analysis, and object recognition.

## Features

- User-friendly Graphical User Interface (GUI) built using Tkinter.
- Supports matching a target object against a reference image.
- Utilizes Feature Matching and Detection Algorithms for accurate object identification.
- Displays detailed results, including matched keypoints and bounding box around the target object.
- Provides options for adjusting algorithm parameters to fine-tune the matching process.
- Allows users to load custom target and reference images from their local storage.

## How it Works

The Object Finder Bot uses the following main steps to find the target object in the reference image:

1. **Input**: The user provides the target image and the reference image via the GUI.

2. **Feature Detection**: The bot employs feature detection algorithms, such as SIFT (Scale-Invariant Feature Transform) or ORB (Oriented FAST and Rotated BRIEF), to identify key feature points in both the target and reference images.

3. **Feature Matching**: The bot matches the key feature points between the target and reference images using techniques like Brute-Force Matching, FLANN (Fast Library for Approximate Nearest Neighbors) Matching, or other efficient algorithms.

4. **Filtering and Validation**: The bot filters out incorrect matches and validates the reliable matches based on parameters like distance ratio or homography.

5. **Visualization**: The bot visualizes the matched keypoints and draws a bounding box around the target object in the reference image.

6. **Result Display**: The final result is displayed on the GUI, showing the reference image with the identified target object highlighted.

## Getting Started

Follow these steps to set up and run the Object Finder Bot on your local machine:

1. Clone the repository: `git clone https://github.com/VishalManam//object-detection-bot.git`
2. Navigate to the project directory: `cd object-detection-bot`
3. Install the required dependencies: `pip install -r requirements.txt`
4. Run the application: `python object_detection_bot.py`

## Usage

1. Launch the Object Finder Bot application by executing the `object_detection_bot.py` script.
2. Click on the "Load Target Image" button to load the image of the object you want to find in the reference image.
3. Click on the "Load Reference Image" button to load the image in which you want to search for the target object.
4. Adjust the algorithm parameters (if required) using the sliders or input fields provided in the GUI.
5. Click the "Find Object" button to initiate the feature matching process.
6. The result will be displayed in a new window, showing the reference image with the identified target object highlighted.


## Example Input

![Reference Image](https://raw.githubusercontent.com/VishalManam/object-detection-bot/main/images/ikigai.jpg)
![Target Image](https://raw.githubusercontent.com/VishalManam/object-detection-bot/main/images/ikigai%20and%20other%20books.jpg)

## Example Output

![Keypoints on Reference Image](https://raw.githubusercontent.com/VishalManam/object-detection-bot/main/images/image1_with_key_points.jpg)
![Keypoints on Target Image](https://raw.githubusercontent.com/VishalManam/object-detection-bot/main/images/image2_with_key_points.jpg)
![Matches between Image](https://raw.githubusercontent.com/VishalManam/object-detection-bot/main/images/matches.jpg)
![Detected Object](https://raw.githubusercontent.com/VishalManam/object-detection-bot/main/images/ikigai_detected.jpg)

## Algorithm Configuration

The Object Finder Bot allows users to fine-tune the feature matching process by adjusting the following algorithm parameters:

- Feature Detector (SIFT, ORB, etc.)
- Matcher (Brute-Force, FLANN, etc.)
- Filtering Thresholds
- Homography Thresholds

## Contributions

Contributions to this project are welcome! If you have any suggestions or improvements, feel free to create a pull request. Please ensure to follow the project's code of conduct.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The bot was inspired by the incredible work in computer vision and object recognition.
- Thanks to the developers of OpenCV, NumPy, and Tkinter for providing powerful libraries for image processing and GUI development.
