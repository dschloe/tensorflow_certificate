## Start coding!

Now that we've seen the concepts behind transfer learning, let's dig in and take a look at how to do it for ourselves with TensorFlow and Keras.

In the next few videos you'll be using this notebook to explore transfer learning: https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/Course%202%20-%20Part%206%20-%20Lesson%203%20-%20Notebook.ipynb

For more on how to freeze/lock layers, explore the documentation, which includes an example using MobileNet architecture: https://www.tensorflow.org/tutorials/images/transfer_learning

## Adding your DNN

In the previous video you saw how to take the layers from an existing model, and make them so that they don't get retrained -- i.e. you freeze (or lock) the already learned convolutions into your model. Now, you'll need to add your own DNN at the bottom of these, which you can retrain to your data. In the next video you'll see how to do that...

## Using dropouts!

Another useful tool to explore at this point is the Dropout.

The idea behind Dropouts is that they remove a random number of neurons in your neural network. This works very well for two reasons: The first is that neighboring neurons often end up with similar weights, which can lead to overfitting, so dropping some out at random can remove this. The second is that often a neuron can over-weigh the input from a neuron in the previous layer, and can over specialize as a result. Thus, dropping out can break the neural network out of this potential bad habit!

Check out Andrew's terrific video explaining dropouts here: https://www.youtube.com/watch?v=ARq74QuavAo

## Applying Transfer Learning to Cats v Dogs

Now that we've explored transfer learning, and taken a look at regularization using dropouts, let's step through the scenario for Cats vs Dogs in this [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/Course%202%20-%20Part%206%20-%20Lesson%203%20-%20Notebook.ipynb) next.


## What have we seen so far?

This week you've learned a lot of great new concepts!

You saw Transfer Learning, and how you can take an existing model, freeze many of its layers to prevent them being retrained, and effectively 'remember' the convolutions it was trained on to fit images.

You then added your own DNN underneath this so that you could retrain on your images using the convolutions from the other model.

You learned about regularization using dropouts to make your network more efficient in preventing over-specialization and this overfitting.

Before you get to the exercise for this week, let's have a quick quiz!

## Quiz 

1. If I put a dropout parameter of 0.2, how many nodes will I lose?

[x] 20% of them
[ ] 2% of them
[ ] 20% of the untrained ones
[ ] 2% of the untrained ones

2. Why is transfer learning useful?

[ ] Because I can use all of the data from the original training set
[ ] Because I can use all of the data from the original validation set
[x] Because I can use the features that were learned from large datasets that I may not have access to
[ ] Because I can use the validation metadata from large datasets that I may not have access to

3. How did you lock or freeze a layer from retraining?

[ ] tf.freeze(layer)
[ ] tf.layer.frozen = true
[ ] tf.layer.locked = true
[x] layer.trainable = false

4. How do you change the number of classes the model can classify when using transfer learning? (i.e. the original model handled 1000 classes, but yours handles just 2)

[ ] Ignore all the classes above yours (i.e. Numbers 2 onwards if I'm just classing 2)
[ ] Use all classes but set their weights to 0
[x] When you add your DNN at the bottom of the network, you specify your output layer with the number of classes you want
[ ] Use dropouts to eliminate the unwanted classes

5. Can you use Image Augmentation with Transfer Learning Models?

[ ] No, because you are using pre-set features
[x] Yes, because you are adding new layers at the bottom of the network, and you can use image augmentation when training these

6. Why do dropouts help avoid overfitting?

[x] Because neighbor neurons can have similar weights, and thus can skew the final training
[ ] Having less neurons speeds up training

7. What would the symptom of a Dropout rate being set too high?

[x] The network would lose specialization to the effect that it would be inefficient or ineffective at learning, driving accuracy down
[ ] Training time would increase due to the extra calculations being required for higher dropout

8. Which is the correct line of code for adding Dropout of 20% of neurons using TensorFlow

[ ] tf.keras.layers.Dropout(20)
[ ] tf.keras.layers.DropoutNeurons(20),
[x] tf.keras.layers.Dropout(0.2),
[ ] tf.keras.layers.DropoutNeurons(0.2),

