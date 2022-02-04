In this project, we're going to be putting what we've learned into practice.

More specificially, we're going to be replicating the deep learning model behind the 2017 paper PubMed 200k RCT: https://arxiv.org/abs/1710.06071

When it was released, the paper presented a new dataset called PubMed 200k RCT which consists of ~200,000 labelled Randomized Controlled Trial (RCT) abstracts.

The goal of the dataset was to explore the ability for NLP models to classify sentences which appear in sequential order.

In other words, given the abstract of a RCT, what role does each sentence serve in the abstract?
<img width="918" alt="68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f6d7264626f75726b652f74656e736f72666c6f772d646565702d6c6561726e696e672f6d61696e2f696d616765732f30392d736b696d6c69742d6f766572766965772d696e7075742d616e642d6f75" src="https://user-images.githubusercontent.com/84591513/152385281-ce6d5338-523c-42f7-bc37-56eeb41ff950.png">

**Problem in a sentence**
The number of RCT papers released is continuing to increase, those without structured abstracts can be hard to read and in turn slow down researchers moving through the literature.

**Solution in a sentence**
Create an NLP model to classify abstract sentences into the role they play (e.g. objective, methods, results, etc) to enable researchers to skim through the literature (hence SkimLit 🤓🔥) and dive deeper when necessary.

**📖 Resources:** Before going through the code in this notebook, you might want to get a background of what we're going to be doing. To do so, spend an hour (or two) going through the following papers and then return to this notebook:

Where our data is coming from: PubMed 200k RCT: a Dataset for Sequential Sentence Classification in Medical Abstracts
Where our model is coming from: Neural networks for joint sentence classification in medical paper abstracts.
What we're going to cover
Time to take what we've learned in the NLP fundmentals notebook and build our biggest NLP model yet:

Downloading a text dataset (PubMed RCT200k from GitHub)
Writing a preprocessing function to prepare our data for modelling
Setting up a series of modelling experiments
Making a baseline (TF-IDF classifier)
Deep models with different combinations of: token embeddings, character embeddings, pretrained embeddings, positional embeddings
Building our first multimodal model (taking multiple types of data inputs)
Replicating the model architecture from https://arxiv.org/pdf/1612.05251.pdf
Find the most wrong predictions
Making predictions on PubMed abstracts from the wild
How you should approach this notebook
You can read through the descriptions and the code (it should all run, except for the cells which error on purpose), but there's a better option.

Write all of the code yourself.

Yes. I'm serious. Create a new notebook, and rewrite each line by yourself. Investigate it, see if you can break it, why does it break?

You don't have to write the text descriptions but writing the code yourself is a great way to get hands-on experience.

Don't worry if you make mistakes, we all do. The way to get better and make less mistakes is to write more code.

**📖 Resource:** See the full set of course materials on GitHub: https://github.com/mrdbourke/tensorflow-deep-learning
