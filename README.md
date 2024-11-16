## Small Object Detection Using the Lacmus Drone Dataset(LADD)

LADD is a dataset created by non-profit search and rescue volunteer organizations dedicated to finding missing persons (Owl, LisaAlert). The data is collected using drones and labeled with machine learning tools. The pictures were taken from a height of 40-50 meters, horizontally. The pictures depict people in various poses. The dataset consists of 1365 images. LADD annotations are available in VOC - Xmax, Ymax Xmin, Ymin and YOLO - XYWH formats.

#### Dataset Features
* Includes images of people
* Focuses on small object detection

#### Challenges

* Training the model to be able to detect small objects i.e persons in complex environments terrains and in various lighting conditions

#### Overcoming limitations

* Utilised `YOLO11-large` model to train on the dataset
* Tiling the images as a preprocessing step to enhance model's performance in small object detection
* Utilising `SAHI(Slicing Aided Hyper Inference)` to slice images and predict on each slice to improve the inference
