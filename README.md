# License-plate-recognition-
This project implements a License Plate Recognition (LPR) system using OpenCV and Tesseract OCR.   It detects vehicle number plates from images and extracts the text using Optical Character Recognition.

---

## 📌 Features

- Detects license plates from images
- Extracts alphanumeric text using OCR
- Cleans unwanted characters from OCR output
- Displays detected plate with bounding box
- Processes multiple images automatically

---

## 🛠️ Technologies Used

- Python
- OpenCV
- Tesseract OCR
- NumPy
- Regular Expressions

---

## 📁 Project Structure

License-Plate-Recognition/
│
├── detection.py
├── main.py
├── requirements.txt
├── README.md
└── images/

---

## ⚙️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/License-Plate-Recognition.git
cd License-Plate-Recognition

2️⃣ Install Python Dependencies
pip install -r requirements.txt

3️⃣ Install Tesseract OCR

Windows:
Download from:
https://github.com/tesseract-ocr/tesseract

Make sure to add Tesseract to system PATH.

Linux:

sudo apt install tesseract-ocr


Mac:

brew install tesseract

▶️ How to Run
python main.py


The system will:

Load each image

Detect license plate

Extract text using OCR

Display result with bounding box

Print detected plate number in terminal

Press any key to close each image window.

🧠 How the Code Works
Step 1: Load Haar Cascade

OpenCV's pre-trained Haar Cascade model is used to detect license plates.

Step 2: Convert Image to Grayscale

Improves detection accuracy.

Step 3: Detect License Plate Region

detectMultiScale() locates possible plate areas.

Step 4: Preprocess for OCR

Convert to grayscale

Apply thresholding

Clean output using regex

Step 5: Extract Text

Tesseract OCR extracts alphanumeric characters.

📸 Sample Output

Terminal Output:

Processing: images/Ford_Licenseplate.jpg
Detected Number from images/Ford_Licenseplate.jpg: MH12AB1234

Processing: images/Hyundai_License.jpg
Detected Number from images/Hyundai_License.jpg: KA05CD5678


Output Image:

Green bounding box around plate

Plate number displayed above the box

🚀 Future Improvements

Real-time webcam detection

YOLO-based deep learning detection

Store detected plates in CSV

Web application deployment

Database integration

👨‍💻 Author

Your Name
Advanced Internship Project – Slash Mark

