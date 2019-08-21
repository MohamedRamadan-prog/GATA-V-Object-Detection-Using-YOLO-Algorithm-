# “YOLO Algorithm”
- YOLO ("you only look once") is a popular algorithm because it achieves high accuracy while also being able to run in real-time, almost clocking 45 frames per second. A smaller version of the network, Fast YOLO, processes an astounding 155 frames per second. Noting that in order to achieve these fps results, we need to have powerful GPUs.
- This algorithm requires only one forward propagation pass through the network to make predictions. After non-max suppression, it then outputs recognized objects together with the bounding boxes.

![image](https://user-images.githubusercontent.com/53750465/63397090-b724dd00-c3c9-11e9-9b40-13b7a6bce413.png)


YOLO is an object detection pipeline based on Neural Network. Contrast to prior work on object detection with classifiers to perform detection, YOLO frame object detection as a regression problem to spatially separated bounding boxes and associated class probabilities. A single neural network predicts bounding boxes and class probabilities directly from full images in one evaluation. Since the whole detection pipeline is a single network, it can be optimized end-to-end directly on detection performance.

![image](https://user-images.githubusercontent.com/53750465/63397117-d0c62480-c3c9-11e9-9afe-e920b2e7e360.png)


Steps to use the YOLO for detection:
I) Resizing the input image to 448x448
II) Running a single convolutional network on the image
III) Thresholding the resulting detections by the model’s confidence


![image](https://user-images.githubusercontent.com/53750465/63397130-e0de0400-c3c9-11e9-8d0a-e6c02f05cf2e.png)

