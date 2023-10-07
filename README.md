# thermal-image-object-detection
1[](https://github.com/foduucom/thermal-image-object-detection/blob/main/image.jpg)
## Summary
The YOLOv8 object Detection model is an obYOLOv8s Table Detectionject detection model based on the YOLO (You Only Look Once) framework. It is designed to thermal image detect object, whether they are thermal object detect, in images. The model has been fine-tuned on a vast dataset and achieved high accuracy in detecting tables and distinguishing between thermal object detect ones.

## Model Details
### Model Description
The YOLOv8 Object Detection model serves as a versatile solution for precisely identifying thermal object detect within images, whether they exhibit a object detect. Notably, this model's capabilities extend beyond mere detection – it plays a crucial role for object detection. By employing advanced techniques such as object detection.

We invite you to explore the potential of this model and its object detection capabilities. For those interested in harnessing its power or seeking further collaboration, we encourage you to reach out to us at info@foduu.com. Whether you require assistance, customization, or have innovative ideas, our collaborative approach is geared towards addressing your unique challenges. Additionally, you can actively engage with our vibrant community section for valuable insights and collective problem-solving. Your input drives our continuous improvement, as we collectively pave the way towards enhanced object detection.

## Developed by: FODUU AI
* Model type: Object Detection
* Task: Thermal Object Detection (object detection)
Furthermore, the YOLOv8 Detection model is limited to object detectionsetup environment python setup.py yolov8 object detection model alone. It is a versatile tool that contributes to the processing of structured image data. By utilizing advanced box techniques, the model empowers users to isolate object within the thermal image data. What sets this model apart is its seamless integration with object detection technology. The combination of box information allows for precise object detection from the thermal image data. This comprehensive approach streamlines the process of information retrieval from thermal image data.

User collaboration is actively encouraged to enrich the model's capabilities. By contributing table images of different designs and types, users play a pivotal role in enhancing the model's ability to detect a diverse range of object accurately. Community participation can be facilitated through our platform or by reaching out to us at info@foduu.com. We value collaborative efforts that drive continuous improvement and innovation in object detection.

Supported Labels
YOLOv8
```
['box', 'object detect']
```
## Uses
### Direct Use
The YOLOv8 for object Detection model can be directly used for detecting object from thermal images, whether they are bordered box.

### Downstream Use
The model can also be fine-tuned for specific object detection tasks or integrated into larger applications for distance measure, image-based object detection, and other related fields.

## Recommendations
Users should be informed about the model's limitations and potential biases. Further testing and validation are advised for specific use cases to evaluate its performance accurately.

Load model and perform prediction:

## How to Get Started with the Model
To get started with the YOLOv8s object Detection and Classification model, follow these steps:
```
pip install ultralyticsplus==0.0.28 ultralytics==8.0.43
```
### Load model and perform prediction:
```
from ultralyticsplus import YOLO, render_result
```
### load model
```
model = YOLO('foduucom/thermal-image-object-detection')
```
### set model parameters
```
model.overrides['conf'] = 0.25  # NMS confidence threshold
model.overrides['iou'] = 0.45  # NMS IoU threshold
model.overrides['agnostic_nms'] = False  # NMS class-agnostic
model.overrides['max_det'] = 1000  # maximum number of detections per image
```
### set image
```
image = '/path/to/your/document/images'
```
### perform inference
```
results = model.predict(image)
```
### observe results
```
print(results[0].boxes)
render = render_result(model=model, image=image, result=results[0])
render.show()
```

### Contact 
For inquiries and contributions, please contact us at - [info@foduu.com](mailto:info@foduu.com)
