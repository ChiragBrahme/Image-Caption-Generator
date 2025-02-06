Image Caption Generator

Mission Statement

Goal: Develop an image caption generator for visually impaired individuals.
Objective: Generate descriptive captions for images to improve accessibility and inclusivity.
Importance: Provides a means for visually impaired users to understand visual content.

Summary of Problem
Problem: Visually impaired individuals face challenges in understanding and interacting with visual content (images, photographs, illustrations).
Solution: Develop an AI-driven image caption generator to create accurate captions for images.
Outcome: Allow visually impaired users to engage with images through contextual descriptions.

Dataset
Source: Kaggle - Flickr8k Dataset
Size: 8,000 images, each with five different captions.
Image Selection: Images from Flickr, depicting a variety of scenes and situations.

Methods Used
Dataset Downloading: Downloaded using Kaggle API; five captions per image.
Caption Preprocessing:
Removal of stopwords, punctuation, and unnecessary spaces.
Added start and end tokens.
Converted text to numerical format using Count Vectorizer.
Tokenized captions to integers.

Transfer Learning:

VGG16 pre-trained model used to extract image features.

LSTM Model Training:
LSTM (Long Short-Term Memory) used to train the network for caption generation.

Dual Input for Neural Network:
Combined image features and text embeddings for the neural network.

Merge and Caption Generation:
Merged image features and text embeddings in the neural network to generate captions.
Technologies and Softwares

Programming Language: Python

Computer Vision Libraries: OpenCV

Deep Learning Frameworks: TensorFlow, Keras
NLP Libraries: NLTK, TextBlob

Image Processing Libraries: Matplotlib, PIL

Pre-trained Models: VGG16

Text Preprocessing: Regular expressions (re), string operations

Required Packages

cv2 (OpenCV): Computer vision tasks
tensorflow, keras: Deep learning
nltk, textblob: NLP and text processing
pandas, numpy: Data manipulation and numerical computing
matplotlib: Data visualization
sklearn: Text vectorization
pickle: Object serialization

Results
Positive Examples:
Images where the model generated accurate captions.
Negative Examples:
Images with incorrect or nonsensical captions.
