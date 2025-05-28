
# 🤖 Automated Facial Recognition Attendance System

![Python](https://img.shields.io/badge/Python-3.8-blue?logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-vision-green?logo=opencv&logoColor=white)
![SMTP](https://img.shields.io/badge/SMTP-Email%20Sync-orange)
![Real-Time](https://img.shields.io/badge/Real--Time-Processing-red)
![Cloud](https://img.shields.io/badge/Cloud-Sync-blueviolet)

A smart, time-efficient system for automating attendance through facial recognition, with real-time processing and cloud synchronization via email.

---

## 📌 Project Overview

This project implements an AI-powered attendance system that:
- Detects and recognizes faces using live webcam feeds
- Marks attendance automatically in a local database
- Syncs attendance records to the cloud using SMTP
- Reduces manual effort and eliminates human errors

---

## 🎯 Key Features

| Feature | Description |
|--------|-------------|
| 🎥 **Face Detection & Recognition** | Uses Haar Cascade & AdaBoost for robust facial recognition |
| 📬 **Cloud Sync via Email** | Sends attendance records through SMTP for remote access |
| 🕒 **Timestamped Logs** | Logs exact date and time of each attendance entry |
| 🗃️ **Trainable Facial Database** | Add multiple users with 30-frame training sets |
| ⚡ **Real-Time Processing** | Attendance marked instantly via live video feed |

---

## 🛠️ Technology Stack

### 🧠 Core Components
- **Python 3.8**
- **OpenCV** – Image processing & facial recognition
- **Haar Cascade Classifiers** – Face detection
- **AdaBoost** – Classifier enhancement
- **SMTP** – Email-based cloud sync
- **SQLite / CSV** – For storing attendance records

### 🧰 Development Tools
- **Anaconda** – Environment management
- **Visual Studio C++** – For OpenCV compilation support

---

## 🧾 System Requirements

### 💻 Hardware
- Windows 10 64-bit OS
- Intel i3-3120M processor or higher
- 4GB RAM (minimum)
- Integrated/External webcam (2.4MP+)
- Stable 2.4GHz Wi-Fi

### 🧑‍💻 Software
- Python 3.8+
- OpenCV
- Anaconda
- SMTP libraries
- Haar Cascade XML files

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/SachinLoddiyaKarthik/Automated_Attendance_System_Using_Python.git
cd Automated_Attendance_System_Using_Python
````

### 2️⃣ Set Up Your Environment

```bash
conda create -n face_attendance python=3.8
conda activate face_attendance
```

### 3️⃣ Install Dependencies

```bash
pip install opencv-python numpy
```

### 4️⃣ Add Haar Cascade Files

Download and place Haar Cascade XML files in the project directory (e.g., `haarcascade_frontalface_default.xml`).

---

## 🧪 How It Works

### 🛠️ Trainset Creation

```bash
python create_trainset.py
```

* Capture 30 face images per user
* Images saved to trainset directory for matching

### ✅ Mark Attendance

```bash
python mark_attendance.py
```

* Webcam captures live feed
* Face detection + recognition
* Attendance recorded locally and sent via email

---

## 📦 Output Example

| Name  | Date       | Time     |
| ----- | ---------- | -------- |
| Alice | 2025-05-27 | 09:03 AM |
| Bob   | 2025-05-27 | 09:07 AM |

Files are saved as:

```
attendance_2025-05-27.csv
```

and emailed to designated admin.

---

## 💡 Future Enhancements

* 🔍 **DRLBP**: Enhance recognition with Dominant Rotated Local Binary Patterns
* 🧠 **SIFT**: Use Scale-Invariant Feature Transform for advanced classification
* 📱 **Mobile App**: Remote attendance monitoring and push notifications
* 🔐 **User Authentication**: Add login security layers
* 🏫 **System Integration**: Link with ERP/HRMS/University portals

---

## 🤝 Contributing

We welcome your contributions!

1. Fork this repo
2. Create your feature branch (`git checkout -b feature/add-enhancement`)
3. Commit your changes (`git commit -am 'Add DRLBP feature'`)
4. Push to the branch (`git push origin feature/add-enhancement`)
5. Create a new Pull Request

---

## 📬 Contact

**Sachin Loddiya Karthik**
[GitHub](https://github.com/SachinLoddiyaKarthik)
[LinkedIn](https://www.linkedin.com/in/sachin-lk/)

---

**Project Repository**:
[https://github.com/SachinLoddiyaKarthik/Automated\_Attendance\_System\_Using\_Python](https://github.com/SachinLoddiyaKarthik/Automated_Attendance_System_Using_Python)

