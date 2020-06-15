## Explore an impactful, real-world solution

As Andrew and Laurence discussed, the techniques you’ve learned already can apply to complex images, and you can start solving real scenarios with them. They discussed how it could be used, for example, in disease detection with the Cassava plant, and you can see a video demonstrating that [here](https://www.youtube.com/watch?v=NlpS-DhayQA). Once you’ve watched that, move onto the next lesson!

## Designing the neural network

Now that you’ve seen how an ImageGenerator can flow images from a directory and perform operations such as resizing them on the fly, the next thing to do is design the neural network to handle these more complex images. You’ll see that in the next video.

## Train the ConvNet with ImageGenerator

Now that you’ve designed the neural network to classify Horses or Humans, the next step is to train it from data that’s on the file system, which can be read by generators. To do this, you don’t use model.fit as earlier, but a new method call: model.fit_generator. In the next video you’ll see the details of this.

## Exploring the solution

Now you’ve gone through the code to define the neural network, train it with on-disk images, and then predict values for new images. Let’s see this in action in a workbook. In the next video, Laurence will step you through the workbook, and afterwards, you can try it for yourself!

## Training the neural network

Now that you’ve learned how to download and process the horses and humans dataset, you’re ready to train. When you defined the model, you saw that you were using a new loss function called ‘[Binary Crossentropy](https://gombru.github.io/2018/05/23/cross_entropy_loss/)’, and a new [optimizer](https://www.tensorflow.org/api_docs/python/tf/train/RMSPropOptimizer) called [RMSProp](http://www.cs.toronto.edu/~tijmen/csc321/slides/lecture_slides_lec6.pdf). If you want to learn more about the type of binary classification we are doing here, check out [this](https://www.youtube.com/watch?v=eqEc66RFY0I&t=6s) great video from Andrew!

## Experiment with the horse or human classifier

Now it’s your turn. You can find the notebook [here](https://colab.sandbox.google.com/github/lmoroney/dlaicourse/blob/master/Course%201%20-%20Part%208%20-%20Lesson%202%20-%20Notebook.ipynb). Work through it and get a feel for how the ImageGenerator is pulling the images from the file system and feeding them into the neural network for training. Have some fun with the visualization code at the bottom!

In earlier notebooks you tweaked parameters like epochs, or the number of hidden layers and neurons in them. Give that a try for yourself, and see what the impact is. Spend some time on this.

Once you’re done, move to the next video, where you can validate your training against a lot of images!

## Get hands-on and use validation

Now you can give it a try for yourself. Here’s the notebook the Laurence went through in the video. Have a play with it to see how it trains, and test some images yourself! Once you’re done, move onto the next video where you’ll compact your data to see the impact on training.

## Get Hands-on with compacted images

Try [this](https://colab.sandbox.google.com/github/lmoroney/dlaicourse/blob/master/Course%201%20-%20Part%208%20-%20Lesson%204%20-%20Notebook.ipynb) version of the notebook where Laurence compacted the images. You can see that training times will improve, but that some classifications might be wrong! Experiment with different sizes -- you don’t have to use 150x150 for example!

## Week 4 Quiz

1. Using Image Generator, how do you label images?
[ ] You have to manually do it
[ ] TensorFlow figures it out from the contents
[x] It’s based on the directory the image is contained in
[ ] It’s based on the file name

2. What method on the Image Generator is used to normalize the image?
[ ] normalize
[ ] normalize_image
[ ] Rescale_image
[x] rescale

3. How did we specify the training size for the images?
[x] The target_size parameter on the validation generator
[ ] The training_size parameter on the validation generator
[ ] The training_size parameter on the training generator
[ ] The target_size parameter on the training generator

4. When we specify the input_shape to be (300, 300, 3), what does that mean?
[ ] Every Image will be 300x300 pixels, and there should be 3 Convolutional Layers
[ ] There will be 300 images, each size 300, loaded in batches of 3
[x] Every Image will be 300x300 pixels, with 3 bytes to define color
[ ] There will be 300 horses and 300 humans, loaded in batches of 3

5. If your training data is close to 1.000 accuracy, but your validation data isn’t, what’s the risk here?
[ ] You’re overfitting on your validation data
[ ] You’re underfitting on your validation data
[ ] No risk, that’s a great result
[x] You’re overfitting on your training data

6. Convolutional Neural Networks are better for classifying images like horses and humans because:
[ ] In these images, the features may be in different parts of the frame
[ ] There’s a wide variety of horses
[ ] There’s a wide variety of humans
[x] All of the above

7. After reducing the size of the images, the training results were different. Why?
[ ] There was less information in the images
[x] We removed some convolutions to handle the smaller images
[ ] The training was faster
[ ] There was more condensed information in the images

## Exercise 4 (Handling complex images)

Let’s now create your own image classifier for complex images. See if you can create a classifier for a set of happy or sad images that I’ve provided. Use a callback to cancel training once accuracy is greater than .999.

NOTE: Please do not modify any of the code already provided in the Exercise question, and please only add your additional code in the indicated areas marked by the comments. Once you have completed your notebook assignment and received a final score, please save your notebook, run the final cell, and close your Jupyter Workspace. This will help optimize your Jupyter workspace performance for future assessments. Please note that this step will shut down your kernel, so it is important to save your work in advance of completing this step. 