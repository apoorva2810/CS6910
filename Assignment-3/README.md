# CS6910

## Assignment 3
Dataset :  Dakshina dataset released by Google
<br />&nbsp; &nbsp;Train words : 44204 words
<br />&nbsp; &nbsp;Validation words : 4358 words
<br />&nbsp; &nbsp; Test words : 4502 words
<br />&nbsp; **WITHOUT ATTENTION LAYER** &nbsp; &nbsp;
<br />&nbsp; &nbsp; The target hindi words have been preprocessed by adding '\t' and '\n' to each of the words in the given dataset
<br />&nbsp; &nbsp; The input data and target data of training dataset have been converted into one hot vectors and later we have used embedding on top of that.
<br />&nbsp; &nbsp; &nbsp; &nbsp;For Test data set, we have used one hot encoding for input text , not for target text.
<br />&nbsp; &nbsp; &nbsp; &nbsp; The model that we have built for seq2seq learning is based on character level modelling.Hence, it gives us character level accuracy. To  get the word level accuracy we have built the custom function ValAcc2().  
<br />&nbsp; &nbsp; &nbsp; &nbsp; model_run() function is being called to build the custom model.
<br />&nbsp; &nbsp; &nbsp; &nbsp; model_run() function also builds the suitable inference model 
<br />&nbsp; &nbsp; &nbsp; &nbsp; decode_sequence() function has been built to provide the predicted hindi words. Function decode_sequence1() is for single layer of encoder and decoder  model .Function decode_sequence2() is for 2 stacked layers of encoder and decoder models.
<br />&nbsp; &nbsp; &nbsp; &nbsp; beam_search_decoder() function has been built so that while predicting the words in decode_sequence() function , the beam search <br />&nbsp; &nbsp; &nbsp; &nbsp; algorithm can also be incorporated to provide better accuracy
<br />&nbsp; &nbsp; &nbsp; &nbsp; model_run() function internally calls all the other above mentioned functions and provides us with the validation/test accuracy 
<br />&nbsp; &nbsp; &nbsp; &nbsp; The best model for seq2seq learning has been built on GRU and has recorded the test accuracy of 33.8% for 2 layers of encoder and decoder
<br />&nbsp; &nbsp; &nbsp; &nbsp; All the predictions have been saved in the predictions_vanilla folder
<br />&nbsp; &nbsp; &nbsp; &nbsp; 

<br />&nbsp; **WITH ATTENTION** &nbsp; &nbsp;
<br />&nbsp; &nbsp; &nbsp; &nbsp;Similar preprocessing has been done before building the seq2seq model with attention layer
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp; The attention layer has been built on GRU model with single layer of encoder and decoder layers.
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;ValAcc2(), decode-sequence1(), beam_search_decoder() has been built for the same purpose as above
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;The model_run() function internally calls all the other functions and returns the accuracy needed
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp; Our best model with attention layer has recorded the test accuracy of 23.25% for one layer of encoder and decoder 
<br />&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp; We have also uploaded all the predictions made by this model in predictions_attention folder
<br />&nbsp; &nbsp; &nbsp; &nbsp;we have also created the attention heatmaps for 10 input words from test dataset. The heatmap images have been stored in the &nbsp; <br />&nbsp; &nbsp; &nbsp;Attentions_heatmap_images folder









      
      
             
 

   

