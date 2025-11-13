# Face Recognition Based Attendance Management System

## 📘 Abstract
This project presents a **Face Recognition–Based Attendance Monitoring System** designed for educational institutions. The system automates attendance marking by recognizing students’ faces through a webcam in real-time using **OpenCV**, **Python**, and **Machine Learning**.  

It eliminates manual entry errors, prevents proxy attendance, and automatically updates attendance data into an Excel sheet, which is then sent to the faculty via email using **SMTP**.

---

## 🚀 Features
- 🎥 **Real-Time Face Detection and Recognition**
- 🧠 **LBPH (Local Binary Pattern Histogram) Algorithm** for training and recognition
- 🧾 **Automated Attendance Logging** into Excel sheets
- 📧 **Automatic Email Notification** of attendance reports
- 🧍‍♂️ **Admin & Teacher Modules** for managing users
- 💾 **Database Creation & Training Module**
- 🖼 **Tkinter GUI Interface** for user interaction

---

## 🧩 Technologies Used
| Category | Tools / Libraries |
|-----------|------------------|
| Programming Language | Python 3.7 |
| Libraries | OpenCV, NumPy, Pandas, PIL (Pillow), Tkinter, smtplib |
| Algorithms | LBPH Face Recognizer, Haar Cascade Classifier |
| IDE / Tools | Anaconda (Jupyter Notebook), Visual Studio Code |
| OS Compatibility | Windows 7 / 8 / 10 (64-bit) |

---

## 🏗 System Architecture
1. **Image Capture** → Webcam captures real-time video feed.  
2. **Face Detection** → Haar Cascade Classifier detects face regions.  
3. **Face Recognition** → LBPH algorithm identifies the student from the trained dataset.  
4. **Attendance Marking** → Recognized faces are recorded in an Excel file.  
5. **Report Mailing** → Attendance sheet is automatically sent via email using SMTP.  

---

## 📂 Project Structure
```
Face-Recognition-Attendance/
│
├── TrainingImage/               # Stores student face images
├── TrainingImageLabel/          # Trained model (Trainner.yml)
├── StudentDetails/              # Student details CSV file
├── Attendance/                  # Saved attendance CSV reports
├── haarcascade_frontalface_default.xml
├── main.py                      # Main Tkinter GUI script
├── train.py                     # Model training script
├── test.py                      # Testing / Recognition script
└── README.md
```

---

## ⚙️ Installation & Setup
1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/face-recognition-attendance.git
   cd face-recognition-attendance
   ```

2. **Install required dependencies**
   ```bash
   pip install opencv-python numpy pandas pillow
   ```

3. **Run the application**
   ```bash
   python main.py
   ```

4. **Train model**
   - Add student images in `TrainingImage/`
   - Run training script:
     ```bash
     python train.py
     ```

5. **Start attendance recognition**
   ```bash
   python test.py
   ```

---

## 👩‍💻 Usage Guide
1. **Register Student**
   - Enter ID and Name → Capture images using webcam → Save to dataset.  
2. **Train Model**
   - Train images using LBPH Face Recognizer.  
3. **Mark Attendance**
   - Start recognition → System automatically marks present students.  
4. **Email Report**
   - Attendance sheet will be sent automatically to the faculty’s email.  

---

## 📊 System Modules
- **Database Creation** – Stores and manages student images and IDs.  
- **Video Recording** – Captures frames from live webcam feed.  
- **Face Detection** – Detects human faces using Haar Cascade Classifier.  
- **Face Recognition** – Identifies faces with trained LBPH model.  
- **Attendance Registration** – Marks attendance in `.csv` format.  
- **Mail Automation** – Sends attendance data via email using SMTP.

---

## 🧠 Algorithms Used
- **Haar Cascade Classifier** – Detects faces from real-time frames.
- **Local Binary Pattern Histogram (LBPH)** – Extracts facial features and compares them for recognition.

---

## 🧪 Testing
- **Unit Testing** – Individual module testing for recognition and data saving.
- **Integration Testing** – Ensures modules interact correctly (Camera + Recognition + Excel).
- **System Testing** – Verifies full functionality and UI flow.
- **Acceptance Testing** – Validated by real users (faculty and students).

---

## 🏁 Conclusion
This automated attendance system minimizes human intervention, saves time, and improves accuracy.  
Future improvements may include:
- Integration with web-based dashboards.
- Real-time cloud data storage.
- Improved accuracy under low-light conditions.

---

## 📚 References
- OpenCV Documentation – [https://opencv.org](https://opencv.org)  
- NumPy – [https://numpy.org](https://numpy.org)  
- IEEE Research Papers on Face Recognition Attendance Systems  

---

## 👨‍💻 Authors
**Developed by:**  
Nandha Kumar N — MCA (Cognifyz Technologies Internship Project)  
**Duration:** May 1, 2025 – September 1, 2025  
**Institution:** [Your College Name]  
**Contact:** [your-email@example.com]

---

## 🏷 License
This project is released under the **MIT License**.  
You’re free to modify and distribute it with attribution.
