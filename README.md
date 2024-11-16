# Brain Tumor Classification App

Check out the live application 🔗<a href="https://brain-tumor-classification-atkjyturudaene3bsmurrr.streamlit.app/" target="_blank">LINK</a>

A Streamlit application for classifying brain MRI scans to detect tumors using multiple deep learning models. The app generates saliency maps to highlight important regions and provides expert explanations using advanced language models.

## Live Demo



https://github.com/user-attachments/assets/d269ee21-35e5-4d64-98f9-454d1fdd3265



## Features

- **Image Classification**: Classify MRI scans into Glioma, Meningioma, Pituitary, or No Tumor.
- **Multiple Models**: Compare predictions and saliency maps from Xception, ResNet, and Custom CNN models.
- **Saliency Maps**: Visualize model focus areas on MRI scans.
- **Explanations**: Generate expert-level explanations using Gemini, Llama, or ChatGPT language models.
- **Probability Distribution**: View probability distributions across different classes and models.

## Technologies

- **Framework**: Streamlit
- **Deep Learning**: TensorFlow, Keras
- **Visualization**: OpenCV, Plotly
- **Language Models**: OpenAI, Google Generative AI, Llama

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/aishasalim/btc.git
   cd btc
   ```

2. **Create a Virtual Environment**

   ```bash
   python@3.11 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables**

   Create a `.env` file in the project root with the following keys:

   ```
   GROQ_API_KEY=your_groq_api_key
   OPEN_AI_KEY=your_openai_api_key
   GOOGLE_API_KEY=your_google_api_key
   ```

## Usage

1. **Run the Streamlit App**

   ```bash
   streamlit run app.py
   ```

2. **Interact with the App**
   - Upload a brain MRI image (`.jpg`, `.jpeg`, `.png`).
   - Select one or more models to compare.
   - View classification results, saliency maps, and probability distributions.
   - Generate expert explanations using the selected language model.

## Models

- **Transfer Learning - Xception**

  - Input Size: 299x299
  - Weights: Pre-trained on ImageNet

- **ResNet**

  - Input Size: 224x224
  - Custom architecture with ResNet50 base

- **Custom CNN**
  - Input Size: 224x224
  - Custom convolutional neural network

## Requirements

- Python 3.10+
- Streamlit
- TensorFlow
- Keras
- OpenCV
- Plotly
- Google Generative AI SDK
- OpenAI SDK
- Other dependencies listed in `requirements.txt`
