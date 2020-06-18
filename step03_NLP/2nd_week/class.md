## IMDB reviews dataset

Please find the link to he IMDB reviews dataset [here](http://ai.stanford.edu/~amaas/data/sentiment/)
You will find here 50,000 movie reviews which are classified as positive of negative.

## Check out the code!
Let's take a look at the first [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%202%20-%20Lesson%201.ipynb) for this week.

## Check out the code!
Let's take a look at the second [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%202%20-%20Lesson%202.ipynb) for this week.

## TensorFlow datasets
Please find [here](https://github.com/tensorflow/datasets/tree/master/docs/catalog) the datasets GitHub url.
For more information, please checkout the [TensorFlow datasets documentation](https://www.tensorflow.org/datasets/catalog/overview).

## Diving into the code (Part1)
The URL shown in the video is outdated. Please use the updated URL shown below:
https://github.com/tensorflow/datasets/tree/master/docs/catalog

The URL shown in the video is outdated. Please use the updated URL shown below:
https://github.com/tensorflow/datasets/blob/master/docs/catalog/imdb_reviews.md

## Subwords text encoder
Please find the url [here](https://www.tensorflow.org/datasets/api_docs/python/tfds/features/text/SubwordTextEncoder)

## Check out the code! - 
Let's take a look at the third [notebook](https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%202%20-%20Lesson%203.ipynb) for this week.

## Week 2 Quiz

1. What is the name of the TensorFlow library containing common data that you can use to train and test neural networks?

[ ] TensorFlow Data
[ ] TensorFlow Data Libraries
[ ] There is no library of common data sets, you have to use your own
[x] TensorFlow Datasets

2. How many reviews are there in the IMDB dataset and how are they split? incorrect

[x] 50,000 records, 50/50 train/test split
[ ] 50,000 records, 80/20 train/test split
[ ] 60,000 records, 80/20 train/test split
[ ] 60,000 records, 50/50 train/test split

3. How are the labels for the IMDB dataset encoded?

[ ] Reviews encoded as a number 1-10
[ ] Reviews encoded as a boolean true/false
[x] Reviews encoded as a number 0-1
[ ] Reviews encoded as a number 1-5

4. What is the purpose of the embedding dimension? incorrect

[x] It is the number of dimensions for the vector representing the word encoding
[ ] It is the number of letters in the word, denoting the size of the encoding
[ ] It is the number of words to encode in the embedding
[ ] It is the number of dimensions required to encode every word in the corpus

5. When tokenizing a corpus, what does the num_words=n parameter do?

[x] It specifies the maximum number of words to be tokenized, and picks the most common ‘n’ words
[ ] It specifies the maximum number of words to be tokenized, and stops tokenizing when it reaches n
[ ] It specifies the maximum number of words to be tokenized, and picks the first ‘n’ words that were tokenized
[ ] It errors out if there are more than n distinct words in the corpus

6. To use word embeddings in TensorFlow, in a sequential layer, what is the name of the class?

[ ] tf.keras.layers.WordEmbedding
[ ] tf.keras.layers.Embed
[x] tf.keras.layers.Embedding
[ ] tf.keras.layers.Word2Vector

7. IMDB Reviews are either positive or negative. What type of loss function should be used in this scenario?

[ ] Categorical crossentropy
[x] Binary crossentropy
[ ] Adam
[ ] Binary Gradient descent

8. When using IMDB Sub Words dataset, our results in classification were poor. Why? incorrect

[ ] Our neural network didn’t have enough layers
[ ] The sub words make no sense, so can’t be classified
[ ] We didn’t train long enough
[x] Sequence becomes much more important when dealing with subwords, but we’re ignoring word positions

## Week 2 Wrap up

This week you looked at taking your tokenized words and using Embeddings to establish meaning from them in a mathematical way. Words were mapped to vectors in higher dimensional space, and the semantics of the words then learned when those words were labelled with similar meaning. So, for example, when looking at movie reviews, those movies with positive sentiment had the dimensionality of their words ending up ‘pointing’ a particular way, and those with negative sentiment pointing in a different direction. From this, the words in future sentences could have their ‘direction’ established, and from this the sentiment inferred. You then looked at sub word tokenization, and saw that not only do the meanings of the words matter, but also the sequence in which they are found.

You’ll look into that next week.

