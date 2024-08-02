# YOLOv8

### YOLOv8 installing

```pip install ultralytics``` 

### Data format

```
./datasets/score   # dataset
├─images           # images
│  ├─train
│  └─val
└─labels           # label, txt files, YOLOV5 format
    ├─train
    └─val
``` 

### For training
  
```yolo task=detect mode=train model=yolov8s.yaml  data=score_data.yaml epochs=100 batch=64 imgsz=640 pretrained=False optimizer=SGD```   

### Demo

```python3 inference.py``` 
