# YOLOv8

### YOLOv8 installing

```pip install ultralytics``` 

### Data format

```
./datasets/score   # 存放的文件，score是数据集的名称
├─images           # 训练图像，每个文件夹下存放了具体的训练图像
│  ├─train
│  └─val
└─labels           # label，每个文件夹下存放了具体的txt标注文件，格式满足YOLOv5
    ├─train
    └─val
``` 

### For training
  
```yolo task=detect mode=train model=yolov8s.yaml  data=score_data.yaml epochs=100 batch=64 imgsz=640 pretrained=False optimizer=SGD```   

### Demo

```python3 inference.py``` 
