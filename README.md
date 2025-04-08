
# 🧠 Face Recognition Attendance System using Python & OpenCV

![Made with Python](https://forthebadge.com/images/badges/made-with-python.svg)
![Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg)

This project is a real-time **Face Recognition-based Attendance System** built using **Python 3.9** and **OpenCV**. It detects and recognizes faces from a webcam feed and automatically marks attendance in a CSV file. This can be used in schools, colleges, or offices.

---

## 🚀 Getting Started

### 🔧 Prerequisites

- Python 3.9+
- OpenCV
- NumPy
- Pandas
- PIL (Pillow)

### 📥 Installation Steps

1. **Clone this repository**:

   ```bash
   git clone https://github.com/yourusername/face-attendance-system.git
   cd face-attendance-system
   ```

2. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Create a folder** named `TrainingImage` in the project directory.

4. **Open the files** `attendance.py` and `automaticAttendance.py` and **update all file paths** according to your local system.

5. **Run the main script**:

   ```bash
   python attendance.py
   ```

---

## 🔄 Project Workflow

### 1. Register a New Student

- Click **Register New Student**.
- Enter **Student ID** and **Name**.
- Click **Take Image**.
- The webcam captures ~50 images and saves them in the `TrainingImage/` folder.
- (You can increase/decrease the number of images as needed.)

### 2. Train the Model

- Click **Train Image**.
- It converts all stored face images into numerical encodings and trains a recognition model.
- Trained data is stored in `TrainingImageLabel/`.

### 3. Mark Attendance

- Click **Automatic Attendance**.
- Enter the subject name.
- The system will detect and recognize faces and mark attendance in a `.csv` file.
- A new file is created per subject with date and time entries.

### 4. View Attendance

- Click **View Attendance**.
- It shows all attendance records in a tabular format inside the GUI.

---

## 🗂️ Folder Structure

```
📁 face-attendance-system/
│
├── TrainingImage/           # Stores face images of registered users
├── TrainingImageLabel/      # Stores trained model file
├── Attendance/              # CSV logs of attendance
├── screenshots/             # UI and functional screenshots
├── attendance.py            # Main app to register/train/take attendance
├── automaticAttendance.py   # Script for attendance recognition
├── requirements.txt         # All required Python packages
└── README.md                # This file
```

---

## 📸 Screenshots

### 🧾 Main UI  
![UI](screenshots/home.png)

### 📷 While Taking Image  
![Capture](screenshots/capture.png)

### 📌 Attendance Window  
![Attendance](screenshots/attendance.png)

### 📊 Attendance Table  
![Table](screenshots/tabular.png)

---

## ⭐ Support

If you like this project, don’t forget to **Star ⭐ the repo** and **Follow** for more cool projects. Contributions and feedback are welcome!

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
