LLM(Large Language Model) is a kind of Deep Learning Model which possess the ability to understand, interpret, and generate human like text. Large in this context denotes both the amount of paramters and data involved. 

LLMs are trained to perform a task called **Next Word Prediction**. Though it seems to be a very simple problem, solving this also helps producing solutions for many inherent problems that involves understanding the syntax and semantics of a language. 

By employing the use of Transformers, they are able to achieve selective attention to certain parts of inputs that helps in understanding the nuances and enhances prediction. 

There are two main stages in building and using an LLM
1. Pretraining - Train the model with large data for Next Word Prediction (Also called base or foundation model)
2. Finetuning - Use the pretrained model on labelled data for specific tasks
	1. Instruction Finetuning - The labelled data consists of instruction and answer pairs
	2. Finetuning for classification - The labelled data consists of texts and their associated labels

