# 🍳 PantryChef - Smart AI Recipe Suggestion System

PantryChef is an AI-powered web application that helps users transform their available kitchen ingredients into delicious meals. By using Machine Learning for ingredient recognition and the Google Gemini API for recipe generation, PantryChef offers a seamless way to reduce food waste and discover new culinary creations.

## ✨ Features
* **AI-Powered Recipe Suggestions**: Get intelligent recipe recommendations based exactly on what you have available.
* **Image Recognition**: An advanced CNN model identifies ingredients directly from photos.
* **Gemini API Integration**: Uses Google's generative AI to provide detailed, step-by-step cooking instructions.
* **Manual Ingredient Entry**: Allows users to supplement detected items with manual text input via the interface.
* **User Authentication**: Secure sign-up and login functionality powered by Firebase.
* **Community & Feedback**: Dedicated sections for sharing recipes with a community and providing feedback.

## 🛠️ Tech Stack
* **Backend**: Flask (Python)
* **Machine Learning**: TensorFlow & Keras (CNN Architecture)
* **Generative AI**: Google Gemini API (`gemini-1.5-pro`)
* **Database & Auth**: Firebase Admin SDK & Firebase Web SDK
* **Frontend**: HTML5, CSS3, JavaScript (jQuery)

## 📂 Project Structure
* **`app.py`**: The core Flask application handling routing, file uploads, and service integration.
* **`train.py`**: Script for training the Convolutional Neural Network (CNN) on ingredient datasets.
* **`predict.py`**: Handles image preprocessing and ingredient classification using the trained model (`food_classifier.h5`).
* **`generate.py`**: Communicates with the Google Gemini API to generate recipes based on ingredients.
* **`static/`**: Contains CSS files, uploaded images, and other assets.
* **`templates/`**: Contains the frontend HTML files (e.g., `generator.html`, `index.html`, `login.html`).

## 🚀 Getting Started

### 1. Prerequisites
Ensure you have Python installed, then install the required dependencies:
```bash
pip install flask tensorflow google-generativeai firebase-admin werkzeug numpy matplotlib
