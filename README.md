# ImageCaptioning
Automatic Image Captioning using CNN(resnet50) and RNN(LSTM)
- Image Captioning[Computer Vision + NLP]
## What is Image Captioning ?
Image Captioning is the process of generating textual description of an image. It uses both Natural Language Processing and Computer Vision to generate the captions. This task lies at the intersection of computer vision and natural language processing. Most image captioning systems use an encoder-decoder framework, where an input image is encoded into an intermediate representation of the information in the image, and then decoded into a descriptive text sequence.

CNNs + RNNs (LSTMs)
To perform Image Captioning we will require two deep learning models combined into one for the training purpose

- CNNs extract the features from the image of some vector size aka the vector embeddings. The size of these embeddings depend on the type of pretrained network being used for the feature extraction

- LSTMs are used for the text generation process. The image embeddings are concatenated with the word embeddings and passed to the LSTM to generate the next word For a more illustrative explanation of this architecture check the Modelling section for a picture representation
- 
### I am using Flickr8K [image-caption] dataset from kaggle which consisits of 8000+ images. with 5 captions for each images
We have taken less image dataset so we will be using Transfer Learning techniques with pretrained model like CNNS(Resnet50) which is trained in 'Imagenet',RNNS(LSTM) for text processing and generating

# Transfer learning is a technique that can be used to improve the performance of a machine learning model when there is a limited amount of training data available. The idea behind transfer learning is to use a pre-trained model that has been trained on a large dataset of images, such as ImageNet, and then fine-tune the model on the smaller dataset.


1. Import all the Required Packages
2. Perform Data Cleaning
3. Extract the Feature Vector
4. Loading dataset for model training
5. Tokenizing the Vocabulary
6. Create a Data generator
7. Define the CNN-RNN model
8. Training the Image Caption Generator model
9. Testing the Image Caption Generator model
