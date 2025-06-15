# Face-Recognition-System
A Python-based Face Recognition system using OpenCV and face detection libraries. This project allows you to detect and recognize human faces in real time or from images.
## 🧾 Description

This project uses OpenCV with Haar Cascades and/or `face_recognition` library (built on top of dlib) to recognize faces. It's useful for building attendance systems, basic biometric verification, or even fun AI camera filters.

## 🚀 Features

- Detect and recognize human faces
- Real-time recognition via webcam
- Add new faces to the database
- Logs or alerts recognized individuals
- Easy to customize for projects like attendance or security

## 🗂️ Project Structure

faceRecognition/
├── dataset/ # Folder to store training face images
├── recognizer/ # Folder to save trained models
├── trainer.yml # Trained model
├── haarcascade_frontalface_default.xml
├── train.py # Script to train the recognizer
├── recognize.py # Script to recognize faces via webcam
├── collect.py # Script to collect face data
└── README.md

## 📦 Requirements

Make sure you have Python 3 and the following libraries installed:

pip install opencv-python opencv-contrib-python numpy

If using face_recognition:
pip install face_recognition

▶️ How to Use

1. Collect Face Data
python collect.py

Follow the prompts to save images of faces into the dataset folder.

3. Train the Model
python train.py

This generates a model (trainer.yml) using the face samples.

5. Run Face Recognition
python recognize.py

Opens webcam and displays recognized faces with their names (or IDs).

📸 Example Output

Detected face: dhivakar
Or with bounding boxes and names over the webcam feed.

🛠️ Customize

You can adapt this code for:
Attendance systems
Smart door locks
Personalized experiences in apps

📄 License

This project is open source under the MIT License.

🙋‍♂️ Contributing
Feel free to fork this repository, open issues, or submit pull requests!

yaml
Copy
Edit

---

### ✅ How to Upload to GitHub:

1. **Extract** your `faceRecognition.zip`.
2. **Copy** the `README.md` into that folder.
3. Open terminal:

bash
cd faceRecognition
git init
git add .
git commit -m "Initial commit: Face Recognition System"
git remote add origin https://github.com/YOUR_USERNAME/faceRecognition.git
git branch -M main
git push -u origin main
