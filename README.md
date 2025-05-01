## 🧠 AI-Powered Exercise Counter 🏋️‍♀️

### 📌 Overview
This project implements an **AI-powered exercise counter** that uses computer vision to automatically detect and count exercise repetitions in real time. It leverages **pose estimation** with **MediaPipe** and integrates logic to monitor body posture, enabling hands-free workout tracking and performance feedback.

Whether it's squats, push-ups, bicep curls, or more, this application offers a smart, camera-based solution to help fitness enthusiasts maintain proper form and track progress—no wearable required.

---

### 🎯 Features

- 🔍 **Real-time pose detection** using MediaPipe
- 📈 **Automated rep counting** based on joint angles
- 🖥️ **Live webcam feed** with feedback overlay
- 🔁 Supports multiple exercises like:
  - Bicep Curls
  - Squats
  - Push-ups *(extendable)*
- 💡 **Angle threshold logic** to accurately detect movement range
- 🧪 Easily testable with different video inputs or live webcam

---

### 🛠️ Tech Stack

| Tech         | Description                         |
|--------------|-------------------------------------|
| Python       | Core programming language           |
| OpenCV       | For image processing & webcam feed  |
| MediaPipe    | Pose estimation and landmark detection |
| NumPy        | For angle and mathematical ops      |
| Jupyter Notebook | Code and experimentation environment |

---

### 🚀 How It Works

1. **Pose Detection**: MediaPipe tracks 33 landmarks on the body using webcam/video input.
2. **Angle Calculation**: Angles between joints (like elbow or knee) are calculated using coordinates.
3. **Repetition Logic**: If angle transitions from 'down' to 'up' past a threshold → counts as a rep.
4. **Live Feedback**: Current angle, rep count, and exercise state displayed on screen.

---

### 🧰 Setup Instructions

#### 📦 Requirements

Install dependencies using pip:

```bash
pip install opencv-python mediapipe numpy
```

#### ▶️ Run the Project

1. Clone the repository:
```bash
git clone https://github.com/your-username/ai-exercise-counter.git
cd ai-exercise-counter
```

2. Launch Jupyter Notebook:
```bash
jupyter notebook Main.ipynb
```

3. Enable webcam and run all cells.

---

### 📁 Project Structure

```
.
├── Main.ipynb          # Jupyter Notebook with full implementation
├── README.md           # This file

```

---

### 📌 Future Improvements

- Add support for more exercise types (e.g. lunges, jumping jacks)
- Implement voice feedback system
- Build standalone app (using Streamlit or Tkinter)
- Add pose correction feedback with audio prompts

---

### 🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

---

### 📜 License

This project is licensed under the [MIT License](LICENSE).

---

### 🙌 Acknowledgements

- [MediaPipe](https://google.github.io/mediapipe/) for their powerful pose estimation tools
- OpenCV community for vision processing tools
