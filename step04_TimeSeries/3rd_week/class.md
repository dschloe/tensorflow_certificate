## More info on Huber loss
Please find the Wikipedia page [here](https://en.wikipedia.org/wiki/Huber_loss).

## RNN notebook
Please find the link to the notebook [here](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%204%20-%20S%2BP/S%2BP%20Week%203%20Lesson%202%20-%20RNN.ipynb)

## Link to the LSTM lesson
Please find the link to the LSTM lesson [here](https://www.coursera.org/lecture/nlp-sequence-models/long-short-term-memory-lstm-KXoay)

## LSTM notebook
Please find the link to the notebook [here](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%204%20-%20S%2BP/S%2BP%20Week%203%20Lesson%204%20-%20LSTM.ipynb)


## Week 3 Quiz

1. If X is the standard notation for the input to an RNN, what are the standard notations for the outputs?

[ ] Y
[ ] H
[x] Y(hat) and H
[ ] H(hat) and Y

2. What is a sequence to vector if an RNN has 30 cells numbered 0 to 29

[x] The Y(hat) for the last cell
[ ] The total Y(hat) for all cells
[ ] The Y(hat) for the first cell
[ ] The average Y(hat) for all 30 cells

3. What does a Lambda layer in a neural network do?

[ ] Changes the shape of the input or output data
[ ] There are no Lambda layers in a neural network
[ ] Pauses training without a callback
[x] Allows you to execute arbitrary code while training

4. What does the axis parameter of tf.expand_dims do?

[ ] Defines the axis around which to expand the dimensions
[ ] Defines the dimension index to remove when you expand the tensor
[ ] Defines if the tensor is X or Y
[x] Defines the dimension index at which you will expand the shape of the tensor

5. A new loss function was introduced in this module, named after a famous statistician. What is it called?

[x] Huber loss
[ ] Hyatt loss
[ ] Hawking loss
[ ] Hubble loss

6. What’s the primary difference between a simple RNN and an LSTM

[ ] LSTMs have a single output, RNNs have multiple
[ ] LSTMs have multiple outputs, RNNs have a single one
[ ] In addition to the H output, RNNs have a cell state that runs across all cells
[x] In addition to the H output, LSTMs have a cell state that runs across all cells

7. If you want to clear out all temporary variables that tensorflow might have from previous sessions, what code do you run?

[x] tf.keras.clear_session
[ ] tf.cache.backend.clear_session()
[ ] tf.cache.clear_session()
[ ] tf.keras.backend.clear_session() 

8. What happens if you define a neural network with these two layers?

```
tf.keras.layers.Bidirectional(tf.keras.layers.LSTM(32)),
tf.keras.layers.Bidirectional(tf.keras.layers.LSTM(32)),
tf.keras.layers.Dense(1),
```

[ ] Your model will compile and run correctly
[ ] Your model will fail because you have the same number of cells in each LSTM
[x] Your model will fail because you need return_sequences=True after the first LSTM layer
[ ] Your model will fail because you need return_sequences=True after each LSTM layer

## Week 3 Wrap up
Now that you've built on your DNNs with RNNs and LSTMs, it's time to put it all together using CNNs and some real world data.

Next week you'll do that, exploring prediction of sunspot data from a couple of hundred years worth of measurements!