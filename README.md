# Final Project

## Final Project: Emotion Detection with Python and Flask

**Project name: Final Project**

基于 Flask 和 Watson NLP 的人工智能情感检测器，提供五类情感输出：anger、disgust、fear、joy、sadness。

## Run

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python server.py
```

Open http://127.0.0.1:5000. API endpoint: `POST /api/emotion` with JSON `{"text":"I love this"}`.

## Tests and static analysis

```bash
python -m unittest discover -s tests -v
python -m py_compile emotion_detection.py server.py
```
