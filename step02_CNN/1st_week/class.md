## Before you Begin: Tensorflow 2.0 and this Course

We've gotten a lot of questions about whether this course teaches TensorFlow 2.0 or 1.x.

The answer is: Both!

We've designed the curriculum for the early modules in this course to have code that's generic enough that it works with both versions, so you are welcome to try it with the 2.0 alpha. If you are using the colabs, you'll use the latest version of TensorFlow that Google Colaboratory supports, which, at time of writing is 1.13. You can replace this with 2.0 by adding a codeblock containing:

```python
!pip install tensorflow==2.0.0-alpha0 
```

...and you should be able to use TF2.0 alpha if you like!

Later modules may use specific versions of libraries, some of which may require TF2.0, and we will note them when you get there!

## The cats vs dogs dataset

In the next video, you'll look at the famous Kaggle Dogs v Cats dataset: https://www.kaggle.com/c/dogs-vs-cats

This was originally a challenge in building a classifier aimed at the world's best Machine Learning and AI Practitioners, but the technology has advanced so quickly, you'll see how you can do it in just a few minutes with some simple Convolutional Neural Network programming.

It's also a nice exercise in looking at a larger dataset, downloading and preparing it for training, as well as handling some preprocessing of data. Even data like this which has been carefully curated for you can have errors -- as you'll notice with some corrupt images!

Also, you may notice some warnings about missing or corrupt EXIF data as the images are being loaded into the model for training. Don't worry about this -- it won't impact your model! :)

## Looking at the notebook

Now that we’ve discussed what it’s like to extend to real-world data using the Cats v Dogs dataset from an old Kaggle Data Science challenge, let’s go into a [notebook](https://colab.sandbox.google.com/github/lmoroney/dlaicourse/blob/master/Course%202%20-%20Part%202%20-%20Lesson%202%20-%20Notebook.ipynb) that shows how to do the challenge for yourself! In the next video, you’ll see a screencast of that notebook in action. You’ll then be able to try it for yourself.

## What you'll see next

In the last video you saw a screencast of the [notebook]() that you can use as an example of how to build a classifier for Cats vs Dogs. You saw how, in some cases it didn’t classify one cat correctly, and we asked you to try to figure out how you might fix it for yourself. In the next video, you’ll see one solution to this. 

## What have we seen so far?

At the end of the last video you saw how to explore the training history and discovered an interesting phenomenon: Even though the training data set’s accuracy went very high, we saw that after only a few epochs, the validation set levelled out. This is a clear sign that we are overfitting again. Using more data should help with this, but there are some other techniques that you can use with smaller data sets too. And we’ll see them in next week’s lesson!

## Week 1 Quiz

1. What does flow_from_directory give you on the ImageGenerator?

[ ] The ability to easily load images for training
[ ] The ability to pick the size of training images
[ ] The ability to automatically label images based on their directory name
[x] All of the above

2. If my Image is sized 150x150, and I pass a 3x3 Convolution over it, what size is the resulting image?

[ ] 153x153
[ ] 150x150
[x] 148x148
[ ] 450x450

3. If my data is sized 150x150, and I use Pooling of size 2x2, what size will the resulting image be?

[ ] 149x149
[ ] 300x300
[ ] 148x148
[x] 75x75

4. If I want to view the history of my training, how can I access it?

[ ] Use a model.fit_generator
[ ] Pass the parameter ‘history=true’ to the model.fit
[x] Create a variable ‘history’ and assign it to the return of model.fit or model.fit_generator
[ ] Download the model and inspect it

5. What’s the name of the API that allows you to inspect the impact of convolutions on the images?

[x] The model.layers API
[ ] The model.pools API
[ ] The model.images API
[ ] The model.convolutions API

6. When exploring the graphs, the loss levelled out at about .75 after 2 epochs, but the accuracy climbed close to 1.0 after 15 epochs. What's the significance of this?

[ ] There was no point training after 2 epochs, as we overfit to the validation data
[x] There was no point training after 2 epochs, as we overfit to the training data
[ ] A bigger training set would give us better validation accuracy
[ ] A bigger validation set would give us better training accuracy

7. Why is the validation accuracy a better indicator of model performance than training accuracy?

[ ] It isn't, they're equally valuable
[ ] There's no relationship between them
[x] The validation accuracy is based on images that the model hasn't been trained with, and thus a better indicator of how the model will perform with new images.
[ ] The validation dataset is smaller, and thus less accurate at measuring accuracy, so its performance isn't as important

8. Why is overfitting more likely to occur on smaller datasets?

[ ] Because in a smaller dataset, your validation data is more likely to look like your training data
[ ] Because there isn't enough data to activate all the convolutions or neurons
[ ] Because with less data, the training will take place more quickly, and some features may be missed
[x] Because there's less likelihood of all possible features being encountered in the training process.