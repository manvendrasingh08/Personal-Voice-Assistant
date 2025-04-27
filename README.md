 Python Virtual Assistant

A voice-activated virtual assistant developed in Python that can perform various tasks such as opening applications, telling jokes, fetching weather, taking notes, playing music, capturing photos, downloading videos, and much more.

---

## Features

- 🎙️ Voice Commands using Speech Recognition
- 🖥️ Open and interact with system applications (CMD, Notepad, Zoom, Calendar, etc.)
- 🌐 Web Automation (Google, YouTube, Gmail, Webex)
- 📅 Date and Time Display
- 🌦️ Weather Reports (using OpenWeatherMap API)
- 📸 Take Pictures using Webcam
- 📝 Take Notes and Save as Word Documents
- 🗑️ Empty Recycle Bin
- 🔐 Lock the Device
- 📩 Open and send Emails
- 🎶 Play Music
- 📷 Take Screenshots
- 📚 Wikipedia Search
- 📰 Fetch Latest News
- 😂 Tell Jokes
- 🎥 Download YouTube Videos
- ⏺️ Voice Recording
- ⏳ Pause Assistant until "Space" Key is Pressed

---

## Setup Instructions

### Prerequisites

- Python 3.x installed
- Pip (Python package manager)

### Install Required Libraries

Run the following command:

```bash
pip install SpeechRecognition pyttsx3 wikipedia pyjokes pytesseract beautifulsoup4 pygame feedparser requests opencv-python winshell plyer pyqrcode youtube_dl keyboard python-docx newspaper3k
```

Also, you may need:

- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) installed and added to your system PATH (for OCR features)
- `ffmpeg` installed for YouTube downloads (for `youtube_dl`)

### File Structure Example

```
VoiceAssistant/
├── Calendar/               # Calendar executable
├── Calculator/              # Calculator executable
├── Recordingapp/            # Voice Recorder executable
├── Screenshot Taker/        # Screenshot taker executable
├── Senting Gmail/           # Gmail sender executable
├── My audio/                # Music files
├── images/                  # Folder to save captured images
├── Documents/               # Saved notes
├── Customization/
│   └── VoiceAssistant.ico           # Notification icon
├── VoiceAssistant.py                # Main script
└── README.md                # This file
```

Make sure paths inside the script (like `C:\Users\joels\Desktop\VoiceAssistant\Documents`) match your system.

---

## How to Run

Simply run:

```bash
python VoiceAssistant.py
```

Make sure your microphone is connected and functional, as the assistant heavily relies on voice commands.

---

## Important Notes

- This project is designed for Windows OS (uses Windows-specific libraries like `ctypes`, `winshell`, and `pyttsx3` with `sapi5`).
- Be sure all external executable programs (like Calendar, Recorder, Calculator) exist at the specified paths or adjust the script accordingly.
- Some modules like `youtube_dl` may require updated forks (like `yt-dlp`) because `youtube_dl` is outdated.