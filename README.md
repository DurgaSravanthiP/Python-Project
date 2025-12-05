# Automated Attendance System Using Face Recognition

A Python-based face recognition attendance system that detects and identifies faces in real-time and automatically stores attendance with timestamps using OpenCV. The system includes dataset creation, face encoding, training, live recognition, and CSV attendance tracking.

---

## 🚀 Features

- 📸 Capture face images and create a dataset
- 🔐 Generate face encodings using OpenCV
- 📹 Real-time face recognition through webcam
- 📝 Automatically record name, date, and time in CSV file
- 🐍 Simple and easy-to-run Python scripts
- 🧩 Modular code (dataset → encoding → recognition)

---

## 📂 Folder Structure

```
Automated-Attendence-System/
│
├── photos/                              # Dataset images (captured faces)
├── resources/                           # Haarcascade and other model files
│
├── EncodeFile.p                         # Encoded face data (pickle file)
├── Automated_Attendence-report.pdf
├── Automated_Attendence using face recognition.pdf
│
├── encodenerator.py                     # Generates encodings for all images
├── main1.py                             # Main face recognition + attendance script
├── upload.py                            # (Optional) Upload attendance file script
├── report_sender.py                     # (Optional) Email sender for reports
│
└── python.code-workspace                # VS Code workspace file
```

---

## 🛠️ Technologies Used

- **Python** - Programming language
- **OpenCV** - Computer vision library
- **NumPy** - Numerical computing
- **face_recognition** - Face detection and recognition (optional)
- **CSV** - Attendance storage format

---

## ▶️ How to Run the Project

### Step 1️⃣: Install Dependencies

```bash
pip install opencv-python numpy
```

If using face_recognition:

```bash
pip install face_recognition
```

### Step 2️⃣: Add Images for Training

1. Create a folder named `photos/`
2. Add face images for training
3. Each person should have multiple images with clear lighting

### Step 3️⃣: Generate Encodings

Run the encoding generator script:

```bash
python encodenerator.py
```

This creates the `EncodeFile.p` file with encoded face data.

### Step 4️⃣: Start Attendance System

Launch the main recognition script:

```bash
python main1.py
```

**This will:**

- ✅ Open webcam feed
- ✅ Detect and recognize faces
- ✅ Mark attendance in a CSV file

---

## 📄 Attendance Output Format

The system stores attendance in a CSV file with the following format:

```csv
Name, Date, Time
```

**Example:**

```csv
Sravanthi, 2025-12-05, 14:32:10
```

---

## 📈 Future Improvements

- ✨ Add liveness detection (to avoid photo spoofing)
- 🎨 Improve UI with a dashboard
- 💾 Add database storage instead of CSV
- 🌐 Build a Streamlit web interface
- 📧 Integrate notification or email system

---

## 👩‍💻 Author

**Durga Sravanthi Peddoju** 

---

## ⭐ Contributions

Pull requests are welcome! If you find bugs or want to improve the project, feel free to contribute.
