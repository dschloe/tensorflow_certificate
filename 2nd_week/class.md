## Exploring how to use data

Machine Learning depends on having good data to train a system with. In this video you saw a scenario for training a system to recognize fashion images. The data comes from a dataset called Fashion MNIST, and you can learn more about it and explore it in GitHub [here](https://github.com/zalandoresearch/fashion-mnist). In the next video, you’ll see how to load that data and prepare it for training.

## The structure of Fashion MNIST data

Here you saw how the data can be loaded into Python data structures that make it easy to train a neural network. You saw how the image is represented as a 28x28 array of greyscales, and how its label is a number. Using a number is a first step in avoiding bias -- instead of labelling it with words in a specific language and excluding people who don’t speak that language! You can learn more about bias and techniques to avoid it [here](https://developers.google.com/machine-learning/fairness-overview/)


## See how it's done

In the next video, Laurence will step you through a workbook where you can see a neural network being trained on Fashion images. After that you’ll be able to try the workbook for yourself!

## Get hands-on with computer vision

Now that you’ve seen the workbook, it’s time to try it for yourself.  You can find it [here](https://colab.sandbox.google.com/github/lmoroney/dlaicourse/blob/master/Course%201%20-%20Part%204%20-%20Lesson%202%20-%20Notebook.ipynb). We’ve also provided a number of exercises you can try at the bottom of the workbook. These will help you poke around and experiment with the code, and will help you with the code you’ll need to write at the end of the week, so it’s really worth spending some time on them! I'd recommend you spend at least 1 hour playing with this workbook. It will be really worth your time!

When you’re done with that, the next thing to do is to explore callbacks, so you can see how to train a neural network until it reaches a threshold you want, and then stop training. You’ll see that in the next video.