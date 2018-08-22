# Printed Chinese Character OCR 
Text recognition is a very important research direction of computer vision, and it is a very effective way to improve the efficiency of information input, and it has high universality.This paper studies the recognition of Chinese and alphanumeric characters based on deep learning, and constructs character recognition system for identity card scene.First, this paper mainly uses the PIL and opencv library underneath the Python generates training set and test set, including 6509 kind of Chinese characters and 61 alphanumeric, and adding random noise, random changes in font size, random Angle rotation, stretching distortion, the commonly used methods such as add a gaussian blur to generate images, reach the purpose of data augmentation as well as the training data set wide distribution.
Secondly, this paper mainly uses the VGG16 network structure to build the recognition model under the keras deep learning framework of the TensorFlow backend.Compared to the model of this building standard VGG16 network structure, reduce the number of input image size and channel, reduced the number of convolution and pooling layer, increase the batch norm layer, increased the number all connection layer neurons, have good learning speed and convergence characteristics, under the Chinese characters of test set with 95% accuracy, alphanumeric character set of test accuracy as high as 99%.
Finally, because of the neural network for character recognition input is 64 * 64 size of the gray-scale images, so the input the id card photo to filter out background, cutting, preprocessing operations such as plastic.This paper mainly uses projection method to cut images.Then cut pretreatment combined with neural network system, to form the input id photos back to text information end-to-end system, text information can be combined with the server database, real-time inputting relevant information quickly and improve production efficiency.

# this is a Chinese character ocr system based on deep learning neural network.this rep include image preprcessing(character segmentation),trainning set generating and augmentation,model(based on vgg16,use keras high level neural network framwork)and model optimize func.

