# <div align="center" markdown>

# Datasets samples

<p align="center">
  <a href="#Overview">Overview</a> •
  <a href="#Test samples">Test samples</a>
</p>

</div>


# Overview

This repository contain test datasets provide by [Supervisely](https://supervisely.com/).

### Supporting formats:
1. [COCO](https://cocodataset.org/)
2. [YOLO](https://learnopencv.com/yolov5-instance-segmentation/)
3. [Cityscapes](https://www.cityscapes-dataset.com/)
4. [PascalVOC](http://host.robots.ox.ac.uk/pascal/VOC/)

### Supporting shapes:
1. Polygon
2. Rectangle
3. PNG masks (convert to Bitmap)

# Test samples

## Data structure 

*empty folders are empty only for this cases

### COCO
```
.
├── annotations
│   └── instance.json
└── img
    └── images samples
'''
### YOLO
'''
├── images
│   ├── train
│   │   ├── image_x.extension
│   │   ├── ...
│   │   └── images.extension
│   └── val
│       └── empty
├── dogs
│   ├── train
│   │   ├── image_x.txt
│   │   ├── ...
│   │   └── images.txt
│   └── val
│       └── empty
└── data_config.yaml
```
### Cityscapes
```
├── gtFine
│   ├── test/ds1
│   │   ├── image_x_object_mask.png
│   │   ├── image_x_class_mask.png
│   │   ├── image_x_polygons_mask.json
│   │   ├── ...
│   │   └── images.extension
│   ├── train/ds1
│   │   ├── image_y_object_mask.png
│   │   ├── image_y_class_mask.png
│   │   ├── image_y_polygons_mask.json
│   │   ├── ...
│   │   └── images.extension
│   └── val/ds1
│       ├── image_z_object_mask.png
│       ├── image_z_class_mask.png
│       ├── image_z_polygons_mask.json
│       ├── ...
│       └── images.extension
├── leftImg8bit
│   ├── test
│   │   ├── image_x.png
│   │   ├── ...
│   │   └── images.extension
│   ├── train
│   │   ├── image_y.png
│   │   ├── ...
│   │   └── images.extension
│   └── val
│       ├── image_z.png
│       ├── ...
│       └── images.extension
└── class_to_id.json
```

### PascalVOC for Rectangles
```
├── annotations
│   ├── image_x.xml
│   ├── ...
│   └── images.xml
└── images
    ├── image_x.extension
    ├── ...
    └── images.extension
```

### PascalVOC with PNG masks
```
├── JPEGImages
│   └── images
├── SegmenationClass
│   └── PNG class masks
├── SegmenationObject
│   └── PNG object masks
├── Annotations
│   └── XML annotations for each image
├── ImageSets
│   ├──Main
│   │   ├── kiwi_train.txt
│   │   ├── ...
│   │   └── val.txt
│   └── Segmentation
│       ├── train.txt
│       ├── ...
│       └── val.txt
└── colors.txt
```

