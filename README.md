# DeepFake Detection and Mitigation 🎭🧠

This project provides a robust deep learning-based solution for detecting and mitigating deepfake videos using computer vision and neural networks. It extracts key visual features from videos using OpenCV and classifies them as real or fake using a trained model built with TensorFlow/Keras.

---

## 📌 Table of Contents

- [About the Project](#about-the-project)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Usage](#usage)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## 📖 About the Project

With the increasing misuse of deepfake technology, this project aims to develop an AI-powered tool to:

- Detect forged video content.
- Mitigate its spread by flagging suspicious content.

This project was created as a final-year research initiative titled **"An Overview on DeepFake Video Detection and Mitigation."**

---

## ⚙️ Tech Stack

- **Programming Language:** Python 3.x
- **Libraries & Tools:**
  - OpenCV
  - TensorFlow / Keras
  - NumPy
  - Matplotlib (for visualization)
  - scikit-learn (for metrics and evaluation)
- **Environment:** Virtualenv (`venv`)
- **IDE:** VS Code / Jupyter Notebook (recommended)

---

## 📁 Project Structure

```bash
DeepFake-Detection-And-Mitigation/
├── deploy/
│ ├── main.py # Main pipeline script
│ ├── models/
│ ├── static/
│ │ ├──uploads/
│ │ └──upload.css
│ ├── templates/
│ │ └──upload.html
│ └── app.py
│
├── venv/ # Python virtual environment (ignored in Git)
├── requirements.txt # Python package dependencies
├── .gitignore # Git ignore rules
└── README.md # Project documentation
```

---

## ⚡ Getting Started

### ✅ Prerequisites

- Python 3.7 or higher
- `pip` installed
- A GPU (optional but recommended for training speed)

### 🛠️ Installation

1. **Clone the Repository**

```bash
git clone https://github.com/Akash-Kumar-2/DeepFake-Detection-And-Mitigation.git
cd DeepFake-Detection-And-Mitigation

    Set up a Virtual Environment

python -m venv venv
# Activate the environment
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

    Install Required Packages

pip install -r requirements.txt
```

### ▶️ Usage

- Prepare your dataset

  - Place real and fake video samples into respective folders (modify paths inside the code accordingly).

- Run the main script

- python deploy/main.py

  - View Output

    - Results are rendered on a web interface, served via Flask on http://localhost:5000, using upload.html.

    - Optionally, Prediction outcomes and relevant metadata are displayed directly in the browser. You can customize this interface to include graphs or confidence scores using Matplotlib or frontend charts.

### 🗃️ Dataset

- You can use open-source datasets such as:

  - FaceForensics++

  - DFDC (DeepFake Detection Challenge Dataset)

Make sure to preprocess the videos using extract_features.py before feeding into the model.

#### 🧠 Model Architecture

- The model is a CNN-based architecture trained on extracted frames. It includes:

  - Convolutional layers

  - Batch normalization

  - Dropout for regularization

  - Dense layers with sigmoid activation for binary classification

You can modify or improve the model in deploy/model.py.

<!--
# 📊 Results

#     Training Accuracy: ~92%

#     Validation Accuracy: ~88%

#     Binary Cross-Entropy Loss used as the loss function

#     Evaluation metrics: Precision, Recall, F1-Score
-->

**Note:** Actual results may vary based on dataset and preprocessing.

###### 🤝 Contributing

- Contributions, issues, and feature requests are welcome!

### To contribute:

    - Fork the repo

    - Create a new branch (git checkout -b feature/your-feature)

    - Commit your changes

    - Push to the branch

    - Open a pull request

<!--
### 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.
-->

### 🙏 Acknowledgements

- TensorFlow

- Keras

- OpenCV

- Research papers and community discussions around Deepfake detection

## 👨‍💻 Author

Akash Kumar

### 📸 Glimpse of The Project

![Image](https://github.com/user-attachments/assets/d5095772-d56a-4add-9243-b114d0cb0d41)
![Image](https://github.com/user-attachments/assets/cfe9c940-d3b0-4be7-a417-39fafe42f150)
![Image](https://github.com/user-attachments/assets/77d777b3-eb4d-415d-850c-b6c724574afb)
![Image](https://github.com/user-attachments/assets/8701522b-cc6c-4c0a-aaac-835603f8e1f3)
![Image](https://github.com/user-attachments/assets/5d08958b-7d7f-44c6-873f-642feface8dc)
