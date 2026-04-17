EyeMe: Eye-Tracking Assistive TechnologyEyeMe is an AI-driven system designed to assist individuals with physical disabilities. 
It enables hands-free interaction with electronic devices by translating real-time eye movements and gaze estimation into control commands.

The project integrates Computer Vision, Deep Learning, and Embedded Systems to provide an accessible interface for those with limited mobility.
Key Features:
Real-time Gaze Tracking: 
Precise detection of pupil position and movement.
Device Control: 
Converts eye movement into interface navigation or device triggers.
Assistive UI: 
Optimized to reduce eye strain while maintaining interaction accuracy.
Mobile Integration: 
Includes a dedicated app for configuration and remote device management.

Technical Architecture:
1. Computer Vision & Deep LearningThe system uses a multi-stage approach for gaze estimation:
2. Face & Landmark Detection: Utilizes Dlib’s 68-point facial landmark predictor to identify eye regions.
3. Gaze Estimation Model: Employs L2CSNet (a two-stage network) for robust gaze prediction across various head poses.
4. Dataset: The model was trained/evaluated on the Gaze360 dataset to ensure generalization in real-world scenarios.

Software StackLanguage: 
PythonLibraries: 
OpenCV (Image processing), Dlib (Face detection), NumPy (Data manipulation).

Hardware :IntegrationImplementation involves Embedded Systems to bridge the AI logic with physical device control.

Performance Metrics:
Based on testing with the Gaze360 dataset, the system achieved:
Mean Error: 9.9^
Validation Performance: 7.9 (as documented in experimental results).


Installation & Setup Prerequisites:
Python 3.x
Required libraries:
pip install opencv-python dlib numpy


Required Model File:
Due to GitHub's file size limits, the mandatory model file shape_predictor_68_face_landmarks.dat (~96MB) is not included in this repository.

Usage:
Run the main script to start the eye-tracking 
interface:
python src/main.py


The TeamInstitution: 
Beni-Suef University, Faculty of Computer Science & AI (IS Section).
Supervisors:
Dr. Amal FouadEng. 
Abanop Gerges

Developers:
Ahmed Ali Shaban
Alaa Sayed Abd Al-Kareem
Omnia Mohammed Sayed
Yomna Magdy Mohammed
Mohammed Ibrahim Mohammed
Ghada Ragab Diab
Reham Mohammed Ahmed
Yomna Mahmoud Mohamed Abdelhafiez


Note: This project was developed as a 2024 Graduation Project to demonstrate the potential of AI in improving accessibility and real-time environmental communication.
