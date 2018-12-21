# Named-Entity-Recognition-BLSTM-CNN-CoNLL
  Keras implementation of the Bidirectional LSTM and CNN model similar to Chiu and Nichols (2016) for CoNLL 2003 news data. Paper: https://arxiv.org/abs/1811.05468

This code is from https://github.com/mxhofer/Named-Entity-Recognition-BidirectionalLSTM-CNN-CoNLL
Here is the corresponding Medium post with more details: https://medium.com/@maxhofer/deep-learning-for-named-entity-recognition-2-implementing-the-state-of-the-art-bidirectional-lstm-4603491087f1

# The difference from the original code:
    1) initiate method(lecun uniform is the best score)
    2) Layer Position(The Embedding vectors are inputed to BLSTM before be concatenated)

# Result 
   The implementation achieves a test F1 score of 82.86 with 10 epochs.
   Increase the number of epochs to 80 reach an F1 over 90.

# Dataset
  CoNLL-2003 newswire articles: https://www.clips.uantwerpen.be/conll2003/ner/
  GloVe vector representation from Jeffrey Pennington, Richard Socher, and Christopher D. Manning. 2014.
  See https://nlp.stanford.edu/projects/glove/

# Dependencies 
    1) numpy 1.15.4
    2) Keras 2.1.6
    3) Tensorflow 1.8.0
    4) Stanford GloVE embeddings
    need to install pydot, graphviz(pip install doesn't work, do make install)
