# CNN-with-different-kernel-size-for-sentence-classification
Convolutional Neural Network (CNN) with different kernel size for sentence classification


This problem is a famous subject in text classification. The classification of IMDB data was made using a CNN with different kernel size.

![CNN-Text](https://user-images.githubusercontent.com/17083899/57735599-d4049280-76ad-11e9-9877-abe14219b312.png)

Here, There are three filter region sizes: 2, 3 and 4, each of which has 2 filters. Every filter carries out convolution on the sentence matrix and creates (variable-length) feature maps. Then 1-max pooling is performed over each map, i.e., the largest number from each feature map is recorded. Thus a univariate feature vector is generated from all six maps, and these 6 features are concatenated to form a feature vector for the penultimate layer. The final softmax layer then receives this feature vector as input and uses it to classify the sentence; here we assume binary classification and hence depict two possible output states.


References: 
1 - http://www.wildml.com/2015/11/understanding-convolutional-neural-networks-for-nlp/
2 - Zhang, Y., & Wallace, B. (2015). A Sensitivity Analysis of (and Practitioners’ Guide to) Convolutional Neural Networks for Sentence Classification.



