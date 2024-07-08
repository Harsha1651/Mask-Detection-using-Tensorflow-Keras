# Mask-detection-using-Tensorflow-Keras
This project aims to detect whether individuals in a video stream are wearing masks using a deep learning model. The program utilizes OpenCV for face detection and TensorFlow/Keras for mask classification.<br>
<b>Components:</b>
<b>Face Detection:</b> The program uses a Haar Cascade classifier to detect faces in real-time from a video feed.<br>
<b>Mask Classification:</b>. A pre-trained convolutional neural network (CNN) model, loaded from saved_model.h5, classifies detected faces as either "Mask" or "No Mask".
<br><b>Visualization:</b> The program draws rectangles around detected faces and labels them with the classification result ("Mask" or "No Mask") in the video stream.
<br><b>Key Steps</b>
<br><b>Load Pre-trained Model:</b> The model is loaded using tensorflow.keras.models.load_model.
<br><b>Initialize Video Capture:</b> The video feed is captured using cv2.VideoCapture. The source can be either a video file or a system camera.
<br><b>Face Detection:</b> Frames from the video feed are processed to detect faces using Haar Cascade classifier (haarcascade_frontalface_default.xml).
<br><b>Preprocess Detected Faces:</b> Detected faces are extracted, resized to the required input dimensions for the model, and converted to arrays.
<br><b>Mask Classification:</b> Each detected face is classified as "Mask" or "No Mask" using the loaded model.
<br><b>Display Results:</b> The results are displayed on the video feed with rectangles drawn around faces and labels indicating mask status.
