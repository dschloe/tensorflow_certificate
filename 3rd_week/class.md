## Coding convolutions and pooling layers

The concepts introduced in this video are available as [Conv2D](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Conv2D) layers and [MaxPooling2D](https://www.tensorflow.org/api_docs/python/tf/keras/layers/MaxPool2D) layers in TensorFlow. You’ll learn how to implement them in code in the next video. 

## Learn more about convolutions

You’ve seen how to add a convolutional 2d layer to the top of your neural network in the previous video. If you want to see more detail on how they worked, check out the playlist at https://bit.ly/2UGa7uH.

Now let’s take a look at adding the pooling, and finishing off the convolutions so you can try them out. 

## Getting hands-on, your first ConvNet

You’ve now seen how to turn your Deep Neural Network into a Convolutional Neural Network by adding convolutional layers on top, and having the network train against the results of the convolutions instead of the raw pixels. In the next video, you’ll step through a workbook to see how this works. 

## Try it for yourself

[Here’s](https://colab.sandbox.google.com/github/lmoroney/dlaicourse/blob/master/Course%201%20-%20Part%206%20-%20Lesson%202%20-%20Notebook.ipynb) the notebook that Laurence was using in that screencast. To make it work quicker, go to the ‘Runtime’ menu, and select ‘Change runtime type’. Then select GPU as the hardware accelerator!

Work through it, and try some of the exercises at the bottom! It's really worth spending a bit of time on these because, as before, they'll really help you by seeing the impact of small changes to various parameters in the code. You should spend at least 1 hour on this today!

Once you’re done, go onto the next video and take a look at some code to build a convolution yourself to visualize how it works!

## Experiment with filters and pools

To try this notebook for yourself, and play with some convolutions, [here’s the notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/Course%201%20-%20Part%206%20-%20Lesson%203%20-%20Notebook.ipynb). Let us know if you come up with any interesting filters of your own!

As before, spend a little time playing with this notebook. Try different filters, and research different filter types. There's some fun information about them here: https://lodev.org/cgtutor/filtering.html

## Week 3 Quiz
1. What is a Convolution?
[ ] A technique to make images smaller 
[ ] ] A technique to make images bigger 
[ ] A technique to filter out unwanted images 
[x] A technique to isolate features in images

2. What is a Pooling?
[ ] A technique to make images sharper
[ ] A technique to combine pictures
[x] A technique to reduce the information in an image while maintaining features
[ ] A technique to isolate features in images

3. How do Convolutions improve image recognition?
[ ] They make processing of images faster
[ ] They make the image smaller
[ ] They make the image clearer
[x] They isolate features in images

4. After passing a 3x3 filter over a 28x28 image, how big will the output be? (정답)

[x] 26x26
[ ] 31x31
[ ] 28x28
[ ] 25x25

5. After max pooling a 26x26 image with a 2x2 filter, how big will the output be? (정답)

[ ] 26x26
[x] 13x13
[ ] 28x28
[ ] 56x56

6. Applying Convolutions on top of our Deep neural network will make training:

[x] It depends on many factors. It might make your training faster or slower, and a poorly designed Convolutional layer may even be less efficient than a plain DNN!
[ ] Faster
[ ] Slower
[ ] Stay the same

## Exercise 3 (Improve MNIST with convolutions)

Ok, now it’s time for this week’s assignment. In the class you learned how to enhance the Fashion MNIST neural network with Convolutions to make it more accurate. Now it’s time to revisit the handwriting MNIST dataset from last week, and see if you can enhance it with Convolutions.

NOTE: Please do not modify any of the code already provided in the Exercise question, and please only add your additional code in the indicated areas marked by the comments. Once you have completed your notebook assignment and received a final score, please save your notebook, run the final cell, and close your Jupyter Workspace. This will help optimize your Jupyter workspace performance for future assessments. Please note that this step will shut down your kernel, so it is important to save your work in advance of completing this step

[노트열기](https://vlxjaasiiaklrpalrbmicg.coursera-apps.org/notebooks/week3/Excercise-3-Question.ipynb)