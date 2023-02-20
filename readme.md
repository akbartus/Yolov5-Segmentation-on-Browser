<p align="center">
  <img src="img/screenshot.jpg" />
</p>


This is adapted and reduced version of YOLOv5 object segmentation (powered by onnx) created by <a href="https://github.com/Hyuto/yolov5-seg-onnxruntime-web">Wahyu Setianto</a>. This version can be run on JavaScript without any frameworks.

## Setup
To see it at work, just run index.html file. 

## Models

**Main Model**

YOLOv5n-seg model converted to onnx.

```
used model : yolov5n-seg.onnx
size       : ~ 8Mb
```

**NMS**

ONNX model to perform NMS operator [CUSTOM].

```
nms-yolov5.onnx
```

**Mask**

ONNX model to produce mask for every object detected [CUSTOM].

```
mask-yolov5-seg.onnx
```

## Use another model

It is possible to use bigger models converted to onnx, however this might impact the total loading time.

To use another YOLOvv model, download it from Ultralytics and convert it to onnx file format. Read more on the [official documentation](https://docs.ultralytics.com/tasks/segmentation/#export)

**Custom YOLOv5 Segmentation Models**

Please update labels object inside of main.js file.

## Demo
To see it at work, please visit the <a href="https://yolov5-segmentation.glitch.me/">following page</a>
