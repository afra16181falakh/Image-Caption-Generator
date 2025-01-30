This project uses deep learning to generate captions for images. It employs MobileNetV2 for feature extraction (optimized for memory efficiency) and an LSTM-based model with an attention mechanism for generating captions. The app is interactive and built with Streamlit for easy usability.

Features:

	•	Lightweight and efficient using MobileNetV2.
	•	Attention mechanism for improved caption relevance.
	•	Interactive app to generate captions on the go.
 

Dataset

The Flickr8k dataset is used for training and evaluation. It consists of:
	•	8,091 images with five captions per image.
	•	A diverse range of real-world scenes for robust training.

Setup

Requirements:

	•	Python 3.10+
	•	TensorFlow, Pandas, NumPy, and other dependencies in requirements.txt.

Installation:

	1.	Clone the repo:

git clone https://github.com/afra16181falakh/image-caption-generator.git
cd image-caption-generator


	2.	Install dependencies:

pip install -r requirements.txt

Streamlit Deployment

To deploy the app:
	1.	Fork the repo and connect it to your Streamlit Sharing account.
	2.	Set up the following configuration in Streamlit Sharing:

[server]
headless = true
port = $PORT
enableCORS = false


	3.	Deploy your app!
 
Key Components

	•	Model Training:
Built on MobileNetV2 for feature extraction, combined with LSTM and an attention mechanism for caption generation.

	•	Interactive App:
A Streamlit app allows users to upload images and generate captions instantly.

	•	Preprocessing:
Tokenization of captions and efficient data handling for training with the Flickr8k dataset.

	•	Trained Weights:
Pretrained weights (mymodel.h5) and tokenizer (tokenizer.pkl) included for quick setup.
