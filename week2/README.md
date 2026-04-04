# Week 2 – YOLO Object Detection

## Virtual Environment Setup

Created Python virtual environment:

python3 -m venv cv_env
source cv_env/bin/activate

## Installed Ultralytics

pip install ultralytics

## Object Detection Execution

Command used:

yolo predict model=yolov8n.pt source='https://ultralytics.com/images/bus.jpg'

## Output

Detected:

4 persons
1 bus
1 stop sign

Output saved in:

runs/detect/predict
