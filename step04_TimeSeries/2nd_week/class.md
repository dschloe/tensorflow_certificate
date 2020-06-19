## Preparing features and labels notebook
Please find the link to the notebook [here](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%204%20-%20S%2BP/S%2BP%20Week%202%20Lesson%201.ipynb)

## Sequence bias
Sequence bias is when the order of things can impact the selection of things. For example, if I were to ask you your favorite TV show, and listed "Game of Thrones", "Killing Eve", "Travellers" and "Doctor Who" in that order, you're probably more likely to select 'Game of Thrones' as you are familiar with it, and it's the first thing you see. Even if it is equal to the other TV shows. So, when training data in a dataset, we don't want the sequence to impact the training in a similar way, so it's good to shuffle them up.

## Single layer neural network notebook
Please find the link to the notebook [here](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%204%20-%20S%2BP/S%2BP%20Week%202%20Lesson%202.ipynb)

## Deep neural network notebook
Please find the link to the notebook [here](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%204%20-%20S%2BP/S%2BP%20Week%202%20Lesson%203.ipynb)

## Week 2 Quiz

1. What is a windowed dataset?

[ ] There’s no such thing
[x] A fixed-size subset of a time series
[ ] The time series aligned to a fixed shape
[ ] A consistent set of subsets of a time series

2. What does ‘drop_remainder=true’ do? incorrect 

[x] It ensures that all rows in the data window are the same length by cropping data
[ ] It ensures that all rows in the data window are the same length by adding data
[ ] It ensures that the data is all the same shape
[ ] It ensures that all data is used

3. What’s the correct line of code to split an n column window into n-1 columns for features and 1 column for a label

[ ] dataset = dataset.map(lambda window: (window[n-1], window[1]))
[x] dataset = dataset.map(lambda window: (window[:-1], window[-1:]))
[ ] dataset = dataset.map(lambda window: (window[-1:], window[:-1]))
[ ] dataset = dataset.map(lambda window: (window[n], window[1]))

4. What does MSE stand for?

[ ] Mean Second error
[x] Mean Squared error
[ ] Mean Slight error
[ ] Mean Series error

5. What does MAE stand for?

[ ] Mean Average Error
[ ] Mean Advanced Error
[x] Mean Absolute Error
Mean Active Error

6. If time values are in time[], series values are in series[] and we want to split the series into training and validation at time 1000, what is the correct code?

time_train = time[split_time]
x_train = series[split_time]
time_valid = time[split_time]
x_valid = series[split_time]


time_train = time[:split_time]
x_train = series[:split_time]
time_valid = time[split_time]
x_valid = series[split_time]


time_train = time[:split_time]
x_train = series[:split_time]
time_valid = time[split_time:]
x_valid = series[split_time:]


time_train = time[split_time]
x_train = series[split_time]
time_valid = time[split_time:]
x_valid = series[split_time:]

7. If you want to inspect the learned parameters in a layer after training, what’s a good technique to use?

[ ] Iterate through the layers dataset of the model to find the layer you want
[x] Assign a variable to the layer and add it to the model using that variable. Inspect its properties after training
[ ] Run the model with unit data and inspect the output for that layer
[ ] Decompile the model and inspect the parameter set for that layer

8. How do you set the learning rate of the SGD optimizer? 

[ ] You can’t set it
[x] Use the lr property
[ ] Use the Rate property 
[ ] Use the RateOfLearning property

9. If you want to amend the learning rate of the optimizer on the fly, after each epoch, what do you do?

[ ] Use a LearningRateScheduler and pass it as a parameter to a callback
[ ] Callback to a custom function and change the SGD property
[x] Use a LearningRateScheduler object in the callbacks namespace and assign that to the callback
[ ] You can’t set it

## Week 2 Wrap up
You've now explored time series data, and seen how to split it into training and validation sets for training a DNN.

But sequence data tends to work better with RNNs, so next week you're going to look at training a model using RNNs and LSTMs on this data to see what happens!

