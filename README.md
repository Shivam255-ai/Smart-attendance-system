# Smart Attendance System - B.Tech Project

## Project Overview
An automated attendance system using face recognition technology to mark student attendance in real-time, preventing proxy attendance and providing comprehensive attendance management.

## Tech Stack
- **Backend**: Flask (Python)
- **Computer Vision**: OpenCV + face_recognition (dlib)
- **Database**: SQLite
- **Frontend**: HTML/CSS/JavaScript
- **Libraries**: NumPy, Pandas, Pillow

## Features
- ✅ Face registration for new students
- ✅ Real-time face recognition via webcam
- ✅ Automatic attendance marking with timestamp
- ✅ Proxy attendance prevention
- ✅ Export attendance as CSV/Excel
- ✅ Admin dashboard for teachers
- ✅ Unknown face detection alerts

## Project Structure
```
smart_attendance_system/
├── app.py                 # Main Flask application
├── config.py             # Configuration settings
├── requirements.txt      # Dependencies
├── database/
│   ├── __init__.py
│   ├── models.py        # Database models
│   └── attendance.db    # SQLite database
├── face_recognition/
│   ├── __init__.py
│   ├── face_encoder.py  # Face encoding utilities
│   └── face_detector.py # Real-time detection
├── static/
│   ├── css/
│   ├── js/
│   └── uploads/         # Student photos
├── templates/           # HTML templates
├── utils/
│   ├── __init__.py
│   └── helpers.py      # Utility functions
└── student_images/     # Training images
```

## Installation & Setup

### Quick Setup
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the application: `python app.py`
4. Access at: `http://localhost:5000`

### Face Recognition Setup (Enhanced Features)
For full face recognition capabilities:

1. **Install CMake** (required for dlib):
   - Windows: Download from https://cmake.org/download/
   - macOS: `brew install cmake`
   - Linux: `sudo apt-get install cmake`

2. **Run setup script**:
   ```bash
   python setup_face_recognition.py
   ```

3. **Test the system**:
   ```bash
   python test_face_recognition.py
   ```

4. **Start the application**:
   ```bash
   python app.py
   ```

### System Requirements
- Python 3.7+
- CMake (for dlib compilation)
- Webcam/Camera device
- 4GB+ RAM recommended

## Usage

### Face Recognition Mode (Automatic)
1. **Register Students**: Upload clear photos via admin panel
2. **Start Camera**: Click "Start Camera" on attendance page
3. **Enable Face Recognition**: Click "Start Face Recognition"
4. **Automatic Detection**: System detects and identifies students
5. **Mark Attendance**: Click "Mark Present" for detected students or use "Auto Mark"

### Manual Mode (Backup)
1. **Manual Entry**: Enter student ID directly
2. **Quick Marking**: Mark attendance without camera
3. **Backup Option**: Use when face recognition is unavailable

### Admin Features
- **Student Management**: Add/edit student profiles
- **Attendance Reports**: View and export attendance data
- **System Settings**: Configure detection parameters
- **Export Data**: Generate CSV/Excel reports

## Author
[Shivam Kumar] - B.Tech 3rd Year Project
