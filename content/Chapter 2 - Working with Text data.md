Models - can't understand text data (can only munch numbers). There are ways to convert text to numerical data. This chapter will be predominantly discussing about that.
The sequence of text data -> continuous valued vectors -> Embedding. 
Embedding is a mapping established from the data of interest (audio, video or text documents) to a vector space. One of the most popular word embedding techniques -> Word2Vec
Word2Vec assumes the words that appear in similar context has similar meanings.

#### Byte Pair Encoders

A simple tokenizer is implemented using the vocabulary of the text data being used. Let's say that we have a word that's not in the vocabulary, it won't be able to provide a corresponding token value. Byte Pair Encoder is a technique which is used to tokenise even the unseen words, by breaking the unknown word into parts. (Todo: Have to look into the implementation in detail)

The remaining part of the chapter 2 is mainly concentrated on implementation of Tokenizers. 
Code repository for the same: https://github.com/saipragathi0912/LLM-from-scratch-python/tree/text_tokenization

##### Miscellaneous
Pytorch's Dataset and DataLoader class:
![[https://drive.google.com/file/d/1fY89iq-R-V5LhnGLOkgzWZWp2fVa67L1/view?usp=drive_link]]
Dataset -> Create datasets to train the models efficiently. It creates a custom class that defines how individual data is recorded
DataLoader -> Handles shuffling, in different batch sizes and more stuff  