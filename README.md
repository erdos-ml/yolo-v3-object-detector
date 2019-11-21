# yolo-v3-object-detector

This repository contains the code to create and run a pretrained object
detection model named YOLOv3. the model is trained on the MSCOCO dataset.
The code is based pretty much in it's entirety on the GitHub repository
keras-yolo3 created by the user experiencor.

I made some minor additions needed in order to be able to run it in my computer.




### Instructions to use the model:

1. Download the pretrained weights to the model using the following link:

   <a href="https://pjreddie.com/media/files/yolov3.weights">YOLOv3
   Pre-trained Model Weights (yolov3.weights) (237 MB)</a>

2. Run the yolo_prepare_model.py script in order to create the model.h5 file
   which will contain the model.

3. Use the yolo_predict.py script to make predictions on individual images. To
   do this correctly do the following steps:

   i. Look at the **labels** variable in the script to see all the classes
      which the model was trained to predict.

   ii. Download from Google Images an image of one of the classes (e.g., an
      image of an airplane or a sandwich) and save it in the same directory as
      the script. (Make sure the image is in .jpg format)

  iii. Look for the **photo_filename** variable in the yolo_predict.py script
       and change its value to a string with the name of the image you
       downloaded (e.g., photo_filename = 'sandwich.jpg')

  iv. Run the yolo_predict.py script.

The outputs of the script will be your image with a bounding box around the
object along with the label and confidence score.
