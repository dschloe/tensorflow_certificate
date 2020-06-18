## Check out the code! - Using API
Let's take a look at the first [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%201%20-%20Lesson%201.ipynb) for this week.

## Check out the code! - Padding
Let's take a look at the second [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%201%20-%20Lesson%202.ipynb#scrollTo=rX8mhOLljYeM) for this week.

## News headlines dataset for sarcasm detection
The following is the public domain dataset based on sarcasm, as depicted in the previous video.

The link is provided here for your convenience:

[Sarcasm in News Headlines Dataset by Rishabh Misra](https://rishabhmisra.github.io/publications/)

## Check out the code!
Let's take a look at the third [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%201%20-%20Lesson%203.ipynb) for this week.

## Week 1 Quiz

1. What is the name of the object used to tokenize sentences?

[ ] WordTokenizer
[ ] CharacterTokenizer
[ ] TextTokenizer
[ ] Tokenizer

2. What is the name of the method used to tokenize a list of sentences?

[ ] tokenize(sentences)
[ ] tokenize_on_text(sentences)
[ ] fit_to_text(sentences)
[ ] fit_on_texts(sentences)

3. Once you have the corpus tokenized, what’s the method used to encode a list of sentences to use those tokens?

[ ] texts_to_sequences(sentences)
[ ] texts_to_tokens(sentences)
[ ] text_to_sequences(sentences)
[ ] text_to_tokens(sentences)

4. When initializing the tokenizer, how to you specify a token to use for unknown words?

[ ] unknown_token=<Token>
[ ] unknown_word=<Token>
[ ] oov_token=<Token>
[ ] out_of_vocab=<Token>

5. If you don’t use a token for out of vocabulary words, what happens at encoding?

[ ] The word isn’t encoded, and is skipped in the sequence
[ ] The word isn’t encoded, and is replaced by a zero in the sequence
[ ] The word isn’t encoded, and the sequencing ends
[ ] The word is replaced by the most common token

6. If you have a number of sequences of different lengths, how do you ensure that they are understood when fed into a neural network?

[ ] Use the pad_sequences object from the tensorflow.keras.preprocessing.sequence namespace
[ ] Make sure that they are all the same length using the pad_sequences method of the tokenizer
[ ] Specify the input layer of the Neural Network to expect different sizes with dynamic_length
[ ] Process them on the input layer of the Neural Netword using the pad_sequences property

7. If you have a number of sequences of different length, and call pad_sequences on them, what’s the default result?

[ ] They’ll get padded to the length of the longest sequence by adding zeros to the end of shorter ones
[ ] Nothing, they’ll remain unchanged
[ ] They’ll get cropped to the length of the shortest sequence
[ ] They’ll get padded to the length of the longest sequence by adding zeros to the beginning of shorter ones

8. When padding sequences, if you want the padding to be at the end of the sequence, how do you do it?

[ ] Pass padding=’post’ to pad_sequences when initializing it
[ ] Call the padding method of the pad_sequences object, passing it ‘after’
[ ] Call the padding method of the pad_sequences object, passing it ‘post’
[ ] Pass padding=’after’ to pad_sequences when initializing it

