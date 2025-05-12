# Traffic Accident Prediction and Chatbot Solution

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange)
![Flask](https://img.shields.io/badge/Framework-Flask-green)

A machine learning-based solution to predict traffic accidents and a chatbot for real-time safety recommendations.

## Overview

This project combines predictive analytics and an interactive chatbot to enhance road safety. It uses historical traffic data to train accident prediction models and provides real-time feedback via a chatbot. The system aims to reduce accidents through data-driven insights and user engagement.

## Features

### Machine Learning Models
- **Logistic Regression**: Binary classification for accident occurrence (78% accuracy).
- **Random Forest**: Improved accuracy (85%) with feature importance analysis.
- **Neural Network**: Deep learning model achieving 89% accuracy.

### Chatbot Capabilities
- Real-time accident risk assessment based on user input.
- Safety recommendations using historical trends and road conditions.
- Integration with weather/traffic APIs for dynamic risk evaluation.
- NLP-driven interactions (future: multi-language and voice support).

## Installation

1. **Clone the repository**:
   
   ```bash
   git clone https://github.com/yourusername/accident-prediction-chatbot.git
   ```
   ```bash
    cd accident-prediction-chatbot
   ```
3. **Set up a virtual environment**:
   ```bash
   python -m venv venv
   ```
   for linux base computers
   ```bash
   source venv/bin/activate
   ```
   for windows base computers
   ```bash
   venv\Scripts\activate
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
## Usage
### Training the Models
Run the training scripts:
```bash
python train_models.py
```
### Starting the Chatbot
Launch the Flask server:
```bash
python app.py
```
Access the chatbot at [http://localhost:5000](http://localhost:5000) via a web browser or API client.

### Starting the Chatbot CLI
Launch the command line interface:
```bash
python chatbot.py
```
## Dataset
The dataset includes 840 records with 14 features:
- Weather, road type, time of day, traffic density, speed limit, driver age/experience, alcohol influence, etc.
- Target variable: Accident Occurrence (0 = No Accident, 1 = Accident).

Preprocessing steps: Missing values filled with averages, one-hot encoding for categorical data, and feature scaling.

Results

| Model               | Accuracy | F1-Score |
|---------------------|----------|----------|
| Logistic Regression | 78%      | 76%      |
| Random Forest      | 85%      | 83%      |
| Neural Network     | 89%      | 86%      |

Key predictors: Weather, road type, speed limit, and traffic density.

### Limitations & Future Improvements
#### Current Limitations
- Class imbalance (fewer accident cases).
- Lack of real-time data integration (e.g., live traffic).
- Excludes factors like driver fatigue.

#### Planned Enhancements
- Integrate real-time GPS/weather APIs.
- Add voice commands and multi-language support.
- Apply deep reinforcement learning for adaptive predictions.
- Expand dataset with diverse accident scenarios.

## References
- James, G., et al. (2013). An Introduction to Statistical Learning.
- Bishop, C. M. (2006). Pattern Recognition and Machine Learning.
- Zhang, H., & Baker, T. (2021). AI in Road Safety (IEEE).


   
