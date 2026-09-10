# 🌾 Crop Disease Prediction using Deep Learning and Large Language Models (LLMs)

This project is an AI-powered crop disease prediction system that identifies diseases from crop leaf images using deep learning models. It combines computer vision with Large Language Models (LLMs) to provide farmer-friendly explanations, symptoms, treatment guidance, and prevention recommendations.

The system uses **Google Gemini 2.5 Flash** to generate contextual responses based on the predicted disease, user's question, and selected language.

## Features

* 🌿 Crop disease detection from leaf images
* 🤖 Deep learning models for image classification
* 🧠 Transfer learning using multiple CNN architectures
* 📊 Model evaluation using accuracy, precision, recall, F1-score, and ROC-AUC
* 📈 Training curves, confusion matrices, and model comparison visualizations
* 💬 Google Gemini 2.5 Flash for AI-generated disease explanations and recommendations
* 🌐 Hindi, English, and Hinglish language support
* 📝 Farmer-friendly symptoms, treatment, and prevention guidance
* 📄 PDF report generation
* 💡 Local knowledge-base fallback when the LLM service is unavailable
* 🖥️ Interactive Streamlit web application
* 🧪 Testing modules for model and LLM functionality
* 📂 Modular project structure for easy maintenance and future development

## Technologies Used

* Python
* PyTorch
* Torchvision
* Streamlit
* OpenCV
* Pillow
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Google Gemini 2.5 Flash
* Google GenAI SDK
* ReportLab

## Project Structure

* `app/` – Application components
* `src/` – Source code, prediction, training, and utility modules
* `models/` – Trained deep learning models
* `outputs/` – Generated outputs and evaluation results
* `results/` – Model performance results and visualizations
* `research_outputs/` – Research and experimental outputs
* `tests/` – Testing modules
* `disease_info.json` – Local crop disease information used for fallback responses
* `streamlit_app.py` – Main Streamlit web application
* `requirements.txt` – Python dependencies

## Deep Learning Models

The project includes multiple deep learning architectures for crop disease classification:

* EfficientNet-B0
* MobileNetV2
* ResNet18
* VGG16

These models are used for experimentation, training, prediction, and performance evaluation.

## LLM Integration

The project integrates **Google Gemini 2.5 Flash** to provide contextual agricultural assistance after disease prediction.

The LLM uses:

* Predicted crop disease
* User's question or problem description
* Selected language

to generate farmer-friendly information including:

* Disease explanation
* Symptoms
* Treatment guidance
* Prevention recommendations

A local `disease_info.json` knowledge base is also available as a fallback when the Gemini service is unavailable.

## Application Workflow

```text
Crop Leaf Image
       ↓
Image Preprocessing
       ↓
Deep Learning Model
       ↓
Disease Prediction
       ↓
Confidence Score
       ↓
Google Gemini 2.5 Flash
       ↓
Disease Explanation & Recommendations
       ↓
PDF Report
