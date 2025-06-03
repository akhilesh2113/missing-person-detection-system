# missing-person-detection-system
This project pioneers a Missing Person Detection System that integrates real-time image and video analysis with intelligent data processing. It's designed to act as a crucial force multiplier for law enforcement and rescue teams, providing rapid identification capabilities in critical moments.

# PROJECT_STRUCTURE
face_reconition_lost_person_find/
├── app.py                      # Main application logic for face detection and recognition
├── main.py                     # Starts the system and initiates recognition
├── train.py                    # Trains the recognition model using provided images
├── haarcascade_frontalface_default.xml  # Haar cascade classifier for face detection
├── att_faces/                  # Folder containing face images for training
│   └── [person_name]/          # Each folder contains images of an individual

# FEATURES
Face detection using OpenCV's Haar cascade.
Face recognition using LBPH (Local Binary Patterns Histograms).
Training support with labeled face images.
Real-time face recognition using a webcam.
Image dataset organized by person names.

# REQUIREMENTS
Python 3.7+
OpenCV
NumPy

Install the dependencies:
pip install opencv-python numpy

#  HOW TO USE 
1. Add Training Images
Place images of individuals in att_faces/[person_name]/.
Each subfolder should be named after the person.

2. Train the Model
python train.py

3. Start Recognition
python main.py

4. (Optional) Run App Interface
python app.py

# DATASET FORMAT
Each person should have their own folder inside att_faces/. For example:
att_faces/
├── akhilesh/
│   ├── 1.png
│   ├── 2.png
│   └── ...
├── john/
│   ├── 1.png
│   ├── 2.png
│   └── ...

# USE CASES
Reuniting lost children or elderly people with their families.
Assisting NGOs and law enforcement in identifying individuals.
Monitoring and alert systems at public places.

# FUTURE REQUIREMENTS
Integrate with a database or cloud storage.
Implement a front-end GUI for easier usage.
Use deep learning-based face recognition models for higher accuracy.







