## Image Augmentation

You'll be looking a lot at Image Augmentation this week.

Image Augmentation is a very simple, but very powerful tool to help you avoid overfitting your data. The concept is very simple though: If you have limited data, then the chances of you having data to match potential future predictions is also limited, and logically, the less data you have, the less chance you have of getting accurate predictions for data that your model hasn't yet seen. To put it simply, if you are training a model to spot cats, and your model has never seen what a cat looks like when lying down, it might not recognize that in future.

Augmentation simply amends your images on-the-fly while training using transforms like rotation. So, it could 'simulate' an image of a cat lying down by rotating a 'standing' cat by 90 degrees. As such you get a cheap way of extending your dataset beyond what you have already.

To learn more about Augmentation, and the available transforms, check out https://github.com/keras-team/keras-preprocessing -- and note that it's referred to as preprocessing for a very powerful reason: that it doesn't require you to edit your raw images, nor does it amend them for you on-disk. It does it in-memory as it's performing the training, allowing you to experiment without impacting your dataset.

## Start Coding...

Ok, now that we've looked at Image Augmentation implementation in Keras, let's dig down into the code.
You can see more about the different APIs at the Keras site here: https://keras.io/preprocessing/image/

## Looking at the notebook

Now that you've gotten to learn some of the basics of Augmentation, let's look at it in action in the Cats v Dogs classifier.
First, we'll run Cats v Dogs without Augmentation, and explore how quickly it overfits.

If you want to run the notebook yourself, you can find it here: https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/Course%202%20-%20Part%204%20-%20Lesson%202%20-%20Notebook%20(Cats%20v%20Dogs%20Augmentation).ipynb

## The impact of augmentation on Cats vs. Dogs

Now that we’ve seen it overfitting, let’s next look at how, with a simple code modification, we can add Augmentation to the same Convolutional Neural Network to see how it gives us better training data that overfits less!


## Try it for yourself!

Having clearly seen the impact that augmentation gives to Cats v Dogs, let’s now go back to the Horses v Humans dataset from Course 1, and take a look to see if the augmentation algorithms will help there! Here’s the [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/Course%202%20-%20Part%204%20-%20Lesson%204%20-%20Notebook.ipynb) if you want to try it for yourself!

## What have we seen so far?

This week you looked at the really useful tool that TensorFlow gives you with Image Augmentation. With it, you can effectively simulate a larger dataset from a smaller one with tools to move images around the frame, skew them, rotate them, and more. It can be an effective tool in fixing overfitting. Hopefully you found it useful!


## Quiz 

1. How do you use Image Augmentation in TensorFLow

[ ] With the tf.augment API
[ ] With the keras.augment API
[ ] You have to write a plugin to extend tf.layers
[x] Using parameters to the ImageDataGenerator

2. If my training data only has people facing left, but I want to classify people facing right, how would I avoid overfitting? (correct)

[ ] Use the ‘flip_vertical’ parameter around the Y axis
[ ] Use the ‘flip’ parameter and set ‘horizontal’
[x] Use the ‘horizontal_flip’ parameter
[ ] Use the ‘flip’ parameter

3. When training with augmentation, you noticed that the training is a little slower. Why?

[ ] Because the augmented data is bigger
[ ] Because the training is making more mistakes
[x] Because the image processing takes cycles
[ ] Because there is more data to train on

4. What does the fill_mode parameter do?

[ ] There is no fill_mode parameter
[ ] It creates random noise in the image
[x] It attempts to recreate lost information after a transformation like a shear
[ ] It masks the background of an image

5. When using Image Augmentation with the ImageDataGenerator, what happens to your raw image data on-disk.

[ ] It gets overwritten, so be sure to make a backup
[ ] A copy is made and the augmentation is done on the copy
[x] Nothing, all augmentation is done in-memory
[ ] It gets deleted

6. How does Image Augmentation help solve overfitting? (correct)

[ ] It slows down the training process
[x] It manipulates the training set to generate more scenarios for features in the images
[ ] It manipulates the validation set to generate more scenarios for features in the images
[ ] It automatically fits features to images by finding them through image processing techniques

7. When using Image Augmentation my training gets... (correct)

[x] Slower
[ ] Faster
[ ] Stays the Same
[ ] Much Faster

8. Using Image Augmentation effectively simulates having a larger data set for training.

[ ] False
[x] True


