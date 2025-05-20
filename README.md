# Gesture Detection

A Python-based hand gesture detection project inspired by the *Naruto* anime series. Using PyTorch and computer vision, this project recognizes 12 distinct hand signs and maps them to keyboard keybinds, allowing users to control their computers with gesture-based input.

---

## 📖 Description

Gesture Detection leverages object detection and machine learning to recognize predefined hand signs, enabling gesture-based computer control. This project was inspired by the dynamic hand signs featured in Naruto and provides an alternative input method by binding gestures to keyboard actions.

- Recognizes **12 hard-coded hand signs**
- Maps gestures to specific **keyboard keybinds**
- Designed for use on **Windows systems**
- Built using **PyTorch**, **OpenCV**, and **Jupyter Notebook**

---

## 🎥 Demo / Screenshots

*Coming soon!*


---

## 📋 Installation

### 🧰 Requirements

- Windows OS
- Python 3.8+
- Jupyter Notebook
- Virtual Environment (recommended)

---

### 📦 Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/hqrris0n/gesture-detection
   cd gesture-detection
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv customNameHere
   .\customNameHere\Scripts\activate
   ```

3. **Run Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

4. **Execution Notes**
   - Open the notebook file in your browser.
   - Run **each cell in sequential order** to initialize the webcam, load the model, and start detection.
   - There is an optional **camera testing cell** near the bottom of the notebook for debugging.

6. **To exit the program**
   - Press `q` in the webcam window to stop detection.
   - Make sure the **next notebook cell is queued to run** to ensure the camera feed and processes close properly.

---

## ⚙️ Usage

- Start Jupyter Notebook and run each cell from top to bottom.
- When a valid hand gesture is detected by the webcam, the corresponding **keyboard input will be sent** to the OS.
- All gestures and their associated keybinds are **hard-coded** (chart to come in a future update).

---

## ✨ Features

- Real-time gesture recognition using webcam
- 12 unique hard-coded hand signs inspired by Naruto
- Gesture-to-keyboard mapping for alternative input
- Jupyter Notebook interface for step-by-step execution
- Optional camera testing/debugging cell
- Windows compatibility with virtual environment setup

---

## 🧪 Technologies Used

- **Python**
- **PyTorch**
- **OpenCV**
- **Jupyter Notebook**

---

## 🤝 Contributing

Contributions are welcome! If you’d like to help improve this project:

1. Fork the repository  
2. Create a new branch (`git checkout -b feature-name`)  
3. Commit your changes (`git commit -m 'Add new feature'`)  
4. Push to the branch (`git push origin feature-name`)  
5. Open a Pull Request

Ideas for future contributions:
- Custom gesture training support
- Editable keybind mapping
- Cross-platform compatibility (Linux, macOS)

---

## 📄 License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Harrison Nguyen**  
[GitHub Profile](https://github.com/hqrris0n)
