## Introducing the Rock-Paper-Scissors dataset

http://www.laurencemoroney.com/rock-paper-scissors-dataset/

Rock Paper Scissors is a dataset containing 2,892 images of diverse hands in Rock/Paper/Scissors poses. It is licensed [CC By 2.0](https://creativecommons.org/licenses/by/2.0/) and available for all purposes, but it’s intent is primarily for learning and research.

Rock Paper Scissors contains images from a variety of different hands,  from different races, ages and genders, posed into Rock / Paper or Scissors and labelled as such. You can download the [training set here](https://storage.googleapis.com/laurencemoroney-blog.appspot.com/rps.zip), and the [test set here](https://storage.googleapis.com/laurencemoroney-blog.appspot.com/rps-test-set.zip). These images have all been generated using CGI techniques as an experiment in determining if a CGI-based dataset can be used for classification against real images. I also generated a few images that you can use for predictions. You can find them [here](https://storage.googleapis.com/laurencemoroney-blog.appspot.com/rps-validation.zip).

Note that all of this data is posed against a white background.
Each image is 300×300 pixels in 24-bit color
You'll see how this dataset can be used to build a multi-class classifier in the next video

## Check out the code!

Now that you've explored the data, and seen how the code can be modified from a binary class classifier to a multi class one, let's take a look at the [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/Course%202%20-%20Part%208%20-%20Lesson%202%20-%20Notebook%20(RockPaperScissors).ipynb) that implements that for us!

## Try testing the classifier

In the following video you'll see me testing the classifier myself. You should also try it out using the data that you can find [here](https://storage.googleapis.com/laurencemoroney-blog.appspot.com/rps-validation.zip).


## What have we seen so far?
You're coming to the end of Course 2, and you've come a long way! From first principles in understanding how ML works, to using a DNN to do basic computer vision, and then beyond into Convolutions.

With Convolutions, you then saw how to extract features from an image, and you saw the tools in TensorFlow and Keras to build with Convolutions and Pooling as well as handling complex, multi-sized images.

Through this you saw how overfitting can have an impact on your classifiers, and explored some strategies to avoid it, including Image Augmentation, Dropouts, Transfer Learning and more. To wrap things up, this week you've looked at the considerations in your code that you need for moving towards multi-class classification!

## Week 4 Quiz

1. The diagram for traditional programming had Rules and Data In, but what came out?

[x] Answers
[ ] Binary
[ ] Machine Learning
[ ] Bugs

2. Why does the DNN for Fashion MNIST have 10 output neurons?

[ ] To make it train 10x faster
[ ] To make it classify 10x faster
[ ] Purely Arbitrary
[x] The dataset has 10 classes

3. What is a Convolution?

[ ] A technique to make images smaller
[ ] A technique to make images larger
[x] A technique to extract features from an image
[ ] A technique to remove unwanted images

4. Applying Convolutions on top of a DNN will have what impact on training?

[ ] It will be slower
[ ] It will be faster
[ ] There will be no impact
[x] It depends on many factors. It might make your training faster or slower, and a poorly designed Convolutional layer may even be less efficient than a plain DNN!

5. What method on an ImageGenerator is used to normalize the image?

[ ] normalize
[ ] flatten
[ ] rezize()
[x] rescale

6. When using Image Augmentation with the ImageDataGenerator, what happens to your raw image data on-disk.

[ ] A copy will be made, and the copies are augmented
[ ] A copy will be made, and the originals will be augmented
[x] Nothing
[ ] The images will be edited on disk, so be sure to have a backup

7. Can you use Image augmentation with Transfer Learning?

[ ] No - because the layers are frozen so they can't be augmented
[x] Yes. It's pre-trained layers that are frozen. So you can augment your images as you train the bottom layers of the DNN with them

8. When training for multiple classes what is the Class Mode for Image Augmentation?

[ ] class_mode='multiple'
[ ] class_mode='non_binary'
[x] class_mode='categorical'
[ ] class_mode='all'

