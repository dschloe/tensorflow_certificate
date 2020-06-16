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

Now that we’ve discussed what it’s like to extend to real-world data using the Cats v Dogs dataset from an old Kaggle Data Science challenge, let’s go into a [notebook]() that shows how to do the challenge for yourself! In the next video, you’ll see a screencast of that notebook in action. You’ll then be able to try it for yourself.


