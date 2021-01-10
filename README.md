# CV_PA4


Run the pre-trained YOLO-V3 object detector on a sample image.
Run the pre-trained YOLO-V3 object detctor on images from PETS dataset.
From the object detected images we will create a top/satellite view.

Task 1: Preapring the pre-trained model for a test run
Evaluate the performance of a pretrained network YOLO-V3 on a sample zebra image provided to you:

Download the pre-trained model weights file "yolov3.weights"(provided to you) and place them into your current working directory.
Download the "yolo3.py" file provided to you and place it into your current working directory, this file contains all the helper functions we will be using for this part.
Define the Keras model for YOLOv3 and load the downloaded weight file into this model.
Run it on the sample image "zebra.jpg" provided to you.

Task 2: Visualizing extracted predictions as bounding boxes

We have extracted predictions from the object detctor that you can observe are very accurate too. Now we need to visualize these predictions as bounding boxes on the input image. For this part you are supposed to wite a function "draw_boxes" to visualize your predictions as bounding boxes. Inputs to this function will be outputs of the function "get_boxes". This function should also save the image along with the bounding boxes in your current working directory. Also show the predicted label and score for each bounding box. Sample output is shown to you.

![WhatsApp Image 2021-01-10 at 7 35 38 PM](https://user-images.githubusercontent.com/46634351/104126037-2662ee80-537c-11eb-95d5-c7e1a0d2680c.jpeg)

Task 3: Perfroming object detection on all images in the PETS dataset(provided to you)

Now when you have succesfully executed the code for object detection, we want you to perform object dection on all images in the PETS dataset provided to you and save them in a seperate folder in your working directory. In this part you will perform object detection in each of the images from different camera views in the PETS dataset. You have been given 10 images per view and 3 views in total.

![7037b988-a5f7-4c00-8cef-df934730b1e0](https://user-images.githubusercontent.com/46634351/104126055-501c1580-537c-11eb-8ad7-16aa44fb620b.jpg)


![6c6ef3c6-00a1-4ae1-90cd-1f4454d204e8](https://user-images.githubusercontent.com/46634351/104126069-6a55f380-537c-11eb-9c72-841f1fabc02a.jpg)

Task 4: Viewing detected object location on Top View/Satellite view
In this part we will use the output from the previous part to project the location of detected objects on the top view/satellite view so that we can analyze all the objects present in the scene in one single view.

![a796f4fe-135b-40ec-91b9-867d48f59491](https://user-images.githubusercontent.com/46634351/104126082-822d7780-537c-11eb-9903-757529cde61e.jpg)


![d2ed77ef-5780-48bb-b338-318733a7733d](https://user-images.githubusercontent.com/46634351/104126093-91142a00-537c-11eb-91a1-53a8ef48b600.jpg)


In this task you will :

Go to the following link (http://maps.google.co.uk/maps?f=q&source=s_q&hl=en&geocode=&q=university+of+reading&sll=51.438895,-0.945747&sspn=0.007544,0.014055&ie=UTF8&ll=51.438895,-0.945747&sspn=0.007544,0.014055&ie=UTF8&ll=51.438534,-0.944561&spn=0.000943,0.001757&t=h&z=19) and capture a satellite view of the area that has been shown in the images of the PETS dataset
Now perform object detection on all the images from PETS dataset provided to you.
Find the corresponding points in the satellite view image and any one of your object detected images.
Compute the homography between the corresponding points.
Object detector will give you a list of bounding boxes, note the mid-point of the base of bounding box and project it on to the top view/satellite view using the computed homography. Top view/satellite view generated from a sample object detected image is provided to you for better understanding.
Save all the top view images in a seperate folder in your working directory and submit it with the assignment on LMS.
You need to perform all the above mentioned steps for each view seperately.

