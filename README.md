<img width="540" alt="image" src="https://github.com/vineetjangiriitb/23B0762_AIC/assets/147324232/afa06d6c-6d45-4a8d-b44f-476d56dee0a0"># 23B0762_AIC
Object detection model
![image](https://github.com/vineetjangiriitb/23B0762_AIC/assets/147324232/e3229eae-422a-4d38-9fbf-84bd9e08897f)
![image](https://github.com/vineetjangiriitb/23B0762_AIC/assets/147324232/78a7fa6b-398d-421e-842d-b44fc368dbd7)
![image](https://github.com/vineetjangiriitb/23B0762_AIC/assets/147324232/ff715a04-8364-4ca4-8095-f30112f5f07a)
![image](https://github.com/vineetjangiriitb/23B0762_AIC/assets/147324232/d46261a6-5843-4eed-ba9d-7223919b003c)
And more test images in my code

Detailed discussion on the performance of your model
I had trained my model on pre-trained Tensorflow hub FasterRCNN+InceptionResNetV2 model which is trained on Open Images V4, containing 600 classes, and modified the final layers of the model. It outputs the following features 
detection_boxes: a tf.float32 tensor of shape [N, 4] containing bounding box coordinates in the following order: [ymin, xmin, ymax, xmax].
detection_class_entities: a tf.string tensor of shape [N] containing detection class names as Freebase MIDs.
detection_class_names: a tf.string tensor of shape [N] containing human-readable detection class names.
detection_class_labels: a tf.int64 tensor of shape [N] with class indices.
detection_scores: a tf.float32 tensor of shape [N] containing detection scores.
Its Precision is 0.75, Recall is 1.0 and mAPis 0.5555555555555556 on test set of randomly chosen images from google. 

Challenges faced during model implementation and training phase: 

There were a lot of challenges when I was working on making the model. I was initially following some more complex strategies in which I was using Pascal VOC dataset and thought of first labelling all the images and then building some models for object detection from scratch in which I was trying to use the Imageset and annotation files files for object detection. Then after initial struggles and significant time investment, I thought of trying to instead find a suitable pre trained model for object detection model and then fine tuning it to get the required results. It also required significant efforts to calculate various metrics which were asked to do which I eventually did using the confidence scores of image detection and manually finding true labels for the images as the dataset consisted of randomly selected google images. Finding right sources for getting related information was also a task as even ChatGPT sucks at various places in this😅. Overall the project was a great learning experience and truly enjoyed doing it.

Some improvements and alternative approaches:

It is still not a highly accurate model and training with more data can help in increasing its performance metrics and overall working. Performing extensive hyperparameter tuning, including learning rates, anchor box scales, and aspect ratios, to find the optimal settings for the model.  Model pruning and quantization can also be applied to reduce model size and improve inference speed without substantial loss in accuracy.
Model can also be modified to even detect objects in moving video objects which is also important in some of real world tasks.

Sources of reference-
https://www.kaggle.com/models/google/faster-rcnn-inception-resnet-v2/tensorFlow1/faster-rcnn-openimages-v4-inception-resnet-v2/1?tfhub-redirect=true
https://www.tensorflow.org/hub/tutorials/object_detection
https://www.tensorflow.org/lite/examples/object_detection/overview
https://www.tensorflow.org/tutorials/images/classification
https://www.youtube.com/watch?v=-ZyFYniGUsw&t=348s

