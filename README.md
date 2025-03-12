Image Colorization Web App

This web app allows you to upload black-and-white images, and it will automatically colorize them using a deep learning model based on the Caffe framework. The application uses Flask for the backend and OpenCV for image processing and model inference.
Features

    Upload a black-and-white image via the web interface.
    Automatically colorize the uploaded image using a pre-trained deep learning model.
    View the original and colorized images on the same page.

Requirements

    Python 3.x
    Flask
    OpenCV
    NumPy

You can install the necessary dependencies using the following command:

pip install flask opencv-python numpy

Setup

    Clone this repository or download the project to your local machine.

    Download the required model files:
        colorization_deploy_v2.prototxt
        pts_in_hull.npy
        colorization_release_v2.caffemodel

    These files are part of the colorization model and can be found from the source repository or relevant model provider. Ensure they are saved in the model folder inside your project directory.

    Directory Structure: Your project folder should look like this:

├── app.py
├── static/
│   └── uploads/
├── templates/
│   └── index.html
└── model/
    ├── colorization_deploy_v2.prototxt
    ├── pts_in_hull.npy
    └── colorization_release_v2.caffemodel

Run the app: Navigate to your project directory and run the following command to start the Flask web server:

    python app.py

    By default, the app will be accessible at http://127.0.0.1:5000/.

Usage

    Open the app in your web browser.
    Click on the "Choose File" button to select a black-and-white image from your computer.
    Once the image is uploaded, it will be colorized automatically, and both the original and colorized versions will be displayed.
