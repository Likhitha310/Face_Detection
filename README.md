Face Detection and Recognition

This project implements a real-time face detection and recognition system using Python. Leveraging libraries such as OpenCV and machine learning algorithms, the system can detect faces in live video streams and recognize known individuals.

 Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

 Features

  Real-time Face Detection: Utilizes webcam input to detect faces in live video streams.
  Face Recognition: Identifies and distinguishes between known individuals using machine learning algorithms.
  Data Generation: Includes tools for generating and storing facial data for training purposes.

## Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - OpenCV: For image and video processing
  - NumPy: For numerical computations
  - Scikit-learn: For implementing machine learning algorithms

 Project Structure

The repository includes the following key files:

 `face_detection.py`: Script for detecting faces in real-time using a webcam.
 `face_recognition_knn.py`: Script implementing face recognition using the k-nearest neighbors algorithm.
 `realtime_data_generation.py`: Script to capture and store facial images for building a training dataset.
 `haarcascade_frontalface_alt.xml`: Pre-trained Haar Cascade classifier for frontal face detection.
 `req.txt`: File listing all the dependencies required to run the project.

Setup Instructions

To set up the project on your local machine, follow these steps:

1. Clone the Repository  
   Open your terminal and run the following commands:
   ```bash
   git clone https://github.com/Likhitha310/Face_Detection.git
   cd Face_Detection
   ```

2. Install Dependencies  
   Ensure that Python is installed on your system. Then, install the required packages by running:
   ```bash
   pip install -r req.txt
   ```

3. Generate Training Data 
   Run the `realtime_data_generation.py` script to capture facial images and build your training dataset:
   ```bash
   python realtime_data_generation.py
   ```
   Follow the on-screen instructions to capture images.

4. Train the Recognition Model  
   After generating the dataset, execute the `face_recognition_knn.py` script to train the k-nearest neighbors model:
   ```bash
   python face_recognition_knn.py
   ```
   This will train the model and save it for future use.

5. Run the Face Detection Application 
   Start the real-time face detection application using:
   ```bash
   python face_detection.py
   ```
   This will launch the webcam interface for face detection and recognition.

 Usage

Real-Time Detection and Recognition: Once the application is running, the system will detect faces in the webcam feed and recognize known individuals based on the trained model.
Data Generation: Use the data generation script to add new individuals to the dataset as needed.

 Contributing

Contributions are welcome! If you'd like to enhance the project, please fork the repository, create a new branch, and submit a pull request with your changes.

 License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---
