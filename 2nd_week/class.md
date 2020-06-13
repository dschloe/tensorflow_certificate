## Exploring how to use data

Machine Learning depends on having good data to train a system with. In this video you saw a scenario for training a system to recognize fashion images. The data comes from a dataset called Fashion MNIST, and you can learn more about it and explore it in GitHub [here](https://github.com/zalandoresearch/fashion-mnist). In the next video, you’ll see how to load that data and prepare it for training.

## The structure of Fashion MNIST data

Here you saw how the data can be loaded into Python data structures that make it easy to train a neural network. You saw how the image is represented as a 28x28 array of greyscales, and how its label is a number. Using a number is a first step in avoiding bias -- instead of labelling it with words in a specific language and excluding people who don’t speak that language! You can learn more about bias and techniques to avoid it [here](https://developers.google.com/machine-learning/fairness-overview/)


## See how it's done

In the next video, Laurence will step you through a workbook where you can see a neural network being trained on Fashion images. After that you’ll be able to try the workbook for yourself!

## Get hands-on with computer vision

Now that you’ve seen the workbook, it’s time to try it for yourself.  You can find it [here](https://colab.sandbox.google.com/github/lmoroney/dlaicourse/blob/master/Course%201%20-%20Part%204%20-%20Lesson%202%20-%20Notebook.ipynb). We’ve also provided a number of exercises you can try at the bottom of the workbook. These will help you poke around and experiment with the code, and will help you with the code you’ll need to write at the end of the week, so it’s really worth spending some time on them! I'd recommend you spend at least 1 hour playing with this workbook. It will be really worth your time!

When you’re done with that, the next thing to do is to explore callbacks, so you can see how to train a neural network until it reaches a threshold you want, and then stop training. You’ll see that in the next video.

## See how to implement Callbacks
Experiment with using Callbacks in this [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/Course%201%20-%20Part%204%20-%20Lesson%204%20-%20Notebook.ipynb) -- work through it to see how they perform!

## Quiz

1. What’s the name of the dataset of Fashion images used in this week’s code?

[ ] Fashion Tensors
[x] Fashion MNIST
[ ] Fashion Data
[ ] Fashion MN

2. What do the above mentioned Images look like?

[x] 28x28 Greyscale
[ ] 28x28 Color
[ ] 82x82 Greyscale
[ ] 100x100 Color

3. How many images are in the Fashion MNIST dataset?

[ ] 60,000
[ ] 10,000
[x] 70,000
[ ] 42

4. Why are there 10 output neurons?

[ ] To make it classify 10x faster
[x] There are 10 different labels
[ ] Purely arbitrary
[ ] To make it train 10x faster

5. What does Relu do?

[ ] For a value x, it returns 1/x
[ ] It only returns x if x is less than zero
[x] It only returns x if x is greater than zero
[ ] It returns the negative of x

6. Why do you split data into training and test sets?

[ ] To make training quicker
[x] To test a network with previously unseen data
[ ] To make testing quicker
[ ] To train a network with previously unseen data

7. What method gets called when an epoch finishes?

[ ] on_end
[ ] On_training_complete
[x] on_epoch_end
[ ] on_epoch_finished

8. What parameter to you set in your fit function to tell it to use callbacks?

[ ] callback=
[ ] oncallback=
[x] callbacks=
[ ] oncallbacks=
