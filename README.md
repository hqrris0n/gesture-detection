# Gesture Detection

A Python-based hand gesture detection project inspired by the *Naruto* anime series. Using PyTorch and computer vision, this project recognizes 12 distinct hand signs and maps them to keyboard keybinds, allowing users to control their computers with gesture-based input.

---

## 📖 Description

Gesture Detection leverages object detection and machine learning to recognize predefined hand signs, enabling gesture-based computer control. This project was inspired by the dynamic hand signs featured in Naruto and provides an alternative input method by binding gestures to keyboard actions.

- Recognizes **12 hard-coded hand signs**
- Maps gestures to specific **keyboard keybinds**
- Runs on **Windows** and **macOS** (separate notebook for each)
- Built using **PyTorch**, **OpenCV**, and **Jupyter Notebook**

---

## 📋 Installation

### 🧰 Requirements

- Windows or macOS
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

5. **To exit the program**
   - Press `q` in the webcam window to stop detection.
   - Make sure the **next notebook cell is queued to run** to ensure the camera feed and processes close properly.

---

### 🍎 macOS Setup

Use `Gesture_Control_macOS.ipynb` instead of `Gesture_Control.ipynb`. It is the same notebook, but sends keypresses with `pynput` instead of the Windows-only `win32api`.

1. **Install dependencies and open the notebook** (using [uv](https://docs.astral.sh/uv/))
   ```bash
   cd gesture-detection
   uv run --with ultralytics --with pynput --with notebook jupyter notebook Gesture_Control_macOS.ipynb
   ```

2. **Grant permissions** in *System Settings → Privacy & Security*
   - **Camera**: for the webcam feed
   - **Accessibility**: so keypresses reach other apps (they silently do nothing without it)
   - Grant both to the app the notebook runs from. When using VS Code's integrated terminal or Jupyter extension, that is **Visual Studio Code**, not Terminal. Add it with the **+** button if it is not listed.

3. **Execution Notes**
   - If the wrong camera opens (e.g. an iPhone via Continuity Camera), use the camera testing cell and change `cv2.VideoCapture(0)` to the right index.
   - Keypresses go to whichever window is focused, so click into the target app after starting detection.

---

## ⚙️ Usage

- Start Jupyter Notebook and run each cell from top to bottom.
- When a valid hand gesture is detected by the webcam, the corresponding **keyboard input will be sent** to the OS.
- All gestures and their associated keybinds are **hard-coded**:

| Class ID | Hand Sign | Key |
|:-:|---|:-:|
| 0 | Bird | `O` |
| 1 | Boar | `E` |
| 2 | Dog | `D` |
| 3 | Dragon | `L` |
| 4 | Hare | `A` |
| 5 | Horse | `J` |
| 6 | Monkey | `I` |
| 7 | Ox | `Q` |
| 8 | Ram | `K` |
| 9 | Rat | `S` |
| 10 | Snake | `P` |
| 11 | Tiger | `W` |

### ✋ Hand Signs

Reference chart for the 12 signs (source: [Naruto Wiki – Hand Seal](https://naruto.fandom.com/wiki/Hand_Seal)):

[![The 12 basic hand seals](https://static.wikia.nocookie.net/naruto/images/a/a7/Hand.png/revision/latest?cb=20130912073828)](https://naruto.fandom.com/wiki/Hand_Seal)

---

## ✨ Features

- Real-time gesture recognition using webcam
- 12 unique hard-coded hand signs inspired by Naruto
- Gesture-to-keyboard mapping for alternative input
- Jupyter Notebook interface for step-by-step execution
- Optional camera testing/debugging cell
- Windows and macOS support

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
- Linux compatibility

---

## 📄 License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Harrison Nguyen**  
[GitHub Profile](https://github.com/hqrris0n)
