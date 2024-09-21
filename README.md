# Emotion-Recognition
Final work in educational course 'Data Science. Middle. Neural Networks'

To run the main code from the main tab, you need to create a new personal API token on kaggle, download the kaggle.json file and select it in the pop-up window, after running the code and clicking on the button in the corresponding 'select files' cell. This is required to download the training dataset from kaggle.

The file emotion_web.ipynb is the third part of the thesis, integrating the trained model with the laptop webcam, it needs to be run locally using jupyter notebook. Before starting, you need to make sure that you have access to the webcam. The script in the file is an implementation of the client logic of a client-server connection in which data is exchanged using the http:/ protocol. Emotion predictions are made using requests to the server implemented using TensorFlow Serving.

Some of the outputs are in russian.
Sorry about that. Due to the fact that it's time-consuming to rerun the whole notebook it has been kept in russian.


