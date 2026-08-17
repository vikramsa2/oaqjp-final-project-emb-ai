# Repository for final project
# Emotion Detection

This project is a Flask-based web application that utilizes IBM Watson's NLP Emotion Detection API to analyze text input and output emotional analysis scores (anger, disgust, fear, joy, and sadness) along with the dominant emotion.

---

## 🛠️ Project Architecture

```text
final_project/
│
├── EmotionDetection/           # Custom Python package
│   ├── __init__.py             # Package initialization
│   └── emotion_detection.py    # Core function integrating Watson NLP API
│
├── static/
│   └── mywebscript.js          # JavaScript front-end interaction logic
├── templates/
│   └── index.html              # Web page interface
│
├── test_emotion_detection.py   # Unit testing suite
├── server.py                   # Flask server entry point
└── README.md                   # Project documentation
```

---

## 🚀 Features

* **Real-time Text Analysis:** Accepts user text input via the web interface and processes emotional sentiment using Watson NLP APIs.
* **Dominant Emotion Identification:** Aggregates scores across five emotional spectrums (anger, disgust, fear, joy, sadness) and dynamically returns the primary emotion.
* **Error & Edge Case Handling:** Gracefully handles empty inputs or HTTP 400 responses from the API, notifying the user of invalid input.
* **Unit Tested:** Built with automated Python unit tests covering typical emotional classifications.
* **PyLint Compliant:** Server code formatted to maintain a 10/10 code quality score.

---

## 📦 Requirements

* Python 3.8+
* `flask`
* `requests`
* `pylint` (for code quality inspection)

---

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd final_project
   ```

2. **Install required packages:**
   ```bash
   python3 -m pip install requests flask pylint
   ```

---

## 🧪 Testing & Code Quality

### Run Unit Tests
To verify the core logic of the `emotion_detector` package:
```bash
python3 test_emotion_detection.py
```

### Run PyLint Static Analysis
To check code compliance and formatting score:
```bash
pylint server.py
```

---

## 🖥️ Running the Application

1. **Start the Flask server:**
   ```bash
   python3 server.py
   ```

2. **Open in browser:**
   Navigate to `http://localhost:5000` or `http://127.0.0.1:5000` in your browser.

3. **Usage:**
   * Enter a sentence into the text input field (e.g., *"I am glad this happened"*).
   * Click **Run Analysis** to view the breakdown of emotional scores and the dominant emotion.
