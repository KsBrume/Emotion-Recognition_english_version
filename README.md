# Emotion-Recognition
Final work in educational course 'Data Science. Middle. Neural Networks'

To run the main code from the main tab, you need to create a new personal API token on kaggle, download the kaggle.json file and select it in the pop-up window, after running the code and clicking on the button in the corresponding 'select files' cell. This is required to download the training dataset from kaggle.

The file emotion_web.ipynb is the third part of the thesis, integrating the trained model with the laptop webcam, it needs to be run locally using jupyter notebook. Before starting, you need to make sure that you have access to the webcam. The script in the file is an implementation of the client logic of a client-server connection in which data is exchanged using the http:/ protocol. Emotion predictions are made using requests to the server implemented using TensorFlow Serving.

Note: Some of the outputs are in russian.
Sorry about that. Due to the fact that it's time-consuming to rerun the whole notebook it has been kept in russian.

In this paper I will teach neural network recognize 9 categories of emotions including 6 basic emotions, contempt, neutral facial expression and uncertain one.

There are 3 parts in this paper:

1. Experiments on training CNN on training data, which are more than 50,000 photos of people in static, one face in the photo, with the corresponding label denoting emotion, to obtain the required metric value categorical accuracy > 0.4.

2. A valence-arousal approach for training a model, where the model is trained on the emotion decomposition components valence (how positive or negative the emotion is) and arousal (intensity).

3. Integration of an emotion recognition model and a webcam for real-time emotion classification. This part of the work goes in a separate emotion_web.ipynb file that needs to be run on the local machine.


Obtained results:

Definition accuracy:

1. surprise - 76.96% (4866 out of 6323 images identified correctly)
2. happy - 66.47% (3958 out of 5955 images identified correctly)
3. fear - 47.34% (2388 out of 5044 images identified correctly)
4. neutral - 46.87% (3185 out of 6795 images identified correctly)
5. disgust - 43.87% (1384 out of 3155 images identified correctly)
6. sad - 42.18% (2843 out of 6740 images identified correctly)
7. anger - 40.62%(2852 out of 7022 images identified correctly)
8. contempt - 38.96% (1202 out of 3085 images identified correctly)
9. uncertain - 35.45% (2101 out of 5927 images identified correctly)

Conclusion: the model performed best on the defining of surprise (surprise) and happiness (happy). Worst of all, the model managed to reveal contempt (contempt) and an indefinite emotion (uncertain).

