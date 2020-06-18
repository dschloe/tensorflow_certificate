## Check out the code!
Let's take a look at the first [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%204%20-%20Lesson%201%20-%20Notebook.ipynb) for this week.

## link to Laurence's poetry
Please find the link to Laurences generated poetry [here](https://storage.googleapis.com/laurencemoroney-blog.appspot.com/irish-lyrics-eof.txt).

## Check out the code!
Let's take a look at the second [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%204%20-%20Lesson%202%20-%20Notebook.ipynb) for this week.


## Text generation with an RNN
Tutorials: https://www.tensorflow.org/tutorials/text/text_generation

## Link to generating text using a character-based RNN
Find the link to generating text using a character-based RNN [here](https://www.tensorflow.org/tutorials/sequences/text_generation).

## Quiz

1. What is the name of the method used to tokenize a list of sentences?

[ ] tokenize(sentences)
[ ] fit_to_text(sentences)
[ ] tokenize_on_text(sentences)
[x] fit_on_texts(sentences)

2. If a sentence has 120 tokens in it, and a Conv1D with 128 filters with a Kernal size of 5 is passed over it, what’s the output shape?

[ ] (None, 120, 124)
[ ] (None, 120, 128)
[x] (None, 116, 128)
[ ] (None, 116, 124)

3. What is the purpose of the embedding dimension?

[ ] It is the number of words to encode in the embedding
[ ] It is the number of letters in the word, denoting the size of the encoding
[x] It is the number of dimensions for the vector representing the word encoding
[ ] It is the number of dimensions required to encode every word in the corpus

4. IMDB Reviews are either positive or negative. What type of loss function should be used in this scenario?

[ ] Categorical crossentropy
[ ] Binary Gradient descent
[ ] Adam
[x] Binary crossentropy

5. If you have a number of sequences of different lengths, how do you ensure that they are understood when fed into a neural network?

[ ] Specify the input layer of the Neural Network to expect different sizes with dynamic_length
[ ] Process them on the input layer of the Neural Network using the pad_sequences property
[ ] Make sure that they are all the same length using the pad_sequences method of the tokenizer
[x] Use the pad_sequences object from the tensorflow.keras.preprocessing.sequence namespace

6. When predicting words to generate poetry, the more words predicted the more likely it will end up gibberish. Why?

[ ] It doesn’t, the likelihood of gibberish doesn’t change
[ ] Because the probability of prediction compounds, and thus increases overall
[ ] Because you are more likely to hit words not in the training set
[x] Because the probability that each word matches an existing phrase goes down the more words you create

7. What is a major drawback of word-based training for text generation instead of character-based generation?

[ ] Word based generation is more accurate because there is a larger body of words to draw from
[x] Because there are far more words in a typical corpus than characters, it is much more memory intensive
[ ] Character based generation is more accurate because there are less characters to predict
[ ] There is no major drawback, it’s always better to do word-based training

8. How does an LSTM help understand meaning when words that qualify each other aren’t necessarily beside each other in a sentence?

[ ] They shuffle the words randomly
[ ] They don’t
[ ] They load all words into a cell state
[x] Values from earlier words can be carried to later ones via a cell state

## Wrap up
Over the last four weeks you've gotten a grounding in how to do Natural Language processing with TensorFlow and Keras. You went from first principles -- basic Tokenization and Padding of text to produce data structures that could be used in a Neural Network.

You then learned about embeddings, and how words could be mapped to vectors, and words of similar semantics given vectors pointing in a similar direction, giving you a mathematical model for their meaning, which could then be fed into a deep neural network for classification.

From there you started learning about sequence models, and how they help deepen your understanding of sentiment in text by not just looking at words in isolation, but also how their meanings change when they qualify one another.

You wrapped up by taking everything you learned and using it to build a poetry generator!

This is just a beginning in using TensorFlow for natural language processing. I hope it was a good start for you, and you feel equipped to go to the next level!