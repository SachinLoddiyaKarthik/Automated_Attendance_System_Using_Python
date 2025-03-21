# Automated Facial Recognition Attendance System

A time-efficient attendance system that uses facial recognition technology to automate the attendance marking process, with cloud synchronization capabilities for remote access.

## Overview

This project implements an automated attendance system using facial recognition technology. It identifies individuals from video footage, marks their attendance in a local database, and synchronizes the data to the cloud using Simple Mail Transfer Protocol (SMTP). The system aims to replace traditional manual attendance systems, reducing time consumption and human error.

## Key Features

- **Face Detection and Recognition**: Uses Haar Cascade classifiers and AdaBoost algorithm for accurate face detection
- **Cloud Synchronization**: Attendance records are sent via email, enabling cloud storage and remote access
- **Time-Stamped Records**: Captures the exact date and time when attendance is marked
- **Scalable Database**: Can store multiple facial patterns in trainsets for comparison
- **Real-Time Processing**: Processes video footage in real-time for immediate attendance marking

## Technologies Used

- **Python**: Primary programming language
- **OpenCV**: For image processing and face detection
- **Haar Cascade**: Pre-compiled libraries for facial pattern recognition
- **AdaBoost Algorithm**: For combining multiple classifiers to improve accuracy
- **SMTP**: For email-based cloud synchronization
- **Anaconda**: For environment management

## System Requirements

### Hardware Requirements
- Computer with Windows 10 64-bit Home Edition
- Intel Core i3-3120M dual-core processor (2.5GHz, 3MB L3 cache) or better
- Intel HD4000 Graphics Card or equivalent
- 4GB DDR3 System Memory or higher
- Webcam with 2.4MP quality or above
- 2.4GHz Network Band with 1MBps network connectivity

### Software Requirements
- Anaconda and its supporting environments
- Python
- Visual Studio C++
- Haar Cascade library
- Mail transfer Protocols and supporting libraries
- OpenCV

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/SachinLoddiyaKarthik/Automated_Attendance_System_Using_Python.git
   ```

2. Create and activate a Conda environment:
   ```
   conda create -n face_attendance python=3.8
   conda activate face_attendance
   ```

3. Install required packages:
   ```
   pip install opencv-python
   pip install numpy
   pip install [other required packages]
   ```

4. Download the Haar Cascade XML files and place them in the project directory

## Usage

### Creating Trainsets

1. Run the trainset creation script:
   ```
   python create_trainset.py
   ```

2. Follow the prompts to capture 30 frames of each individual's face
3. The system will process these frames and create facial pattern trainsets

### Marking Attendance

1. Run the attendance system:
   ```
   python mark_attendance.py
   ```

2. The system will access the webcam and begin detecting faces
3. Recognized individuals will have their attendance marked with a timestamp
4. Attendance records will be automatically stored in the local database and sent via email

## How It Works

1. **Trainset Creation**: The system captures 30 frames of each person's face and processes them using Haar Cascade and AdaBoost algorithms to create a strong facial pattern recognition model.

2. **Face Detection**: When the attendance system is running, it uses Haar Cascade Frontal face detection to identify faces in the video feed.

3. **Pattern Matching**: The system compares detected faces with the stored trainsets.

4. **Attendance Marking**: If a match is found, the system marks attendance in the local database with a timestamp.

5. **Cloud Synchronization**: The attendance record is sent via email, allowing for cloud storage and remote access.

## Advantages

- Eliminates time-consuming manual attendance processes
- Reduces human error in attendance marking
- Provides digital records that can be accessed anywhere, anytime
- Timestamps provide accurate record of when individuals were present
- Cloud synchronization ensures data availability across platforms

## Future Enhancements

- Implementation of DRLBP (Dominant Rotated Local Binary Pattern) for improved accuracy
- Integration of SIFT (Scale Invariant Feature Transform) for better face classification
- Mobile application for monitoring attendance remotely
- Addition of authentication layers for increased security
- Integration with existing educational/organizational management systems

