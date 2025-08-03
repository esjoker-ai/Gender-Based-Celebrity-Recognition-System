# Gender-Based-Celebrity-Recognition-System
This repository contains a Python project for a gender-based celebrity recognition system. The core of the system is a pipeline that integrates two distinct machine learning models:

Gender Detection: A YOLO model is used to detect people in an image or video stream. It then classifies the detected person as either male or female. The system provides visual feedback by drawing a bounding box around the person, colored green for females and blue for males.

Celebrity Classification: The output from the YOLO model is fed into a classifier.h5 model. This model is trained to recognize 12 specific celebrities. It identifies which of the 12 classes the detected person belongs to.

The entire process is orchestrated within a main.ipynb Jupyter Notebook, which serves as the pipeline connecting the gender detection and celebrity classification models to produce the final result.

Project Flow
Input: An image or video stream containing one or more people.

Step 1: The YOLO model processes the input to detect a person and predict their gender.

Step 2: A bounding box is drawn around the person, with a color (green for female, blue for male) indicating the detected gender.

Step 3: The cropped image of the person is passed to the classifier.h5 model.

Step 4: The classifier model predicts which of the 12 celebrities the person is.

Output: The final output is an image or video frame with colored bounding boxes and labels identifying both the gender and the celebrity name.
