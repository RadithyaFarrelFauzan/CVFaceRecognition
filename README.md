# CVFaceRecognition
# Requirements
Install these Python libraries first:
pip install opencv-python numpy scikit-learn matplotlib

How to Run
1. Prepare the Dataset
Create a folder named images/.
Inside images/, create one folder for each person (use their name as folder name).
Add at least 10 images per person.
Include your own face images too (varied lighting and expressions).

2. Train the Model
Run the main script to train the model:
python face_recognition.py

It will automatically:
- Load images
- Train using Eigenfaces
- Save the trained model into eigenface_pipeline.pkl
- Print classification report on the console

3. Run Real-Time Face Recognition
- After training, the script will open the webcam automatically.

It will:
- Detect faces
- Recognize them
- Display bounding boxes with names and scores
- Press 'q' to quit the webcam window.

Tips
- Make sure the lighting is good when testing with the webcam.
- If the webcam is not available, you can modify the script to process a recorded video.
- To improve accuracy, collect more diverse images for each person.
