### Text Classification Using DNN Architectures
This is the repository for sentiment analysis of the **Amazon Reviews Sentiment Dataset**. We have created models based on Convolutional Neural Networks, Recurrent Neural Networks and Hierarchical Attention Networks. We have then compared the performance of these networks based on accuracy and loss.

### Project Setup
Since the project requires training deep networks, we will be requiring a GPU. To facilitate this, the project is done using Google Colab.

### Dataset:
* The dataset contains 4 million customer reviews.
* Each review consists of text along with the number of stars (1-5). Higher the stars better the rating. 
* Finally each review has been categorized as either positive or negative.

### Preprocessing: Amazon Reviews Classification.ipynb
* This file preprocesses the entire 4 million reviews of training and test dataset.
* It includes steps such as converting data to UTF-8 format, separation of labels and reviews, removal of URL’s, removal of stopwords, removing punctuations, extra spaces and digits etc. 
* It then performs tokenization and padding of input data to make it ready to be fed to NN models. 
* The embedding matrix, which serves as the initial weights (word vectors) for the DNN models are also prepared here and stored for future use.

### Convolutional Neural Network: Amazon_Reviews_CNN.ipynb
* This file defines and trains the CNN model using the preprocessed train reviews and labels and evaluates it on test_reviews and labels. 
* The code for loading the pre-processed data is given in the file. 
* The Results of the code are stored in CNN/Result folder
* Pretrained model (1 million train + Validation) is present in CNN/Result folder.

### Recurrent Neural Network: RNN.ipynb 
* This file is the implementation of the Recurrent Neural Network on the Amazon Reviews dataset
* The Results of the code are stored in RNN/Result folder
* The hierarchically prepared test and train data are located in RNN/Code folder
* Pretrained model (1 million train + Validation) is present in RNN/Result folder

### Hierarchical Attention Network: HAN.ipynb 
* This file is the implementation of the Hierarchical Attention Network on the Amazon Reviews dataset
* The Results of the code are stored in HAN/Result folder
* The hierarchically prepared test and train data are located in HAN/Code folder
* Pretrained model (1 million train + Validation) is present in HAN/Result folder
