# Sign Language Interpreter

A comprehensive Sign Language Interpreter application that converts text to sign language and provides real-time sign language recognition using TensorFlow and MediaPipe.

## 🚀 Features

- Text to Sign Language conversion
- Real-time sign language recognition
- Computer vision-based gesture detection
- User-friendly interface with GUI support
- Comprehensive dataset support

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

### System Requirements:
- **Python 3.8 to 3.11** (Recommended: Python 3.9 or 3.10)
  - ⚠️ **Important**: TensorFlow 2.12.1 requires Python 3.8-3.11
  - Python 3.12+ is not supported by this TensorFlow version
- **Operating System**: Windows (due to pywin32 dependency)
- **RAM**: Minimum 8GB recommended
- **Storage**: At least 2GB free space for dataset and dependencies

### Check Your Python Version:
```bash
python --version
```

If you don't have the correct Python version, download it from [python.org](https://www.python.org/downloads/)

## 🛠️ Installation & Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/KunalVishwakarma55/Kunal.git
cd Kunal
```

### Step 2: Create Python Virtual Environment

Create a virtual environment to isolate project dependencies:

```bash
# Create virtual environment
python -m venv sign_language_env

# Activate virtual environment (Windows)
sign_language_env\Scripts\activate

# You should see (sign_language_env) in your command prompt
```

### Step 3: Upgrade pip and Install Dependencies

```bash
# Upgrade pip to latest version
python -m pip install --upgrade pip

# Install all required packages
pip install -r requirements.txt
```

**Note**: Installation may take 10-15 minutes due to TensorFlow and other large packages.

### Step 4: Download Dataset

1. **Download** the dataset from Google Drive: [📁 Dataset Link](https://drive.google.com/drive/folders/1kuFzuLSNsfWzpcxqfJqUmTsajNVBcyik?usp=drive_link)

2. **Extract** the downloaded dataset files

3. **⚠️ IMPORTANT**: Place the extracted dataset folder as `Dataset` inside the `text-to-sign` directory

**Correct folder structure:**
```
Kunal/
├── text-to-sign/
│   ├── Dataset/          # <- Place downloaded dataset HERE (capital D)
│   │   ├── [dataset files and folders]
│   │   └── [sign language images/videos]
│   ├── combined.mp4
│   └── .gitignore
├── sign-to-text/
│   └── [sign recognition files]
├── ui/
│   └── [user interface files]
├── assets/
│   └── [project assets]
├── main.py              # Main application entry point
├── loading.py           # Loading screen module
├── requirements.txt     # Python dependencies
├── combined.avi         # Demo video
└── README.md           # This file
```

### Step 5: Run the Application

Make sure your virtual environment is activated, then:

```bash
python main.py
```

## 🔧 Troubleshooting

### Python Version Issues:
```bash
# Check your Python version
python --version

# If you have multiple Python versions, try:
python3.9 -m venv sign_language_env
# or
python3.10 -m venv sign_language_env
```

### Common Installation Errors:

1. **TensorFlow installation fails**:
   ```bash
   # Try installing TensorFlow separately first
   pip install tensorflow==2.12.1
   ```

2. **OpenCV issues**:
   ```bash
   # Reinstall OpenCV packages
   pip uninstall opencv-python opencv-contrib-python
   pip install opencv-contrib-python==4.10.0.84
   ```

3. **MediaPipe installation fails**:
   ```bash
   # Install MediaPipe separately
   pip install mediapipe==0.10.18
   ```

4. **Dataset not found error**: 
   - Verify the `Dataset` folder is in `text-to-sign/Dataset/` (note the capital D)
   - Check that all files were extracted properly
   - Ensure you have read permissions for the dataset folder

5. **Memory errors**:
   - Close other applications to free up RAM
   - Restart your computer if needed

### Virtual Environment Issues:
```bash
# Deactivate current environment
deactivate

# Remove and recreate environment
rmdir /s sign_language_env
python -m venv sign_language_env
sign_language_env\Scripts\activate
pip install -r requirements.txt
```

## 🖥️ System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| Python | 3.8 | 3.9 or 3.10 |
| RAM | 8GB | 16GB |
| Storage | 2GB free | 5GB free |
| OS | Windows 10 | Windows 10/11 |

## 📖 Usage

1. **Activate** your virtual environment:
   ```bash
   sign_language_env\Scripts\activate
   ```

2. **Run** the application:
   ```bash
   python main.py
   ```

3. **Features available**:
   - **Text-to-Sign**: Convert written text to sign language animations
   - **Sign-to-Text**: Real-time sign language recognition and conversion to text
   - **Interactive UI**: User-friendly interface for easy navigation

## 🎯 Project Modules

- **`main.py`**: Application entry point and main controller
- **`text-to-sign/`**: Text to sign language conversion module
- **`sign-to-text/`**: Sign language recognition and text conversion
- **`ui/`**: User interface components
- **`assets/`**: Project resources and media files
- **`loading.py`**: Loading screen and initialization

## 🛠️ Key Dependencies

- **TensorFlow 2.12.1**: Machine learning framework for model training and inference
- **MediaPipe 0.10.18**: Hand tracking and pose detection
- **OpenCV 4.10.0.84**: Computer vision processing and video handling
- **NumPy 1.24.3**: Numerical computations and array operations
- **PyQt5/PySide6**: GUI framework for user interface
- **CVZone 1.6.1**: Computer vision utilities

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Kunal Vishwakarma**
- GitHub: [@KunalVishwakarma55](https://github.com/KunalVishwakarma55)

## 🙏 Acknowledgments

- TensorFlow and MediaPipe teams for excellent ML frameworks
- OpenCV community for computer vision tools
- Sign language community for dataset contributions
- Contributors to the open-source libraries used in this project

---

## ⚠️ Important Notes

1. **Python Version**: Must use Python 3.8-3.11 (TensorFlow 2.12.1 requirement)
2. **Dataset**: Download and place in `text-to-sign/Dataset/` folder
3. **Virtual Environment**: Highly recommended to avoid dependency conflicts
4. **Windows**: Some dependencies (pywin32) are Windows-specific
5. **First Run**: Initial setup may take time for model loading

## 🚀 Quick Start

```bash
# Clone and setup
git clone https://github.com/KunalVishwakarma55/Kunal.git
cd Kunal

# Create environment and install dependencies
python -m venv sign_language_env
sign_language_env\Scripts\activate
pip install -r requirements.txt

# Download dataset and place in text-to-sign/Dataset/

# Run the application
python main.py
```

**Need Help?** Open an issue on GitHub with your error message and system details.
```

Now let's commit and push the updated README:

```bash
git add README.md
```

```bash
git commit -m "Update README with correct project structure and folder names"
```

```bash
git push origin main
