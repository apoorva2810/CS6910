# CS6910

## Assignment 2
Dataset : inaturalist 
<br />&nbsp; &nbsp;Train Images : 4500 images 
<br />&nbsp; &nbsp;Validation Images : 500 Images
<br />&nbsp; &nbsp; Test Images : 1000 Images
<br />&nbsp; **PART A** &nbsp; &nbsp;
<br />&nbsp; &nbsp; The images used for training/validating/testing the CNN model are of dimensions 350 x 350 x 3
<br />&nbsp; &nbsp; Before running the model , we need to preprocess the images.
<br />&nbsp; &nbsp; &nbsp; &nbsp; We have changed the images to Numpy Array first and then rescaled the images so that the pixel values are between 0 and 1.
<br />&nbsp; &nbsp; &nbsp; &nbsp; We have divided the 'Training data' into Train Data and Validation Data. Validation data comprises of 10% of the 'Training data' that is used &nbsp; &nbsp; &nbsp; &nbsp;for hyperparameter tuning
<br />&nbsp; &nbsp; &nbsp; &nbsp; Then we change the labels of the train/validation/test images to categorical values using the to_categorical() function
<br />&nbsp; &nbsp; &nbsp; &nbsp; Now, we will define the model structure using model_run()
<br />&nbsp; &nbsp; &nbsp; &nbsp; train() function will actually call the model_run() function internally and report the accuracy of the model that has been chosen by sweep &nbsp; &nbsp; &nbsp; &nbsp; configuration
<br />&nbsp; &nbsp; &nbsp; &nbsp; The best test accuracy reported by our CNN model is 35.5 %
<br />&nbsp; &nbsp; &nbsp; &nbsp; We have also visualized the filters of the first hidden layer of the model for a random image . 
<br />&nbsp; &nbsp; &nbsp; &nbsp; We have also plotted 30 images from our test dataset with their predicted and actual labels.
<br />&nbsp; &nbsp; &nbsp; &nbsp; Finally , Guided Backpropagation on a random image has been done. 
<br />&nbsp; &nbsp; &nbsp; &nbsp; All the results/plots are displayed in the report.

<br />&nbsp; **PART B** &nbsp; &nbsp;
<br />&nbsp; &nbsp; &nbsp; &nbsp;The pretrained models that we have used while working on this project are as follows :
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp; *VGG16
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp; *VGG19
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp; *ResNet50
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp; *InceptionResNetV2
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp; *Xception
<br />&nbsp; &nbsp; &nbsp; &nbsp;create_model() is used to initialize the chosen pretrained model by imagenet weights. 
<br />&nbsp; &nbsp; &nbsp; &nbsp;Then we call model_layer_freeze() is used to freeze the appropriate hidden layers based on sweep configuration.
<br />&nbsp; &nbsp; &nbsp; &nbsp; Finally testModel() is called to run the model and report the train/test accuracy 
<br />&nbsp; &nbsp;The best performing models that we encountered with the inaturalist dataset after all the experiments are InceptionResNetV2 and Xception
<br />&nbsp; **PART C** &nbsp; &nbsp;
<br />&nbsp; &nbsp; &nbsp; &nbsp;We have used a YOLO model that has been trained on images having Ambulances . This model is hence efficient enough to detect ambulances in real &nbsp; &nbsp; &nbsp; &nbsp;time scenarios.
<br />&nbsp; &nbsp; &nbsp; &nbsp; We have tested the model on a test video . The performance of the model can be viewed on the given link 
<br />&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;[YOLO Ambulance Detection](https://www.youtube.com/watch?v=t65xGPpDVCw)







      
      
             
 

   

