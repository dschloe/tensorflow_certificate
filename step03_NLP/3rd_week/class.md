## Link to Andrew's sequence modeling course

Here is the [link](https://www.coursera.org/lecture/nlp-sequence-models/deep-rnns-ehs0S) to Andrew's course on sequence modeling.

## More info on LSTMs

Please find here a [link](https://www.coursera.org/lecture/nlp-sequence-models/long-short-term-memory-lstm-KXoay) to more information on LSTMs (Long Short Term Memory cells) by Andrew.

## Check out the code!
We've created a number of notebooks for you to explore the different types of sequence models.

Spend some time going through these to see how they work, and what the impact of different layer types have on training for classification.

[IMDB Subwords 8K with Single Layer LSTM](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%203%20-%20Lesson%201a.ipynb)

[IMDB Subwords 8K with Multi Layer LSTM](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%203%20-%20Lesson%201b.ipynb)


## Check out the code!
Spend some time going through this notebook to see how it works.

[IMDB Subwords 8K with 1D Convolutional Layer](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%203%20-%20Lesson%201c.ipynb)

## Check out the code!
Spend some time going through this notebook to see how it works and what the impact of different layer types have on training for classification.

[IMDB Reviews with GRU (and optional LSTM and Conv1D)](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%203%20-%20Lesson%202d.ipynb#scrollTo=nHGYuU4jPYaj)

## Exploring different sequence models
We've created a number of notebooks for you to explore the different types of sequence model.

Spend some time going through these to see how they work, and what the impact of different layer types have on training for classification.

[Sarcasm with Bidirectional LSTM](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%203%20-%20Lesson%202.ipynb#scrollTo=g9DC6dmLF8DC)

[Sarcasm with 1D Convolutional Layer](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%203%20-%20Lesson%202c.ipynb#scrollTo=g9DC6dmLF8DC)

## Quiz

1. Why does sequence make a large difference when determining semantics of language? correct

[ ] Because the order in which words appear dictate their meaning
[ ] It doesn’t
[x] Because the order in which words appear dictate their impact on the meaning of the sentence
[ ] Because the order of words doesn’t matter

2. How do Recurrent Neural Networks help you understand the impact of sequence on meaning?

[ ] They look at the whole sentence at a time
[x] They carry meaning from one cell to the next
[ ] They shuffle the words evenly
[ ] They don’t

3. How does an LSTM help understand meaning when words that qualify each other aren’t necessarily beside each other in a sentence? correct
 
[ ] They don’t
[ ] They shuffle the words randomly
[x] Values from earlier words can be carried to later ones via a cell state
[ ] They load all words into a cell state

4. What keras layer type allows LSTMs to look forward and backward in a sentence? correct

[ ] Bilateral
[x] Bidirectional
[ ] Bothdirection
[ ] Unilateral

5. What’s the output shape of a bidirectional LSTM layer with 64 units?

[x] (None, 128)
[ ] (None, 64)
[ ] (128,None)
[ ] (128,1)

6. When stacking LSTMs, how do you instruct an LSTM to feed the next one in the sequence?

[x] Ensure that return_sequences is set to True only on units that feed to another LSTM
[ ] Ensure that return_sequences is set to True on all units
[ ] Do nothing, TensorFlow handles this automatically
[ ] Ensure that they have the same number of units

7. If a sentence has 120 tokens in it, and a Conv1D with 128 filters with a Kernal size of 5 is passed over it, what’s the output shape?

[ ] (None, 120, 124)
[x] (None, 116, 128)
[ ] (None, 116, 124)
[ ] (None, 120, 128)

8. What’s the best way to avoid overfitting in NLP datasets?

[ ] Use LSTMs
[ ] Use GRUs
[ ] Use Conv1D
[x] None of the above

## Week 3 Wrap up
You’ve been experimenting with NLP for text classification over the last few weeks. Next week you’ll switch gears -- and take a look at using the tools that you’ve learned to predict text, which ultimately means you can create text. By learning sequences of words you can predict the most common word that comes next in the sequence, and thus, when starting from a new sequence of words you can create a model that builds on them. You’ll take different training sets -- like traditional Irish songs, or Shakespeare poetry, and learn how to create new sets of words using their embeddings!


