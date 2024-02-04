pip install -r requirements.txt
pip install pandastable
pip install Werkzeug==0.16.0
python app.py


(Forgive the image quality and my expressions 😆)


# Tech Stack:
- Keras
- Tensorflow
- Spotipy
- Tkinter (For testing)
- Flask

# Dataset:
The dataset used for this project is the famous FER2013 dataset. Models trained on this dataset can classify 7 emotions. The dataset can be found <a href = "https://www.kaggle.com/msambare/fer2013">here</a>.

Note that the dataset is highly imbalanced with happy class having maxiumum representation. This might be a factor resulting in okaysish accuracy after training.


# Image Processing and Training:
- The images were normalised, resized to (48,48) and converted to grayscale in batches of 64 with help of 'ImageDataGenerator' in Keras API.
- Training took around 13 hours locally for 75 epochs with an accuracy of ~66 %

# Current condition:
The entire project works perfectly fine. Live detection gives good frame rates due to multithreading.



