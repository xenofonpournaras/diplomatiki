# In-browser Object Detection


## **Information** ##

With this web app the user can easily run COCO-SSD and TINY YOLO in the browser in order to make in-browser detection. More specifically, COCO-SSD is provided by TensorFlow.js and TINY YOLO from ml5.js. Both models are trained on COCO dataset and can detect up to 80 object categories. The app consists of 5 UIs. Based on the device that the user is using and the choice of the model, the start.html file redirects him to the responsible web page.

## **Supported Modes** ## 
The supported modes for both models are four:
1. Snapshot detection 
2. Video detection 
3. Detection od imported image 
4. Save of file with the predictions of the models (*for the creation of the blob file "FileSaver.js" is used, that its derived from* https://github.com/eligrey/FileSaver.js/)

## **Model Characteristics** #
1. COCO-SSD: The feature extractor of this model is "lite_mobilenet_v2" since it is the smallest model in size that is provided by TensorFlow.js. The reason is that the small size of this model is more suitable for the efficient running of the app in mobile devices.

2. TINY YOLO: The model is provided by ml5.js. The configurations of the model are the following: the IOU threshold is set on 0.4 and the  class propability threshold is set on 0.3.

## **Functions** ##
**laptop or Desktop use:** The ```javascript
getUserMedia()``` method is used for the 

