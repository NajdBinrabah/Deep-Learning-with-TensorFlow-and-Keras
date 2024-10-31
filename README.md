<h1 align="center">Deep Learning with TensorFlow & Keras: Emotion Detection in Audio</h1>

<p align="center">This personal project uses Deep Learning, to classify emotions in audio data, employing TensorFlow, Keras, and Librosa.</p>

---

This project explores the use of Deep Learning for classifying emotions in audio data, leveraging the capabilities of TensorFlow and Keras alongside Librosa for audio analysis. The aim is to address an audio classification problem, exploring how different Deep Learning models such as LSTMs and 1D CNNs handle the unique challenges of audio data.

<h3>Libraries Used</h3>

- **TensorFlow & Keras:** For building, training, and evaluating Deep Learning models.
- **Librosa:** For audio analysis, particularly feature extraction, which converts audio files into numerical representations that the model can interpret.

<h3>Models and Techniques Explored</h3>

**1. Feature Extraction with Librosa**
-	Mel-frequency cepstral coefficients (MFCCs)
-	Chroma features
-	Mel spectrogram

**2. Long Short-Term Memory (LSTM) and 1D Convolutional Neural Network (1D CNN) Models**

Two Deep Learning models were evaluated:
-	**LSTM (Long Short-Term Memory):** LSTM networks were developed to address the vanishing/exploding gradient problem in traditional RNNs. Known for capturing long-term dependencies, LSTMs are suited for sequential data. However, they may be overly complex for short, simple audio clips, potentially leading to overfitting in a dataset like this one.
-	**1D CNN (1D Convolutional Neural Network):** A simpler model architecture adapted for sequential data, such as audio. 1D CNNs apply convolution filters along a single axis, processing information across time or sequence dimensions. This makes them ideal for tasks like time-series analysis or audio classification, where short-term dependencies are key. In this case, the 1D CNN proved more compatible with the dataset, demonstrating smoother convergence and improved accuracy.
