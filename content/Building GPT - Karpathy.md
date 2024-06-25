The below are the main steps involved in building a GPT
1. Load the training data (Obviously :D)
2. Get all the unique characters, vocabulary size
3. Tokenize the text (Convert string to some integer (Just a representation of a word - doesn't represent context) There are many tokenizers available. Choose your favourite one - Mine is OAI's tiktoken)
4. Provide input to the transformer in form of chunks of size (batch_size X block_size)
	A little context about this - A transformer is a neural network model used in predicting next word given the context ( Positional occurence of words ). 
	What is a block size:
	A block is used to split the training data into multiple blocks. Each block consists of multiple training examples in itself. For example, let's say that a block of size 4 is represented by a vector v = \[17,29,31,24]. It has the following training examples:
		Context = \[17]; Output = \[29]
		Context = \[17, 29]; Output = \[31]
		Context = \[17, 29, 31]; Output = \[24]
	Block size can also be thought of as context window size in this case.
	What is a batch size:
	Batch size is just a list of blocks. It is used to train multiple chunks of text in parallel. 
5. Building baseline model - can be used for experimentation, not for actual use.

After this, I realised I need to visit his previous lectures to make sense of what he is talking about. Hence, I dived into the makemore lecture. Check out the notes for them here [[Makemore - Karpathy]]

