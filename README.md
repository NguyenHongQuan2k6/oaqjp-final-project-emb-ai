# Emotion Detector – AI-based Web Application

Final project for the IBM course *Developing AI Applications with Python and Flask*.

**Emotion Detector** is a Flask web application that analyzes a piece of text with the
**Watson NLP Emotion Predict** service and returns the scores for five emotions
(anger, disgust, fear, joy, sadness) together with the dominant emotion.

## Project structure

```
EmotionDetection/
    __init__.py               # makes EmotionDetection a package
    emotion_detection.py      # emotion_detector() – calls Watson NLP and formats the output
server.py                     # Flask web server (route /emotionDetector)
test_emotion_detection.py     # unit tests
templates/index.html          # web interface
static/mywebscript.js         # front-end script
```

## Run

```bash
python3.11 -m pip install flask requests pylint
python3.11 server.py            # open http://localhost:5000
python3.11 test_emotion_detection.py
pylint server.py
```
