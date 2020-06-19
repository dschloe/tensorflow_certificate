## Convolutional neural networks course
More information on CNNs can be found on Andrews course within the Deep Learning Specialization.
If you are curious about the content and would like to learn more, here is the [link](https://www.coursera.org/learn/convolutional-neural-networks/home/welcome) to the course.

## More on batch sizing
Please find more information [here](https://www.youtube.com/watch?v=4qJaSmvhxi8)

## LSTM notebook
Please find the link to the notebook [here](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%204%20-%20S%2BP/S%2BP%20Week%204%20Lesson%201.ipynb)

## Sunspots notebook
Please find the link to the [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%204%20-%20S%2BP/S%2BP%20Week%204%20Lesson%205.ipynb) here
For fun, there's also a version of the notebook that uses only DNN [here](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%204%20-%20S%2BP/S%2BP%20Week%204%20Lesson%203.ipynb).

## Week 4 Quiz

1. How do you add a 1 dimensional convolution to your model for predicting time series data?

[x] Use a Conv1D layer type
[ ] Use a 1DConv layer type
[ ] Use a 1DConvolution layer type
[ ] Use a Convolution1D layer type

2. What’s the input shape for a univariate time series to a Conv1D? incorrect 

[ ] [1]
[ ] []
[x] [None, 1]
[ ] [1, None]

3. You used a sunspots dataset that was stored in CSV. What’s the name of the Python library used to read CSVs?

[ ] PyFiles
[ ] PyCSV
[ ] CommaSeparatedValues
[x] CSV

4. If your CSV file has a header that you don’t want to read into your dataset, what do you execute before iterating through the file using a ‘reader’ object? incorrect

[x] next(reader)
[ ] reader.next
[ ] reader.ignore_header()
[ ] reader.read(next)

5. When you read a row from a reader and want to cast column 2 to another data type, for example, a float, what’s the correct syntax? incorrect

[ ] float f = row[2].read()
[ ] You can’t. It needs to be read into a buffer and a new float instantiated from the buffer
[x] float(row[2])
[ ] Convert.toFloat(row[2])

6. What was the sunspot seasonality?

[ ] 11 years
[ ] 22 years
[ ] 4 times a year
[x] 11 or 22 years depending on who you ask

7. After studying this course, what neural network type do you think is best for predicting time series like our sunspots dataset?

[x] A combination of all of the above
[ ] RNN / LSTM
[ ] DNN
[ ] Convolutions

8. Why is MAE a good analytic for measuring accuracy of predictions for time series?

[ ] It only counts positive errors
[ ] It punishes larger errors
[ ] It biases towards small errors
[x] It doesn’t heavily punish larger errors like square errors do

## Wrap up
Congratulations on getting this far! In this course you've dipped your toe into the water of understanding sequences and some of the tools for predicting them! Hopefully it was a fun journey and we're really looking forward to what you build next! :)