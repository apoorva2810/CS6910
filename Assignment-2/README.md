# CS6910

## Assignment 2
Dataset : inaturalist 
<br />&nbsp; &nbsp;Train Images : 4500 images 
<br />&nbsp; &nbsp;Validation Images : 500 Images
<br />&nbsp; &nbsp; Test Images : 1000 Images
**PART A** &nbsp; &nbsp;
<br />&nbsp; &nbsp; The images used for training/validating/testing the CNN model are of dimensions 350 x 350 x 3
<br />&nbsp; &nbsp; Before running the model , we need to preprocess the images.
<br />&nbsp; &nbsp; &nbsp; &nbsp; We have changed the images to Numpy Array first and then rescaled the images so that the pixel values are between 0 and 1.
<br />&nbsp; &nbsp; &nbsp; &nbsp; We have divided the 'Training data' into Train Data and Validation Data. Validation data comprises of 10% of the 'Training data' that is used &nbsp; &nbsp; &nbsp; &nbsp;for hyperparameter tuning
<br />&nbsp; &nbsp; &nbsp; &nbsp; Then we change the labels of the train/validation/test images to categorical values using the to_categorical() function
<br />&nbsp; &nbsp; &nbsp; &nbsp; Now, we will define the model structure using model_run()
<br />&nbsp; &nbsp; &nbsp; &nbsp; train() function will actually call the model_run() function internally and report the accuracy of the model that has been chosen by sweep &nbsp; &nbsp; &nbsp; &nbsp; configuration


      
      
             
 

   

